# Fila de vacinação de uma clínica

## Contexto

Quando uma vaga é liberada, painel, aplicativo, SMS e equipe de recepção precisam reagir. Novos meios de aviso devem ser adicionados sem alterar o serviço que publica a vaga.

## Primeira entrega

Notifique o painel e a recepção quando uma vaga aparecer.

## Mudança realista

O paciente pode cancelar a inscrição em SMS, e observadores temporários precisam ser removidos para não receber eventos antigos. Uma falha em um canal não deve impedir os demais.

## Critérios de aceitação

- O publicador não conhece implementações concretas dos observadores.
- Inscrição e remoção são explícitas.
- Cada observador reage ao mesmo evento conforme sua responsabilidade.
- Falha isolada de um canal não interrompe a distribuição.
