# Reembolso de compra no cartão

## Contexto

Um pedido de reembolso passa por atendente, supervisor, antifraude e financeiro conforme valor, prazo e motivo. Cada etapa pode resolver, rejeitar ou encaminhar sem conhecer a cadeia inteira.

## Primeira entrega

Atenda reembolsos pequenos dentro do prazo diretamente no suporte.

## Mudança realista

Valores altos precisam de supervisor, compras suspeitas precisam de antifraude e o financeiro executa o pagamento. Uma nova conferência de cupom deve ser inserida sem editar todos os handlers.

## Critérios de aceitação

- Cada handler decide se resolve ou encaminha.
- A cadeia pode ser configurada em ordem explícita.
- Nenhum handler conhece todos os demais.
- Um pedido sem responsável termina com resultado claro.
