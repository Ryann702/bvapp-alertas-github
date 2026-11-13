# Dúvidas para esclarecimento

As lacunas abaixo permanecem abertas. As regras observadas no código servem para identificar diferenças e precisam de validação quando excedem os critérios fornecidos.

## D01

Confirmar frequência da rotina, horário, fuso e comportamento em execução interrompida.

## D02

Definir cálculo sem OS anterior e unidade da periodicidade. O código usa última realização ou data de início. Confirmar equivalência de última realização com última OS executada.

## D03

Confirmar inclusão de exatamente sete dias, manutenção no próprio dia, vencimentos e referência de data ou instante.

## D04

A US #25236 menciona sete dias, mas ordem_servico_job.py usa três dias para proximidade do início. servico_job.py usa sete dias para serviço periódico. Esclarecer a função pretendida pela história.

## D05

Definir período de verificação e chave de duplicidade. O código usa janela de sete dias para serviço periódico. Confirmar essa interpretação com os stakeholders.

## D06

Confirmar se TECNICO do código equivale a Gestor Técnico, como tratar ausência de gestores e se o solicitante pode receber. O código inclui solicitante e perfil técnico, enquanto #25229 restringe o envio ao Gestor Técnico.

## D07

Definir apresentação de serviço sem ativo ou com vários ativos.

## D08

Definir campos do histórico, granularidade por destinatário, momento do registro e tratamento de falhas e tentativas.

## D09

Definir prazo e comportamento da atualização automática da lista.

## D10

Definir estados após visualização e tratamento, efeito por usuário, repetição da marcação e significado de tratar a manutenção.

## D11

Definir comportamento ao navegar para registro removido, indisponível ou sem permissão.

## D12

Alinhar os títulos das US e features à organização dos requisitos RF03011 a RF03013. A US #25259 tem título de rotina e corpo de consulta. Verificar vínculo do CA #25251, que aparece na hierarquia, mas não na lista visível de relações dessa US.