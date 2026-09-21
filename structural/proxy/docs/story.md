# Acesso a laudos de exames

## Contexto

O portal mostra laudos armazenados em um serviço lento e protegido. O usuário só pode abrir exames próprios, a miniatura deve carregar rapidamente e o download precisa ser auditado.

## Primeira entrega

Exiba a miniatura e permita abrir um laudo autorizado.

## Mudança realista

O serviço remoto passa a responder lentamente. A aplicação deve aplicar autorização, cache e carregamento sob demanda sem alterar a interface usada pela tela.

## Critérios de aceitação

- O proxy mantém o mesmo contrato do serviço real.
- Usuários sem permissão não acionam o serviço remoto.
- Miniaturas podem ser carregadas sob demanda e armazenadas em cache.
- Downloads geram registros de auditoria.
