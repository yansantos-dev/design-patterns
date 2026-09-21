# Mapa de bicicletas compartilhadas

## Contexto

O mapa exibe milhares de bicicletas. Muitas compartilham modelo, ícone, cor e regras de manutenção; apenas posição, bateria e identificação mudam por bicicleta.

## Primeira entrega

Mostre bicicletas no mapa reutilizando os dados que são iguais entre unidades do mesmo modelo.

## Mudança realista

O volume cresce dez vezes em horários de pico. O sistema deve reduzir memória sem confundir o estado individual nem alterar o modelo compartilhado quando uma bicicleta for danificada.

## Critérios de aceitação

- Dados intrínsecos são compartilhados.
- Dados extrínsecos permanecem por bicicleta.
- O modelo compartilhado é imutável ou protegido.
- A criação de objetos equivalentes reutiliza a instância adequada.
