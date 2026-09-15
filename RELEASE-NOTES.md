# Pouso 0.2.0-beta.5

Camada de estabilidade e diagnóstico local do beta.

## Alterações

- Falhas recuperáveis da interface deixam de encerrar todo o aplicativo.
- Configurações ganha a ação **Copiar diagnóstico**.
- Eventos técnicos permanecem locais e não contêm mensagens de exceção, nomes, caminhos ou conteúdo de arquivos.
- O registro é limitado e rotacionado para não crescer indefinidamente.
- Testes adicionais cobrem CSV bloqueado e codificação incomum.

O Pouso não envia telemetria automaticamente.

Esta compilação ainda não possui assinatura Authenticode e pode exibir um aviso do Windows SmartScreen.
