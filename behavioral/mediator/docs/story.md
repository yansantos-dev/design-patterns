# Cozinha de restaurante por delivery

## Contexto

Pedido, cozinha, entregador e cliente trocam mensagens e estados. Quando cada componente fala diretamente com todos os outros, uma alteração no tempo de preparo quebra várias integrações.

## Primeira entrega

Coordene um pedido desde a confirmação até a retirada pelo entregador.

## Mudança realista

A cozinha informa atraso, o cliente cancela e o entregador pode ser substituído. Essas mudanças devem ser coordenadas sem adicionar novas dependências diretas entre todos os participantes.

## Critérios de aceitação

- Participantes conversam por uma coordenação central.
- A regra de transição fica no mediador adequado.
- Um novo participante não exige alterar todos os existentes.
- Cancelamentos e atrasos geram estados observáveis.
