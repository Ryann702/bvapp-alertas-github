# Evidências da implementação e limites da especificação

Revisão estática dos ZIPs bvapp-backend-master.zip e bvapp-frontend-main.zip fornecidos pelo estudante. Não houve execução do sistema nem dos cenários. Os caminhos abaixo são relativos à raiz de cada projeto extraído. O comportamento implementado não substitui a aprovação dos requisitos.

| Fonte | Observação | Consequência documental |
| --- | --- | --- |
| Backend: src/bvapp/scheduler/servico_job.py, _proxima_data_prevista | Soma periodicidade em dias à última realização ou, na ausência, à data de início | UC002 usa datas concretas; fallback fica em D02 |
| Mesmo arquivo, _alerta_recente_para_servico | Consulta alertas recentes pelo serviço e janela temporal | UC004 exige validação da definição de período em D05 |
| Mesmo arquivo, _criar_alerta_servico_periodico | Associa solicitante e perfil TECNICO; descrição inclui previsão e periodicidade | UC005 confronta exclusividade de Gestor Técnico; UC006 exige conferir também ativo, não garantido pela descrição construída |
| Mesmo arquivo, _tem_ordem_servico_nao_finalizada | Existe verificação de OS não finalizada | Validar se a existência de OS deve impedir alertas; essa restrição não foi adicionada aos CAs |
| Backend: src/bvapp/services/alertas/alerta_service.py, update_alerta_leitura | Grava lido e lido_em no vínculo com usuário | UC009 diferencia leitura de status geral; alcance por destinatário requer confirmação |
| Mesmo arquivo, create_alerta, update_alerta e delete_alerta | Existe manutenção genérica de alertas, com remoção lógica | O código tem CRUD. Os três RF enviados não especificam esse CRUD; confirmar se pertence à responsabilidade do estudante antes de ampliá-la |
| Frontend: src/components/features/alertas/notification-bell.tsx | Sino permite marcar leitura e oferece link /area-cooperado/feed-alertas | Caminho utilizado nos UC006 e UC009 |
| Frontend: src/components/features/alertas/alertas-feed-section.tsx | Ação Marcar lido; apresenta título, descrição resumida, data de início, status e severidade | UC008 distingue início do alerta da previsão da manutenção; UC009 usa a ação existente |
| Mesmo componente, alertasQuery e markAsReadMutation | Consulta com useQuery e invalidação após leitura; não há refetchInterval nesse trecho | Não comprova atualização automática por geração de alerta. UC008 mantém D09 |
| Mesmo componente, cartões do feed | Nos cartões examinados não há acesso direto ao serviço/OS | UC010 especifica o CA25253 e orienta registrar ausência do acesso como divergência, sem inventar botão |

## Decisões de escopo

Os dez cenários detalham RF03011, RF03012 e RF03013. Não foram acrescentados filtros, exportação, cadastro manual, edição genérica ou remoção de alertas como exigências. Essas funcionalidades podem existir no projeto completo, mas não aparecem nos 17 critérios fornecidos para este recorte.

D13 — Confirmar com o professor/equipe se a responsabilidade por Gestão de Alertas inclui também o CRUD genérico identificado no código. Se incluir, organizar os requisitos correspondentes antes de acrescentar um cenário de manutenção com as quatro operações.

D14 — Confirmar se uma OS não finalizada impede o alerta de serviço periódico e como esse comportamento se relaciona aos critérios de manutenção preventiva.

## Referências de formato

- https://github.com/LucaMarques/bvapp-cenarios-gestao-servicos — branch entrega; UC002 consultado para massa concreta, resultados precisos e passos numerados.
- https://github.com/fariassmari/bvapp-cenarios-gestao-ordens-servico — branch main; UC001 consultado para organização FP, alternativas e regras numeradas.

As referências orientam a apresentação. Regras de serviços e ordens de serviço desses repositórios não foram copiadas para alertas.
