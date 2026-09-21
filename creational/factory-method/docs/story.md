# Roteamento de entregas de um pequeno comércio

## Contexto

Uma loja vende pelo site, por um marketplace e por mensagens. Cada canal precisa criar uma entrega com etiqueta, prazo e código de rastreio diferentes. O checkout não deve conhecer a classe concreta do parceiro logístico.

## Primeira entrega

Feche pedidos recebidos pelo site e gere uma entrega para o parceiro padrão. O fluxo deve registrar o pedido, criar a entrega e mostrar o rastreio.

## Mudança realista

A loja adere a um armário inteligente e depois a uma transportadora de bicicleta. Incluir cada canal não pode transformar o checkout em uma sequência de `if` e `switch`.

## Critérios de aceitação

- O fluxo de fechamento trabalha com a abstração de entrega.
- Cada canal decide qual produto concreto deve ser criado.
- Adicionar um canal não exige editar o código comum do checkout.
- A etiqueta e o rastreio seguem o contrato da entrega.

## Perguntas para explorar

Quem deve ser responsável por decidir a classe concreta? A criação pode ser postergada até o momento em que o fluxo realmente precisa da entrega?
