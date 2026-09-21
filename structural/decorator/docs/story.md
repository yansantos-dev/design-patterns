# Recibo de feira com benefícios

## Contexto

Um recibo básico pode receber desconto de feira, arredondamento solidário, cashback e conversão para nota fiscal. A ordem das opções muda o valor final, e cada campanha deve ser ativável sem criar uma classe para cada combinação.

## Primeira entrega

Calcule o total de uma compra simples e permita aplicar um desconto.

## Mudança realista

Uma campanha temporária adiciona cashback e outra exige nota fiscal. As opções devem ser combináveis e cada camada precisa poder ser testada isoladamente.

## Critérios de aceitação

- Todas as opções preservam o contrato do recibo.
- Decoradores podem ser encadeados em qualquer composição válida.
- O cálculo básico não conhece as campanhas.
- A ordem do encadeamento é explícita e testável.
