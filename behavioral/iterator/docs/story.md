# Histórico de compras com paginação

## Contexto

O histórico pode vir de memória, banco local ou API paginada. A tela precisa avançar pelos pedidos sem conhecer como cada fonte armazena ou busca os dados.

## Primeira entrega

Mostre os pedidos do cliente em ordem cronológica usando uma coleção em memória.

## Mudança realista

O histórico cresce e passa a ser carregado por páginas. Filtros e carregamento tardio devem ser introduzidos sem expor a lista interna nem reescrever a tela.

## Critérios de aceitação

- A tela percorre uma abstração de iteração.
- A fonte pode ser trocada sem mudar o consumidor.
- O iterador controla posição e fim dos dados.
- Paginação não carrega tudo antes do primeiro resultado.
