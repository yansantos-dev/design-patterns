# Relógio de expediente em quiosques offline

## Contexto

Vários componentes de um quiosque consultam uma fonte de horário sincronizado para decidir abertura, pausa e fechamento. Quando a rede cai, criar relógios independentes pode fazer o caixa e o painel tomarem decisões diferentes.

## Primeira entrega

Ofereça uma única fonte de horário para todos os componentes do quiosque. Ela deve guardar o instante da última sincronização e permitir consultas consistentes.

## Mudança realista

Os testes precisam usar um relógio controlado, e uma futura versão pode substituir a implementação por uma fonte remota. O acesso global não pode tornar o código impossível de testar.

## Critérios de aceitação

- Todas as partes do quiosque consultam a mesma instância.
- A inicialização é segura em cenários concorrentes.
- O estado global não pode ser criado acidentalmente duas vezes.
- Existe uma forma clara de substituir a dependência em testes.

## Perguntas para explorar

O problema realmente exige uma única instância ou uma dependência compartilhada seria melhor? Como evitar que Singleton vire estado global escondido?
