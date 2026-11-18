# BVapp — Gestão de Alertas de Serviços

Autor: Ryan Monteiro Gomes. Entrega documental de dez cenários; nenhuma implementação ou execução de testes integra este pacote.

## Organização

- [Requisitos funcionais](requisitos/requisitos-funcionais.md)
- [Cenários numerados](functional_tests/README.md)
- [Rastreabilidade](docs/rastreabilidade.md)
- [Dúvidas de requisitos](docs/pendencias.md)
- [Evidências e divergências do BVapp](docs/evidencias-bvapp.md)

## Convenções

UC identifica o cenário; FP identifica o fluxo principal; A1, A2 e A3 identificam alternativas; RN1 identifica as regras. Cada fluxo reinicia sua numeração em 1. Uma referência como UC009/FP.4 identifica uma ação específica. As alternativas indicam ponto de origem, preparação e retorno ou encerramento.

O escopo normativo é RF03011–RF03013 e seus 17 critérios de aceitação. O código foi consultado estaticamente para identificar telas, ações e diferenças; não foi executado. O CRUD genérico existente no sistema não foi incorporado como requisito aprovado de manutenção preventiva.

Para publicar, extraia este ZIP e substitua os arquivos documentais anteriores. Remova a pasta antiga bvapp/alertas/tests/cenarios para não manter versões conflitantes.
