# Rascunho de anúncio de imóvel

## Contexto

Um corretor edita título, preço, fotos e descrição. Ele precisa desfazer alterações sem que o editor conheça os detalhes de como o histórico deve ser armazenado.

## Primeira entrega

Permita salvar um rascunho e desfazer a última alteração.

## Mudança realista

O histórico terá limite de vinte versões, permitirá restaurar uma versão antiga e não poderá expor o estado interno do editor para outros componentes.

## Critérios de aceitação

- O estado pode ser restaurado sem expor seus detalhes.
- O histórico pertence ao componente responsável por cuidar dele.
- Restaurar uma versão não corrompe as demais.
- O limite de versões é aplicado de forma previsível.
