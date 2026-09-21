# Escala de entregadores

## Contexto

O sistema calcula rotas por menor distância, menor custo, menor emissão ou prioridade para clientes idosos. A política pode mudar por horário e região.

## Primeira entrega

Despache uma entrega usando a rota de menor distância.

## Mudança realista

Em dias de chuva, a operação prioriza segurança; em regiões congestionadas, prioriza emissão. O despacho não deve conhecer detalhes dos algoritmos nem ganhar uma subclasse para cada política.

## Critérios de aceitação

- O algoritmo pode ser trocado em tempo de execução.
- O despacho depende de uma abstração de cálculo.
- Cada política pode ser testada isoladamente.
- Adicionar uma política não altera o fluxo de despacho.
