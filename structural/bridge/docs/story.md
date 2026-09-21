# Notificações por canal e urgência

## Contexto

A central de um condomínio envia avisos informativos, alertas de manutenção e emergências. Cada aviso pode sair por SMS, aplicativo, ligação automática ou painel físico, com regras de confirmação e repetição diferentes.

## Primeira entrega

Envie um alerta de manutenção por SMS e registre se houve confirmação.

## Mudança realista

A administração quer adicionar painel físico e ligação automática, além de uma nova categoria de emergência. O sistema não deve criar uma classe para cada combinação de categoria e canal.

## Critérios de aceitação

- O tipo de aviso pode variar independentemente do canal.
- Cada canal implementa sua própria forma de entrega.
- Uma nova combinação não exige duplicar hierarquias.
- Regras de urgência permanecem na abstração adequada.
