# Etiquetas de produtos sazonais

## Contexto

Uma confeitaria mantém etiquetas aprovadas para bolos e kits de festa. O operador duplica uma etiqueta, troca sabor, validade e lote, mas não pode alterar o modelo original nem compartilhar acidentalmente a lista de alergênicos mutável.

## Primeira entrega

Permita duplicar uma etiqueta aprovada e personalizar os dados do novo lote. A etiqueta original deve continuar pronta para ser usada como modelo.

## Mudança realista

Algumas etiquetas possuem objetos internos, como composição nutricional e lista de alergênicos. A cópia precisa ser independente para que uma alteração no novo produto não apareça nos demais.

## Critérios de aceitação

- A cópia mantém os dados aprovados do modelo.
- Campos de lote podem ser alterados sem modificar a origem.
- O estado mutável interno não é compartilhado indevidamente.
- O código que duplica não conhece todas as classes internas.

## Perguntas para explorar

A cópia deve ser rasa ou profunda? Quais campos são identidade do modelo e quais pertencem ao lote?
