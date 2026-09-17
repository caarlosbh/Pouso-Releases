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
