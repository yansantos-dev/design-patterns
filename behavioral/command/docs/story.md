# Rotina de fechamento de loja

## Contexto

Fechar uma loja envolve baixar portas, desligar letreiros, conferir estoque e enviar relatório. O gerente quer executar, desfazer a última ação quando possível e registrar quem acionou cada comando.

## Primeira entrega

Execute a rotina manualmente e registre cada ação feita.

## Mudança realista

O fechamento passa a ser agendável e pode falhar parcialmente. No dia seguinte, o sistema deve reexecutar somente as ações que falharam e permitir desfazer a última ação reversível.

## Critérios de aceitação

- Cada ação é um objeto independente.
- O invocador não conhece os detalhes do receptor.
- Histórico e agendamento usam o mesmo comando.
- A reversibilidade é explícita por comando.
