# Pouso 0.2.0-beta.12

Recuperação segura de envios interrompidos para o Google Drive.

## Novidades

- O Pouso identifica uploads pendentes na próxima abertura e oferece **Retomar**, **Recomeçar** ou **Descartar**.
- A retomada reconcilia arquivos e pastas já confirmados no Drive e envia somente o que falta.
- Um arquivo interrompido no meio da transferência é reenviado desde o início; os demais arquivos confirmados não são duplicados.
- Cada item remoto recebe um marcador privado e determinístico para impedir duplicação durante a recuperação.
- Uma permissão pública criada antes de uma queda de conexão é reconhecida antes que outra seja solicitada.
- Arquivos locais são conferidos por caminho, tamanho e data de modificação antes da retomada.
- Recomeçar cria uma nova pasta sem apagar a tentativa parcial; descartar remove somente o checkpoint local.

## Segurança e privacidade

- Nenhum arquivo ou pasta do Google Drive é apagado pela recuperação.
- A sessão pendente não armazena tokens nem o segredo OAuth e é removida depois da conclusão ou do descarte.
- Nomes, caminhos e textos do envio ficam somente no computador enquanto forem necessários para uma possível retomada.

Esta compilação ainda não possui assinatura Authenticode e pode exibir um aviso do Windows SmartScreen.
