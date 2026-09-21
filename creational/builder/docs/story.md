# Orçamento de reforma recebido por áudio

## Contexto

Uma profissional autônoma recebe pedidos de reforma pelo celular. O áudio pode mencionar metragem, cômodos, acabamento, descarte de entulho, prazo e forma de pagamento em qualquer ordem. Alguns dados são opcionais, mas metragem, endereço e prazo são obrigatórios.

## Primeira entrega

Crie um orçamento válido para uma reforma simples. O objeto final deve ser imutável depois de enviado e não deve exigir um construtor com uma longa lista de parâmetros.

## Mudança realista

O mesmo orçamento precisa gerar uma visão para a cliente, uma ordem de trabalho para a equipe e um resumo para o financeiro. Novos opcionais, como seguro e taxa de urgência, devem ser adicionados sem quebrar chamadas existentes.

## Critérios de aceitação

- Campos obrigatórios são validados antes da construção.
- Opções podem ser informadas em qualquer ordem.
- O orçamento não expõe estado mutável.
- A criação continua legível quando novos opcionais aparecem.

## Perguntas para explorar

A validação pertence ao builder ou ao objeto construído? O mesmo builder deve gerar representações diferentes ou apenas um produto completo?
