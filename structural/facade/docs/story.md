# Organizar uma consulta médica

## Contexto

Marcar uma consulta exige verificar convênio, disponibilidade do médico, autorização, endereço e lembrete. O aplicativo quer oferecer um botão único sem expor a sequência desses serviços à tela.

## Primeira entrega

Agende uma consulta quando o convênio estiver válido e houver horário disponível.

## Mudança realista

A autorização do convênio passa a ocorrer antes da reserva, e falhas precisam cancelar o que já foi reservado. A tela não deve ser reescrita por causa dessa mudança de orquestração.

## Critérios de aceitação

- A tela conhece uma operação de alto nível.
- Subsistemas continuam especializados e independentes.
- A fachada define a sequência e trata falhas previsíveis.
- O acesso direto aos subsistemas continua possível para fluxos avançados.
