# Maquininha antiga no caixa novo

## Contexto

O novo caixa espera uma API de pagamento que trabalha com valores decimais e uma única confirmação. Algumas lojas ainda usam uma maquininha antiga que recebe centavos inteiros, retorna códigos numéricos e exige confirmação em duas etapas.

## Primeira entrega

Faça o caixa concluir uma venda usando a maquininha antiga sem conhecer seu protocolo.

## Mudança realista

A maquininha será substituída gradualmente. O checkout deve continuar igual enquanto o adaptador traduz valores, códigos de erro e as duas etapas de confirmação.

## Critérios de aceitação

- O caixa depende apenas da interface moderna.
- Conversões ficam concentradas no adaptador.
- Erros da maquininha são convertidos para o contrato do caixa.
- A troca do equipamento não altera o fluxo de venda.
