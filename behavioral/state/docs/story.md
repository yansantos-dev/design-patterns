# Armário inteligente de encomendas

## Contexto

Um armário pode estar disponível, reservado, ocupado, aguardando retirada ou bloqueado para manutenção. O mesmo botão tem efeitos diferentes conforme o estado atual.

## Primeira entrega

Reserve um compartimento, deposite uma encomenda e permita sua retirada.

## Mudança realista

Uma encomenda expira, uma retirada pode ser recusada por código inválido e a manutenção bloqueia novas reservas. Transições inválidas não podem ficar espalhadas em dezenas de condicionais.

## Critérios de aceitação

- Cada estado define os eventos válidos.
- Transições inválidas produzem resultado explícito.
- Adicionar um estado não exige alterar todas as regras existentes.
- O contexto não conhece detalhes internos dos estados.
