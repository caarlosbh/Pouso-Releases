# Pouso 0.2.0-beta.21

## Caixa de entrada do celular

- Nova ação **Receber do celular** no menu da bandeja.
- Arquivos colocados em **Pouso > Entrada** no Google Drive são importados para a prateleira aberta.
- Os originais permanecem no Drive e downloads incompletos não entram na prateleira.
- Identidade e versão remotas são registradas localmente para evitar duplicações.

## Organização no Google Drive

- Nova pasta principal **Pouso**, com as áreas **Entrada**, **Envios** e **Prateleiras**.
- Novos links públicos passam a ser criados em **Pouso > Envios**.
- As antigas pastas **Pouso - Envios** são preservadas para não quebrar links existentes.

## Privacidade e validação

- A caixa de entrada usa autorização Google separada e importa somente os itens de **Pouso > Entrada**.
- Nenhum arquivo original do Google Drive é alterado ou apagado durante o recebimento.
- 176 testes automatizados aprovados.

Esta compilação ainda não possui assinatura Authenticode e pode exibir um aviso do Windows SmartScreen.
