# Pouso 0.2.0-beta.17

## OCR local pesquisável

- Imagens PNG, JPEG, BMP, GIF e TIFF recebem OCR em segundo plano.
- O texto reconhecido entra automaticamente na busca da prateleira.
- A ação **Copiar texto da imagem (OCR)** entrega o resultado completo à área de transferência.
- Um selo `OCR` identifica imagens que já possuem texto pesquisável.
- O índice persiste entre reinicializações e é atualizado quando o arquivo original muda.
- O processamento ocorre uma imagem por vez, limitado a 50 MB e 100 megapixels por origem.

## Privacidade e compatibilidade

- O OCR usa o mecanismo nativo do Windows e o idioma preferido instalado no perfil do usuário.
- Nenhuma imagem nem texto reconhecido é transmitido para nuvem.
- O instalador Win32 atual é preservado; não é necessário migrar para MSIX.
- Se não houver idioma OCR disponível ou o formato não for compatível, a imagem continua funcionando normalmente.

## Ajuste de interação

- Aproximar o mouse do ícone do Pouso na bandeja não abre mais o seletor automaticamente.
- Clique esquerdo continua abrindo a prateleira e clique direito mantém todas as opções e prateleiras.
- A troca rápida por aproximação no botão de prateleiras dentro da janela permanece disponível.

Esta compilação ainda não possui assinatura Authenticode e pode exibir um aviso do Windows SmartScreen.
