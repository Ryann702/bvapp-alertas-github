# Módulo 03 - Gestão de Manutenção de Ativos

## Submódulo 04 - Gestão de Alertas de Serviços

### [RF03011] - Monitoramento automático de manutenções preventivas

Como gestor técnico, gostaria que o sistema verificasse automaticamente, em intervalos definidos, as datas de manutenção preventiva dos serviços cadastrados. A próxima manutenção deve ser calculada com base na data da última Ordem de Serviço executada somada à periodicidade do serviço. Quando a manutenção estiver prevista para ocorrer dentro de sete dias, o sistema deve gerar um alerta de manutenção preventiva, evitando alertas duplicados para o mesmo serviço dentro do mesmo período de verificação.

### [RF03012] - Envio de alertas de manutenção preventiva

Como gestor técnico, gostaria de receber alertas quando uma manutenção preventiva estivesse próxima da data prevista. Os alertas devem ser enviados a todos os usuários com perfil Gestor Técnico, exclusivamente para esse perfil, e exibidos dentro do sistema em formato de notificação. Cada alerta deve conter nome do serviço, ativo relacionado, data prevista da próxima manutenção e periodicidade do serviço. O sistema deve registrar o envio no histórico e manter o alerta pendente até que o usuário visualize ou trate a manutenção.

### [RF03013] - Consulta e acompanhamento de alertas

Como gestor técnico, gostaria de consultar os alertas de manutenção preventiva gerados em uma lista contendo, no mínimo, nome do serviço, ativo relacionado, data prevista da manutenção e status do alerta. Devo poder marcar um alerta como visualizado e acessar diretamente a página do serviço ou da Ordem de Serviço relacionada a partir dele. A lista deve ser atualizada automaticamente quando novos alertas forem gerados.
