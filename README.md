# BVapp — Cenários de Gestão de Alertas de Serviços

Autor — Ryan Monteiro Gomes

Instituto Federal da Paraíba — Verificação, Validação e Testes de Software

Dez cenários documentam os requisitos RF03011 a RF03013 do submódulo Gestão de Alertas de Serviços (#23456), integrante do Módulo 03 — Gestão de Manutenção de Ativos. Cada cenário inclui objetivo, requisitos, ator, preparação, fluxo principal, alternativas, regras, resultados esperados e autoria. A documentação descreve expectativas para execução futura.

## Cenários

| Arquivo | Requisito | Título | Critérios do OpenProject |
| --- | --- | --- | --- |
| [UC001](bvapp/alertas/tests/cenarios/UC001.md) | RF03011 | Executar a verificação automática | #25081, #25085 |
| [UC002](bvapp/alertas/tests/cenarios/UC002.md) | RF03011 | Calcular a próxima manutenção | #25082 |
| [UC003](bvapp/alertas/tests/cenarios/UC003.md) | RF03011, RF03012 | Identificar manutenção próxima e gerar alerta | #25083, #25084, #25228 |
| [UC004](bvapp/alertas/tests/cenarios/UC004.md) | RF03011 | Evitar alertas duplicados | #25086 |
| [UC005](bvapp/alertas/tests/cenarios/UC005.md) | RF03012 | Enviar alerta aos gestores técnicos | #25229 |
| [UC006](bvapp/alertas/tests/cenarios/UC006.md) | RF03012 | Apresentar notificação com informações completas | #25230, #25233 |
| [UC007](bvapp/alertas/tests/cenarios/UC007.md) | RF03012 | Registrar o envio no histórico | #25232 |
| [UC008](bvapp/alertas/tests/cenarios/UC008.md) | RF03013 | Consultar e atualizar automaticamente a lista | #25249, #25250, #25254 |
| [UC009](bvapp/alertas/tests/cenarios/UC009.md) | RF03012, RF03013 | Marcar alerta como visualizado | #25234, #25251 |
| [UC010](bvapp/alertas/tests/cenarios/UC010.md) | RF03013 | Acessar serviço ou OS a partir do alerta | #25253 |

## Documentos de apoio

- [Requisitos e hierarquia](requisitos/requisitos-funcionais.md)
- [Rastreabilidade](docs/rastreabilidade.md)
- [Dúvidas para esclarecimento](docs/pendencias.md)

## Escopo e entrega

Os critérios fornecidos cobrem geração automática, envio, consulta e visualização de alertas. A manutenção completa de cadastro de alertas com criar, consultar, atualizar e excluir depende de requisitos adicionais. Por isso, os dez cenários correspondem às funções efetivamente especificadas nas capturas.

A documentação está organizada em bvapp/alertas/tests/cenarios. Os identificadores UC são locais ao mini projeto. A numeração RF03011 a RF03013 dá continuidade aos requisitos RF03001 a RF03010 de Gestão de Ordens de Serviço no documento coletivo. Os IDs numéricos preservam os vínculos do OpenProject.

Os requisitos do submódulo estão em [requisitos/requisitos-funcionais.md](requisitos/requisitos-funcionais.md).

As dúvidas de negócio estão registradas em docs/pendencias.md, conforme a orientação da atividade. Os fluxos com resultado dependente dessas decisões devem ser complementados após esclarecimento com os stakeholders.
