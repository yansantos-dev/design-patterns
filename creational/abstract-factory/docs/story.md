# Kit operacional de uma filial

## Contexto

Uma rede de assistência técnica abriu filiais em bairros com fornecedores diferentes. Cada filial precisa de agenda, cobrança, notificações e impressão de recibos. Os componentes de um mesmo fornecedor compartilham regras de identidade visual, impostos e formatos de data; misturar componentes de fornecedores diferentes gera ordens difíceis de auditar.

## Primeira entrega

Modele uma filial usando um único fornecedor. O sistema deve criar um agendamento, uma cobrança, uma notificação e um recibo coerentes entre si.

## Mudança realista

Durante uma greve regional, uma filial precisa trocar o conjunto inteiro de fornecedores sem alterar o fluxo que atende o cliente. A troca deve ser feita por configuração, e não por condicionais espalhadas.

## Critérios de aceitação

- Todos os objetos de uma filial pertencem à mesma família de fornecedor.
- O fluxo da filial não conhece classes concretas.
- Adicionar uma nova família não altera o código do fluxo existente.
- Deve ser impossível montar um kit misturando fornecedores incompatíveis.

## Perguntas para explorar

Como representar a fábrica da filial? O que deve acontecer quando um fornecedor não oferece um dos produtos necessários?
