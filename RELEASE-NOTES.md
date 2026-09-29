# Pouso 0.2.0-beta.56

## Envio pelo menu do Explorador

- Corrige **Enviar cópia para o Pouso** e **Adicionar pasta ao Pouso** para passar o caminho completo entre aspas.
- Recupera caminhos com espaços enviados por uma integração antiga sem aspas.
- Atualiza as associações do Explorador durante a instalação.
- 275 testes automatizados .NET passaram.

Em sessões que já carregaram a ação antiga, pode ser necessário reiniciar o Explorador de Arquivos ou entrar novamente no Windows. Os arquivos originais são preservados; o Pouso adiciona cópias à Caixa de entrada.

O instalador não tem assinatura Authenticode.

---

# Pouso 0.2.0-beta.55

## Tamanho da prateleira expandida

- Em Configurações → Geral, escolha entre 75% e 100% em passos de 1%, incluindo 81%.
- O tamanho escolhido é salvo; o modo compacto permanece igual.
- Em tamanhos menores, as ações usam ícones com dicas, sem reduzir a letra dos itens.
- 274 testes automatizados .NET passaram. A conferência visual cobriu grade em 75% e 81%, e lista em 75%.

O instalador não tem assinatura Authenticode.

---

# Pouso 0.2.0-beta.54

## Visual do Pouso no Windows

- Cabeçalho, controles, prévias dos itens, troca de prateleira e Configurações seguem a identidade visual compartilhada com o Mac.
- Os fluxos de arquivos, atalhos, envios e dados locais permanecem como na beta 53.
- O instalador inclui o cliente OAuth Desktop já usado nas betas anteriores; autorizações existentes são preservadas.
- 268 testes automatizados .NET passaram. A beta 54 foi instalada e a sincronização da Caixa de entrada foi conferida neste Windows antes da reconstrução final do instalador.

O instalador não tem assinatura Authenticode.

---

# Pouso 0.2.0-beta.53

## Cleaner expanded shelf

- Add and Send are on the left; Filter and Sync are on the right; search is at the bottom.
- Sort, share history, list/grid view, grouping, shelf color, and settings are grouped in the More menu.
- Send offers iPhone or another device through the destination picker, plus a Public link.
- 268 automated .NET tests passed. The installed build was checked with the expanded-shelf visual render.

The installer is not signed with Authenticode.

---

# Pouso 0.2.0-beta.49

## Windows and iPhone beta

- Fixed the Inbox label when English is selected.
- Added iPhone as a destination for internal transfers when the matching iPhone development build publishes its device catalog.
- Bundled the Windows Google Desktop OAuth client. Sharing links, receiving from Drive, and transfers use one `drive.file` authorization; Google may ask for consent again.
- Preserved the record of already received files when the OAuth client changes for the same Google account, along with earlier share history and upload recovery.
- 264 automated .NET tests passed. Swift tests, localization checks, and the iOS Simulator build passed in CI.

After publication, the user reported successful Windows → iPhone tests on a physical device, including a large file, network interruption, resume, and no duplicates. A read-only check with the existing Google account found all 13 legacy-visible historical IDs in the sample accessible through `drive.file`; one historical file downloaded successfully. This was not an exhaustive check of all local records. The iPhone app is not included in this Windows installer. The installer is not signed with Authenticode.

---

# Pouso 0.2.0-beta.47

## Language setting fix

- Changing the app language no longer retries unchanged global shortcuts, which could prevent settings from being saved.
- If a newly chosen global shortcut conflicts with another app, the other settings are saved and the previous shortcuts remain in place.
- The selected language takes effect after restarting Pouso.
- 260 automated Windows tests passed, including a regression test for saving English after a shortcut conflict.

The installer is not signed with Authenticode.

---

# Pouso 0.2.0-beta.46

## English and Brazilian Portuguese

- English is the default for new Windows installations. Brazilian Portuguese is available in Settings.
- Existing installations keep Brazilian Portuguese until the user selects another language. Restart Pouso to apply a language change.
- The app interface, notifications, update flow, Explorer actions, and installer have English and Brazilian Portuguese text.
- Existing shelf names and Google Drive folder names remain unchanged to preserve compatibility with Mac and iPhone.
- 259 automated Windows tests passed. The translation catalog check found no missing referenced keys.

The installer is not signed with Authenticode.

---

# Pouso 0.2.0-beta.44

## Estabilidade, recuperação e segurança

- Backup local e restauração assistida das prateleiras, preservando os dados atuais antes de recuperar uma cópia.
- Gravação mais segura das prateleiras e recuperação da cópia de segurança quando o arquivo principal está inválido.
- Falhas de persistência passam a ser informadas sem encerrar silenciosamente o aplicativo ou descartar a alteração sem aviso.
- Validação mais estrita de URLs, redirecionamentos, endereços de rede e tamanho de respostas ao ler links e atualizações.
- Sincronização com o Drive verifica espaço e limites antes de importar; credenciais são isoladas por integração e buffers temporários são limpos.
- Remoção de itens e prateleiras trata falhas de gravação e limpeza preservando os dados recuperáveis.

## Validação e distribuição

- 246 testes automatizados aprovados.
- Instalador beta distribuído diretamente; sem assinatura Authenticode.

---

# Pouso 0.2.0-beta.43

## Novo ícone e abertura da miniatura

- Novo ícone com paraquedas e documento no executável, atalhos, barra de tarefas e bandeja.
- A bandeja deixa de usar a seta antiga e passa a compartilhar o ICO multirresolução do aplicativo.
- Duplo clique na miniatura compacta abre a visualização do item.
- 230 testes automatizados aprovados.
- Instalador sem assinatura Authenticode.

---

# Pouso 0.2.0-beta.35

## Envio interno para outro computador

- **Enviar para…** escolhe computador e prateleira sem criar link público.
- Arquivos, textos e links são preparados como cópias duráveis e enviados para `Pouso/Entrada`.
- A fila pode ser retomada depois de uma falha e reconcilia repetições sem duplicar o arquivo remoto.
- Catálogos incoerentes, duplicados ou destinos removidos interrompem o envio com segurança.
- Pastas continuam desabilitadas nesta primeira entrega.

## Validação desta beta

- 219 testes automatizados aprovados.
- Layout verificado entre 100% e 200%, nos temas claro, escuro e alto contraste.
- Instalador sem assinatura Authenticode.

---

# Pouso 0.2.0-beta.34

## Destinos por computador e prateleira

- O Windows publica em `Pouso/Prateleiras` um catálogo mínimo dos destinos deste computador.
- O iPhone e o Mac poderão escolher o computador e a prateleira usando o novo contrato do Drive.
- Destinos válidos entram diretamente na prateleira, sem gerar regra automática.
- Uma prateleira removida causa fallback seguro para a Caixa de entrada.
- Arquivos destinados a outro computador permanecem disponíveis no Drive e não são baixados.
- Arquivos antigos continuam usando normalmente a Caixa de entrada e as regras locais aceitas.

## Validação desta beta

- 209 testes automatizados aprovados.
- Migração preserva a deduplicação e cria uma identidade estável para o computador.
- O catálogo não contém itens, caminhos, conteúdo, OCR, tags ou credenciais.
- Instalador sem assinatura Authenticode.

---

# Pouso 0.2.0-beta.29

## Colar diretamente no Pouso

- Novo ícone de colar sempre disponível no cabeçalho da prateleira.
- **Win + Alt + P** cola arquivos, imagens ou texto no Pouso e mostra a prateleira.
- **Ctrl + Alt + P** continua apenas abrindo o aplicativo.
- Proteção contra fechamento duplicado do seletor de prateleiras.

## Validação desta beta

- 188 testes automatizados aprovados.
- Layout compacto verificado em múltiplas escalas do Windows.
- Instalador sem assinatura Authenticode.

---

# Pouso 0.2.0-beta.26

## Refinamentos da prateleira compacta

- Alça superior dedicada para mover a janela sem conflitar com os demais controles.
- Clique no nome abre o seletor visual das prateleiras recentes.
- Abertura automática por aproximação removida.
- Botão **Ver itens** compacto e centralizado.

## Validação desta beta

- 188 testes automatizados e 197 verificações de renderização WPF.
- Instalação e interação conferidas em Windows.
- Instalador sem assinatura Authenticode.

---

# Pouso 0.2.0-beta.24

## Nova experiência de prateleira

- Janela compacta por padrão, com expansão em grade ou lista.
- Busca, filtros, agrupamento, seleção e ordenação.
- Extensões visíveis nos nomes longos.
- Menu de prateleiras e ações gerais reorganizados.
- Tarefas no ícone da barra do Windows; painel ao clicar na bandeja.
- Fechar oculta a prateleira. Atalho global Ctrl+Alt+P.

## Validação desta beta

- 188 testes automatizados e 190 verificações de renderização WPF.
- Instalação, abertura e expansão conferidas em Windows.
- Múltiplos monitores e fluxos completos de arrastar/enviar ainda precisam de validação manual.
- Instalador sem assinatura Authenticode.

---

# Pouso 0.2.0-beta.22

## Recebimento direto do celular

- Novo botão **Receber do celular** no cabeçalho da prateleira.
- Arquivos enviados pelo Pouso Web entram na prateleira aberta como cópias gerenciadas.
- Os cartões importados recebem o selo **RECEBIDO** e informam a origem Google Drive.

## Sincronização discreta

- Depois da primeira conexão, o Pouso confere **Pouso > Entrada** a cada três minutos.
- Novos itens geram uma notificação do Windows sem trazer a janela para frente.
- Identidade e versão remotas continuam registradas localmente para evitar duplicações.
- Os arquivos originais nunca são alterados ou apagados do Google Drive.

## Validação

- 177 testes automatizados aprovados.
- Instalador e manifesto verificados por SHA-256.

Esta compilação ainda não possui assinatura Authenticode e pode exibir um aviso do Windows SmartScreen.
# Pouso 0.2.0-beta.45

## Áudio, cópias e imagens

- Pré-visualização de áudio dentro do Pouso com reprodução, pausa, duração e busca na faixa; não abre um player externo.
- A opção do menu de contexto do Explorador envia uma cópia independente de arquivos para a Caixa de entrada, preservando o original.
- A seleção de vários arquivos pelo menu do Explorador é encaminhada como cópias separadas.
- Exportação de imagens para JPG, PNG, BMP ou TIFF, com opções de tamanho e qualidade JPEG.
- 256 testes automatizados aprovados; tela de áudio validada visualmente.
- Instalador sem assinatura Authenticode.

---
