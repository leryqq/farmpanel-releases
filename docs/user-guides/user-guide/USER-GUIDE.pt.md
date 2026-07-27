# Guia do usuário do FarmPanel

**Painel de controle para o seu farm de contas Steam e CS2 no Windows**

Versão do documento: 1.0

🌐 [English](USER-GUIDE.md) · [Русский](USER-GUIDE.ru.md) · [Español](USER-GUIDE.es.md) · **Português** · [Français](USER-GUIDE.fr.md) · [Türkçe](USER-GUIDE.tr.md) · [Bahasa Indonesia](USER-GUIDE.id.md) · [Tiếng Việt](USER-GUIDE.vi.md) · [हिन्दी](USER-GUIDE.hi.md) · [中文](USER-GUIDE.zh.md) · [العربية](USER-GUIDE.ar.md)

---

> **Como ler este guia.** Botões, abas e status aparecem no aplicativo exatamente como estão escritos em **negrito** (por exemplo, **Add Account**, **Start**, **Running**), para que você sempre clique na coisa certa. Cada procedimento indica no que clicar, o que acontece em seguida e como confirmar o sucesso.

## Conteúdo

1. [Introdução](#1-introdução)
2. [Antes de começar](#2-antes-de-começar)
3. [Primeira execução](#3-primeira-execução)
4. [Visão geral da interface](#4-visão-geral-da-interface)
5. [Fluxos de trabalho principais](#5-fluxos-de-trabalho-principais)
6. [Tarefas comuns («Quero…»)](#6-tarefas-comuns-quero)
7. [Referência de funcionalidades](#7-referência-de-funcionalidades)
8. [Status e indicadores](#8-status-e-indicadores)
9. [Notificações](#9-notificações)
10. [Erros e solução de problemas](#10-erros-e-solução-de-problemas)
11. [Boas práticas](#11-boas-práticas)
12. [Perguntas frequentes](#12-perguntas-frequentes)

---

# 1. Introdução

## O que é o FarmPanel

O **FarmPanel** é um aplicativo de desktop para Windows que ajuda você a gerenciar muitas contas Steam e clientes de Counter-Strike 2 a partir de uma única janela. Em vez de abrir dezenas de janelas do Steam manualmente, vigiar cada uma e reiniciar as que travam, você gerencia todo o seu farm de contas de forma centralizada — a partir de um único painel claro.

O FarmPanel inicia os clientes, isola as contas umas das outras, acompanha o estado delas em tempo real e as recupera automaticamente após falhas.

> **Importante.** O FarmPanel **não é um bot nem um autofarm**. Ele não joga por você e não imita ações dentro do jogo. Ele gerencia tudo o que acontece *em volta* do jogo: iniciar os clientes, enviar convites de lobby, recuperar após falhas e dar visibilidade em tempo real de cada conta. Todas as ações dentro do jogo são realizadas por uma pessoa real.

## Que problemas ele resolve

Se você usa mais de uma conta, esta rotina é familiar:

- é preciso iniciar dezenas de clientes Steam e CS2;
- cada conta precisa funcionar separadamente, sem interferir nas outras;
- montar lobbies e enviar convites manualmente é lento e cansativo;
- um CS2 que travou precisa ser percebido e reiniciado a tempo;
- é difícil saber quem já está em partida e quem ficou preso no carregamento.

O FarmPanel elimina essa rotina e reúne todas as operações em um único aplicativo.

## Para quem é

O aplicativo foi criado para quem precisa gerenciar de forma centralizada muitas contas Steam e CS2 — de um punhado a várias centenas — com inicialização automatizada, monitoramento em tempo real e recuperação confiável após falhas.

## O que você pode fazer

- Manter todas as contas em um só lugar e encontrar rapidamente a que precisa.
- Iniciar e parar contas uma a uma ou todas de uma vez.
- Isolar cada conta em seu próprio ambiente protegido (uma sandbox).
- Formar grupos (party) de contas e colocá-los na fila de matchmaking juntos.
- Acompanhar a carga do computador, a saúde dos processos e as quedas em tempo real.
- Recuperar automaticamente as contas após uma queda ou depois que o aplicativo é fechado.
- Organizar as janelas do CS2 pelos monitores usando um layout predefinido.

![tela principal do FarmPanel (Dashboard)](../images/dashboard-overview.png)

---

# 2. Antes de começar

## Requisitos do sistema

| Item | Mínimo | Recomendado |
|---|---|---|
| Sistema operacional | Windows 10 ou 11 (64 bits) | Windows 10 / 11 (64 bits) |
| Memória | 8 GB | 32 GB |
| Disco | Qualquer | SSD |
| Contas simultâneas | 2 | 4–10 contas de CS2 |
| Resolução de tela | área de trabalho de pelo menos 1280 pixels de largura | Full HD (1920×1080) ou superior |

## O que preparar de antemão

- **O instalador do FarmPanel** — um arquivo chamado `Setup.exe` que você baixa na página de download oficial.
- **Uma chave de licença** — você a recebe com a compra. Ela tem este formato: `XXXX-XXXX-XXXX-XXXX-XXXX` (cinco grupos de quatro caracteres).
- **Os dados das suas contas Steam** — logins e senhas, e códigos do Steam Guard se você os usar. Você pode inseri-los um a um ou importar uma lista de um arquivo.
- **Uma conexão com a internet** — necessária na primeira execução para ativar a licença e, depois, para que o Steam e o CS2 funcionem.

## Permissões

- A instalação **não exige direitos de administrador** — o aplicativo é instalado apenas para a sua conta de usuário.
- Na primeira vez que você executar o instalador, o Windows pode exibir uma janela azul do **SmartScreen** (“O Windows protegeu o seu PC”) — esse é um aviso comum para programas novos. Clique em **Mais informações** e depois em **Executar assim mesmo**.
- O aplicativo pode precisar de acesso à rede (para o Steam) e às regras do Firewall do Windows. Se aparecer um aviso do firewall, permita o acesso.

## Onde seus dados ficam guardados

Logins e senhas são criptografados com a proteção nativa do Windows e ficam guardados **apenas no seu computador**. Nunca são salvos em texto puro e nunca são enviados a lugar nenhum.

---

# 3. Primeira execução

Abaixo está o caminho da instalação até um painel pronto para uso. Siga os passos na ordem.

## Passo 1. Instale o aplicativo

1. Baixe o instalador `Setup.exe` na página de download.
2. Dê um clique duplo no arquivo `Setup.exe`.
3. Se aparecer uma janela azul do **SmartScreen** (“O Windows protegeu o seu PC”), clique em **Mais informações** e depois em **Executar assim mesmo**. Esse é um aviso comum para programas novos, não um erro.
4. Aguarde a instalação terminar. Não são necessários direitos de administrador — o instalador verifica o seu sistema e prepara tudo.

**O que acontece em seguida.** Um ícone do FarmPanel aparece na sua área de trabalho e no menu Iniciar.

![a janela do instalador Setup.exe](../images/setup-installer.png)

## Passo 2. Abra o aplicativo

Dê um clique duplo no ícone do **FarmPanel** na sua área de trabalho.

**O que você verá.** Na primeira execução, enquanto a licença ainda não está ativada, a janela de ativação (**Activation Wizard**) abre. A tela principal aparece apenas após uma ativação bem-sucedida.

## Passo 3. Ative sua licença

A janela de ativação orienta você passo a passo.

1. Digite ou cole sua chave de licença no campo de entrada. Para colá-la da área de transferência, clique em **Paste from clipboard**.
2. O aplicativo verifica o formato da chave enquanto você digita. Quando o formato está correto, o botão de ativação fica disponível.
3. Clique em **Activate**.

**O que acontece em seguida.** O aplicativo entra em contato com o servidor de licenças e verifica a chave. Isso leva alguns segundos — você verá o estado **Activating**.

**Sinal de sucesso.** A janela de ativação se fecha e a tela principal do aplicativo (**Dashboard**) abre. Sua licença está ativa — você não precisará digitar a chave novamente nas próximas execuções.

> **Se a ativação falhar**, o aplicativo mostra uma mensagem clara e indica o que fazer. Os casos mais comuns estão em [10. Erros e solução de problemas](#10-erros-e-solução-de-problemas).

![a janela de ativação da licença](../images/license-activation.png)

## Passo 4. Verifique os ajustes básicos

Antes de iniciar contas pela primeira vez, vale a pena verificar seus ajustes.

1. Clique em **Settings** no painel esquerdo, ou pressione `Ctrl+,`.
2. Abra a seção **Sandboxes** e, se necessário, escolha uma pasta para as sandboxes.
3. Opcionalmente, abra **Appearance** e escolha um tema (**System / Dark / Light**) e a densidade da interface.

Os ajustes são salvos automaticamente: após cada alteração aparece uma breve notificação **Saved**.

## Passo 5. Pronto para começar

Agora você pode adicionar contas e iniciar seu primeiro farm. Veja como em [5. Fluxos de trabalho principais](#5-fluxos-de-trabalho-principais).

**Sinal de que tudo funciona.** A barra inferior da janela (a barra de status) mostra um resumo: o número de contas, os processos ativos e a versão atual do aplicativo.

---

# 4. Visão geral da interface

O aplicativo funciona em uma única janela principal. Ela é composta por elementos fixos, que estão sempre presentes, e por uma área de tela que muda conforme a seção escolhida.

```
┌────────────────────────────────────────────────────────────┐
│  Barra de comandos (Command Bar)                           │
├──────────┬─────────────────────────────────────────────────┤
│          │                                                 │
│ Barra    │   Área de trabalho da tela selecionada          │
│ lateral  │                                                 │
│          │                                                 │
├──────────┴─────────────────────────────────────────────────┤
│  Barra de status (Status Bar)                              │
└────────────────────────────────────────────────────────────┘
```

![estrutura geral da janela com as áreas identificadas](../images/window-layout.png)

## 4.1. Barra de comandos (Command Bar)

**Propósito.** Uma faixa fixa no topo da janela. Contém a navegação, a busca global e as notificações.

**Localização.** A linha superior da janela.

**Elementos principais (da esquerda para a direita):**

- **Botão de menu (☰)** — recolhe e expande a barra lateral. Atalho `Ctrl+B`.
- **Logotipo** — ao clicar, você volta à tela principal (**Dashboard**).
- **Trilha de navegação** — mostra onde você está, por exemplo `Accounts › alex_42 › Events`. Clique em qualquer segmento para ir até ele.
- **Busca / paleta de comandos** — no centro. Pressione `Ctrl+K` para abrir a paleta de comandos (veja abaixo).
- **Indicador de notificações** — um ícone com um contador (por exemplo, `⚠ 3`). Ao clicar, abre o centro de notificações.

**Quando usar.** A barra de comandos está sempre à mão: para saltar rapidamente entre telas, buscar uma conta pelo login ou executar um comando sem o mouse.

### Paleta de comandos (Command Palette)

Pressione `Ctrl+K` a qualquer momento para abrir a paleta de comandos — uma caixa de busca de todas as ações e objetos do aplicativo.

1. Comece a digitar o nome de um comando, uma tela, o login de uma conta ou um workflow.
2. A lista se reduz aos resultados correspondentes. Percorra-os com `↑` `↓`.
3. Pressione `Enter` para executar o item selecionado.

**Por que ajuda.** A paleta de comandos é a maneira mais rápida de encontrar qualquer coisa sem memorizar onde ficam os botões.

![a paleta de comandos aberta](../images/command-palette.png)

## 4.2. Barra lateral (Sidebar)

**Propósito.** A navegação principal do aplicativo.

**Localização.** À esquerda, em toda a altura da janela.

**Seções (de cima para baixo):**

| Ícone | Seção | O que mostra |
|---|---|---|
| ▤ | **Dashboard** | Visão geral de todo o farm |
| 👥 | **Accounts** | Lista de todas as contas (a tela de trabalho principal) |
| ⚙ | **Workflows** | Cenários de inicialização automatizados e seu progresso |
| ⚔ | **Matchmaking** | Grupos (party) e busca de partida |
| 📈 | **Monitoring** | Carga do computador e saúde dos processos |
| 📜 | **Logs** | O registro de eventos |
| ▣ | **Layouts** | Organização das janelas do CS2 pelos monitores |
| ▦ | **Sandboxes** | Sandboxes (ambientes isolados) |
| ⚙ | **Settings** | Ajustes do aplicativo |
| ? | **Help** | Ajuda |

Algumas seções mostram um contador (por exemplo, o número de contas) ou um ponto ativo quando há atividade.

**Ações principais:**

- Clique em uma seção para abri-la. Você também pode usar `Ctrl+1`…`Ctrl+8`.
- O botão de recolher (ou `Ctrl+B`) reduz o painel a ícones para liberar espaço.

**Dica.** Alternar entre seções preserva o seu estado — filtros, seleção e posição de rolagem. Ao voltar a uma tela, você a encontra exatamente como a deixou.

![a barra lateral com todas as seções](../images/sidebar.png)

## 4.3. Barra de status (Status Bar)

**Propósito.** Uma faixa fina na parte inferior da janela com um resumo rápido do estado de todo o farm.

**Localização.** A linha inferior da janela.

**O que mostra (exemplo):**

```
[env: PROD] | ● 412 contas (238 em execução) | ▶ 18 workflows | ◎ 7 partidas | CPU 42% RAM 71% | ⚠ 3 erros | 14:32:08 | v1.0.1
```

- quantas contas existem e quantas estão em execução agora;
- quantos workflows e partidas ativas estão em andamento;
- carga do processador e da memória;
- o número de erros (clique para abrir o centro de notificações);
- a hora e a versão do aplicativo.

**Quando usar.** Dê uma olhada na barra de status para saber em um segundo se está tudo bem.

## 4.4. Tela Dashboard

**Propósito.** Uma única tela de visão geral. Em poucos segundos, ela responde: quantas contas estão online, quantos workflows estão em execução ou falharam, se há atividade de matchmaking, se há quedas e quão carregado está o computador.

**Localização.** A primeira seção da barra lateral. Abre logo após a inicialização.

**Áreas principais:**

- **Faixa de KPIs** — cinco cartões no topo: **Accounts**, **Workflows**, **Matches**, **Errors**, **System**. Cada um mostra um número em destaque e um minigráfico. Clicar em um cartão leva à tela correspondente.
- **Live Activity Feed** — um fluxo em tempo real de eventos operacionais. Use o botão de pausa (ou a tecla `Space`) para pausar a rolagem.
- **Account State Heatmap** — uma grade em que cada conta é uma célula colorida. A cor reflete o status dela. Passe o cursor para ver o login e o status; clique para ir até a conta.
- **Active Workflows / Matchmaking Queue / Sandboxes** — três blocos que resumem os workflows, a fila de partidas e as sandboxes.
- **Failures & Crashes** — uma tabela de erros e quedas recentes da última hora.

**Uso típico.** De manhã, abra o **Dashboard** para avaliar o farm de relance e depois vá aonde é preciso dar atenção.

**Dicas.**
- As métricas se atualizam automaticamente. Para forçar uma atualização completa, pressione `F5`.
- Se algo estiver destacado em vermelho no cartão **Errors** ou na tabela de falhas, comece a investigação por ali.

![o Dashboard com a faixa de KPIs e o feed de atividades](../images/dashboard-screen.png)

## 4.5. Tela Accounts

**Propósito.** A tela de trabalho principal. Aqui você guarda as contas, encontra as que precisa e as inicia e para.

**Localização.** A segunda seção da barra lateral (`Ctrl+2`).

**Áreas principais:**

- **Barra de ferramentas** — os botões **Add Account**, **Import**, **Export** e **Refresh**, o campo de busca, os filtros e os controles de exibição.
- **Tabela de contas** — uma lista de todas as contas com colunas: status, login, apelido, rank, workflow, sandbox, tags, hora do último acesso e outras.
- **Details Pane** (painel de detalhes) — à direita. Mostra os detalhes da conta selecionada. Exiba-o ou oculte-o com `Ctrl+\`.

**O que você pode fazer:**

- Adicionar contas uma a uma ou importar uma lista.
- Buscar e filtrar contas.
- Iniciar, parar e reiniciar uma conta ou várias de uma vez.
- Vincular contas a sandboxes e atribuir workflows.
- Ver uma ficha detalhada da conta: dados, histórico, eventos e logs.

**Uso típico.** Selecione as contas que precisa na tabela e execute uma ação sobre elas — usando a barra de ferramentas, o menu de contexto (clique com o botão direito) ou os atalhos de teclado.

Instruções detalhadas passo a passo estão em [5. Fluxos de trabalho principais](#5-fluxos-de-trabalho-principais).

![a tela Accounts com a tabela e o painel de detalhes](../images/accounts-screen.png)

### Painel de detalhes da conta (Details Pane)

À direita da tabela, aparece uma ficha da conta selecionada com estas abas:

| Aba | O que mostra |
|---|---|
| **Overview** | Dados principais, vínculo de sandbox, workflow atribuído, tags, datas-chave e botões de ação |
| **Inventory** | O inventário da conta: quantidade de itens e valor |
| **Workflow** | O estado atual do cenário atribuído e seu passo atual |
| **Events** | Eventos recentes desta conta |
| **Logs** | O registro de eventos filtrado por esta conta |
| **History** | Histórico de alterações: criação, edições, renomeações, revínculos de sandbox |

Na parte inferior da aba **Overview** há um bloco de botões: **Start**, **Stop**, **Restart**, **Pause**, além de **Edit account** e **Delete**. A ação mais relevante aparece em destaque: **Start** quando a conta está parada, e **Stop** quando está em execução.

## 4.6. Tela Workflows

**Propósito.** Gerenciar cenários de inicialização automatizados e observar sua execução.

**Localização.** A terceira seção da barra lateral (`Ctrl+3`).

**O que é um workflow.** Um workflow é uma sequência de passos predefinida que o aplicativo executa para uma conta: entrar no Steam, iniciar o CS2 e assim por diante. O mesmo cenário sempre é executado da mesma forma, então o resultado é previsível.

- **Definition** (definição) — o modelo do cenário: um conjunto de passos.
- **Instance** (instância) — uma única execução de uma definição para uma conta específica.

**Áreas principais:**

- **À esquerda** — uma lista de definições (modelos) e suas versões.
- **No centro** — uma tabela de instâncias em execução: qual cenário, para qual conta, em qual passo, quantas tentativas, quando foi iniciada.
- **À direita** — detalhes da instância selecionada (abas **Overview**, **State Machine**, **Steps**, **Logs**, **Retries**).
- **Embaixo** — uma linha do tempo de eventos recolhível para as instâncias visíveis (`Ctrl+T`).

**Quando usar.** Venha aqui para ver em que passo está a inicialização de cada conta, pausar ou reiniciar um cenário, ou descobrir por que algo não terminou.

![a tela Workflows com três painéis](../images/workflows-screen.png)

## 4.7. Tela Matchmaking

**Propósito.** Formar grupos de contas (party) e colocá-los na fila de matchmaking juntos.

**Localização.** A quarta seção da barra lateral (`Ctrl+4`).

**Conceitos-chave:**

| Termo | Significado |
|---|---|
| **Party** (grupo) | Um conjunto de contas que buscam uma partida juntas |
| **Quorum** | Todos os membros do grupo estão logados, na fila e fora de partida |
| **Queue** (fila) | A espera por uma partida: posição, região, modo |
| **Match Found** (partida encontrada) | O Steam encontrou uma partida. O aplicativo confirma a prontidão de todos os membros automaticamente — você não precisa fazer nada |
| **Desync** (dessincronização) | Os membros estão em um estado inconsistente (por exemplo, alguém saiu da fila) |

**Áreas principais:**

- **À esquerda** — uma lista de grupos com o estado deles (quórum, dessincronização, partida encontrada, ocioso).
- **À direita** — detalhes do grupo selecionado: membros, o estado deles, posição na fila, latência de rede, sandbox.
- **Embaixo** — uma linha do tempo de eventos recentes de matchmaking.

**Quando usar.** Aqui você forma grupos de 2–5 contas e os coloca na fila. Quando uma partida é encontrada, o aplicativo confirma a prontidão de todos os membros automaticamente.

![a tela Matchmaking com grupos e detalhes](../images/matchmaking-screen.png)

## 4.8. Tela Monitoring

**Propósito.** Acompanhar a carga do computador, a saúde dos processos e as quedas em tempo real.

**Localização.** A quinta seção da barra lateral (`Ctrl+5`).

**Áreas principais:**

- **Medidores de recursos** — cartões de **CPU**, **RAM**, **Disk**, **Net** e, quando disponível, **GPU**, com os valores atuais e minigráficos.
- **Process Explorer** — uma tabela de todos os processos Steam e CS2 em execução: a que conta cada um pertence, quanto consome e há quanto tempo está rodando.
- **Crashes & Warnings** — um feed de falhas recentes.
- **Logs panel** — um registro na parte inferior da tela, que pode ser recolhido.

**Controles de tempo.** No topo, você pode alternar entre **Live** (tempo real), **Last 1h / 24h** (última hora/24 h) e **Custom** (um período personalizado). O botão **Freeze** (`Ctrl+Space`) congela a imagem para você estudá-la com calma.

**Quando usar.** Se o computador começar a ficar lento ou as quedas ficarem frequentes, abra o **Monitoring** para ver qual processo está consumindo recursos e o que exatamente travou.

> **Dica.** Você pode abrir a tela **Monitoring** em uma janela separada com o botão de desacoplar e colocá-la em um segundo monitor.

![a tela Monitoring com medidores e a lista de processos](../images/monitoring-screen.png)

## 4.9. Tela Logs

**Propósito.** Um registro detalhado de todos os eventos do aplicativo — como um feed ao vivo do que está acontecendo.

**Localização.** A sexta seção da barra lateral (`Ctrl+6`).

**Recursos principais:**

- **Filtro por nível** — os interruptores **Error**, **Warn**, **Info**, **Debug**. Por padrão, são exibidos erros, avisos e mensagens informativas.
- **Filtro por origem** — você pode restringir o registro a uma única conta, workflow ou sandbox.
- **Busca** — `Ctrl+F`, com salto entre ocorrências (`F3` / `Shift+F3`).
- **Follow** (acompanhar) — o registro rola automaticamente para as novas linhas. A tecla `Space` liga e desliga o acompanhamento. Se você rolar para cima, o acompanhamento pausa e aparece um botão para voltar ao fim.
- **Export** (exportar) — salvar as linhas visíveis em um arquivo.

**Quando usar.** Quando você precisa dos detalhes: exatamente o que aconteceu com uma conta específica e em que ordem.

![a tela Logs com um registro de eventos](../images/logs-screen.png)

## 4.10. Tela Layouts

**Propósito.** Organizar as janelas do CS2 por um ou vários monitores usando um layout predefinido.

**Localização.** A sétima seção da barra lateral (`Ctrl+7`).

**Conceitos-chave:**

- **Preset** (predefinição) — um arranjo de janelas salvo.
- **Slot** — uma área retangular em um monitor onde ficará uma janela.
- **Snap** (organizar) — o comando que dispõe as janelas em execução nos slots.

**Áreas principais:**

- **À esquerda** — uma lista de predefinições salvas.
- **À direita** — uma tela que mostra os seus monitores, na qual você posiciona os slots.
- **Embaixo** — uma tabela de atribuições: qual slot corresponde a qual conta ou função.

**Como usar.**
1. Crie uma predefinição com o botão **New Preset**.
2. Posicione os slots na tela.
3. Defina qual conta vai em cada slot.
4. Clique em **Apply** ou **Snap windows** — o aplicativo dispõe as janelas do CS2 em execução nos lugares definidos.

> **Rede de segurança.** Antes de organizar, o aplicativo memoriza as posições atuais das janelas. O botão **Revert layout** restaura as posições anteriores dentro de um minuto.

![a tela Layouts com a tela dos monitores](../images/layouts-screen.png)

## 4.11. Tela Sandboxes

**Propósito.** Gerenciar as sandboxes — os ambientes isolados nos quais os clientes Steam funcionam.

**Localização.** A oitava seção da barra lateral (`Ctrl+8`).

**O que é uma sandbox.** Uma sandbox é um ambiente separado e protegido para um cliente Steam. Contas em sandboxes diferentes nunca se sobrepõem: não compartilham sessões, arquivos nem rastros. Uma conta é vinculada a uma sandbox.

**Quando usar.** Aqui você cria sandboxes e acompanha o estado delas. Na maioria dos casos, as sandboxes são atribuídas automaticamente ao adicionar contas, então raramente é preciso vir aqui de propósito.

## 4.12. Tela Settings

**Propósito.** Adaptar o aplicativo às suas preferências.

**Localização.** A seção **Settings** na parte inferior da barra lateral (`Ctrl+,`).

**Estrutura.** À esquerda há uma lista de seções de ajustes; à direita, os ajustes em si. As alterações são salvas de imediato: uma breve notificação **Saved** aparece após cada uma.

**Seções de ajustes:**

| Seção | O que configura |
|---|---|
| **General** | Iniciar junto com o Windows, minimizar para a bandeja, canal de atualizações |
| **Appearance** | Tema (**System / Dark / Light**), densidade, escala da fonte, redução de animações |
| **Accounts** | Comportamento ao criar contas, retenção das excluídas |
| **Workflows** | Política de novas tentativas, limites de execuções simultâneas |
| **Sandboxes** | Pasta das sandboxes, recuperação automática |
| **Monitoring** | Frequência de atualização dos dados, limites de aviso |
| **Notifications** | Notificações e sons por nível de gravidade |
| **Layouts** | Layouts padrão, comportamento com vários monitores |
| **Hotkeys** | Atalhos de teclado — podem ser reatribuídos |
| **Advanced** | Nível de registro, diagnóstico, seleção de ambiente, restaurar padrões |
| **About** | Versão do aplicativo, botões para abrir as pastas de dados e de logs |

> **Observação.** Alguns ajustes (por exemplo, a pasta das sandboxes ou o ambiente) só se aplicam após reiniciar. Esses ajustes exibem uma etiqueta “Requires restart” ao lado.

![a tela Settings](../images/settings-screen.png)

---

# 5. Fluxos de trabalho principais

Esta é a seção mais importante. Ela contém instruções completas passo a passo para as tarefas principais. Cada passo descreve o que você verá e como confirmar o sucesso.

## 5.1. Adicionar uma única conta

**Objetivo.** Adicionar uma nova conta Steam ao aplicativo.

**O que você precisa.** O login e a senha da conta. Um código do Steam Guard, se aplicável.

### Passo 1 — Abra o formulário de cadastro

Vá para a tela **Accounts** e clique em **Add Account** na barra de ferramentas. Você também pode pressionar `Ctrl+N`.

**Resultado esperado.** Abre um formulário com campos para a nova conta.

### Passo 2 — Preencha os dados

Preencha os campos:

- **Login** — obrigatório, deve ser único.
- **Password** — obrigatório.
- **Steam Guard secret** — o código do Steam Guard, se você tiver um (opcional).
- **Nickname** — opcional; pode ser obtido automaticamente no primeiro acesso.
- **Tags** — tags opcionais para agrupar.
- **Sandbox binding** — escolha **Auto-assign**, uma sandbox específica ou **None**.
- **Workflow** — o cenário de inicialização, se quiser atribuir um de imediato.

**Resultado esperado.** Se o login já estiver em uso, o campo fica destacado em vermelho com uma explicação. Uma senha fraca fica destacada em âmbar — isso é um aviso e não impede salvar.

### Passo 3 — Salve a conta

Clique no botão de salvar do formulário.

**Resultado esperado.** O formulário se fecha e a nova conta aparece na tabela com o status **Draft** ou, se estiver vinculada a uma sandbox, pronta para iniciar.

**Sinal de sucesso.** A conta está visível na tabela da tela **Accounts**.

### Dicas

- Se você ativar **Validate immediately** no formulário, o aplicativo verifica o login em segundo plano e mostra o resultado como uma notificação.
- Para que uma conta possa ser iniciada, ela precisa estar vinculada a uma sandbox. A opção mais simples é **Auto-assign**.

### Erros comuns e como resolvê-los

- **“Login already in use.”** Esse login já existe no aplicativo. Verifique sua lista de contas — talvez você já o tenha adicionado.
- **Esqueceu a sandbox.** Uma conta sem sandbox não pode ser iniciada. Vincule uma depois pelo menu de contexto → **Bind sandbox**.

![o formulário de adição de conta](../images/accounts-add-form.png)

## 5.2. Importar uma lista de contas de um arquivo

**Objetivo.** Adicionar rapidamente muitas contas de uma vez a partir de um arquivo.

**O que você precisa.** Um arquivo com uma lista de contas (TXT, CSV ou TSV). O formato de linha TXT mais simples é `login:senha` (você também pode usar `login:senha:steamguard:apelido`).

### Passo 1 — Inicie o assistente de importação

Na tela **Accounts**, clique na seta ao lado do botão **Import** e escolha uma origem — por exemplo, **From file…**. Você também pode pressionar `Ctrl+I`.

**Resultado esperado.** Abre um assistente de importação passo a passo.

### Passo 2 — Escolha a origem e como as sandboxes são atribuídas

Aponte para o arquivo com o botão **Browse…**. Na parte de baixo, escolha como atribuir as sandboxes:

- **Auto-assign (round-robin)** — distribuir em ciclo (recomendado);
- **Bind to specific sandbox** — vincular todas a uma sandbox;
- **Leave unbound** — deixar sem sandbox.

Clique em Avançar.

### Passo 3 — Verifique como os dados foram reconhecidos

O assistente mostra as primeiras linhas do arquivo como uma tabela. Confirme que os dados foram divididos em colunas corretamente. Se o delimitador foi detectado errado, defina-o manualmente.

**Resultado esperado.** Na pré-visualização, logins e senhas estão em suas próprias colunas.

### Passo 4 — Mapeie os campos

Arraste os cabeçalhos das colunas para as células necessárias: **Login**, **Password**, **SteamGuard**, **Nickname**.

### Passo 5 — Verifique se as linhas são válidas

O assistente marca cada linha: ✓ válida, ⚠ aviso, ✕ erro. As linhas com erros podem ser corrigidas aqui mesmo ou ignoradas.

**Resultado esperado.** Você vê quantas contas serão adicionadas, quantas são duplicadas e quantas têm erros.

### Passo 6 — Confirme a importação

Clique em **Import N accounts**.

**Resultado esperado.** Aparece uma barra de progresso com o status de cada linha. Ao terminar, as contas aparecem na tabela.

**Sinal de sucesso.** O número de contas na tabela aumentou pela quantidade importada.

### Como cancelar e recuperar

Se você cancelar a importação enquanto ela está em execução, o aplicativo oferece reverter o lote já adicionado. Confirme a reversão para voltar ao estado original.

![o assistente de importação, etapa de validação das linhas](../images/import-wizard-validation.png)

## 5.3. Iniciar várias contas

**Objetivo.** Iniciar várias contas ao mesmo tempo.

**O que você precisa.** Contas já adicionadas e vinculadas a sandboxes.

### Passo 1 — Selecione as contas

Na tela **Accounts**, marque as contas desejadas na primeira coluna. Para selecionar todas as visíveis, pressione `Ctrl+A`.

**Resultado esperado.** A barra de ferramentas muda para o modo em massa e mostra quantas linhas estão selecionadas, por exemplo `12 selected`.

### Passo 2 — Inicie as contas selecionadas

Clique em **Start** na barra de operações em massa. Você também pode pressionar `Ctrl+R`.

**Resultado esperado.** O status das contas selecionadas muda para **Starting**. O aplicativo prepara cada conta e começa a iniciar. A inicialização ocorre em lotes para não sobrecarregar o computador.

### Passo 3 — Aguarde a inicialização

Observe a coluna de status. Aguarde até as contas passarem para o estado **Running**.

**Resultado esperado.** As contas iniciadas mostram **Running**, com um contador de tempo de atividade ao lado.

**Sinal de sucesso.** Todas as contas selecionadas mostram **Running**. A contagem de ativas na barra de status aumentou.

### Dicas

- Você não precisa iniciar todas as contas de uma vez. Comece com um lote pequeno, confirme que tudo está estável e depois adicione mais.
- Para iniciar uma única conta: selecione uma linha e clique em **Start**, ou use o botão **Start** no painel de detalhes à direita.

### Erros comuns e recuperação

- **Uma conta fica em Starting por muito tempo.** O login pode estar lento. Aguarde; se o status mudar para **Error**, use o botão **Retry**.
- **Algumas contas não iniciaram.** Após uma inicialização em massa, um resumo mostra quantas tiveram sucesso e quantas falharam. Clique em **Filter to failed** para tratar apenas dessas.

![inicialização em massa de contas, status Starting/Running](../images/accounts-bulk-start.png)

## 5.4. Parar todas as contas em execução

**Objetivo.** Encerrar de forma ordenada todas as contas ativas.

### Passo 1 — Selecione as contas

Selecione as contas em execução. Para selecionar todas as visíveis, pressione `Ctrl+A`.

### Passo 2 — Pare-as

Clique em **Stop** na barra de operações em massa, ou pressione `Ctrl+.` (Ctrl e ponto).

**Resultado esperado.** O aplicativo encerra de forma ordenada cada conta. O status muda para **Stopped**. Se uma conta não responder, após algum tempo o aplicativo a encerra à força.

**Sinal de sucesso.** Todas as contas mostram **Stopped**. A contagem de ativas na barra de status diminuiu.

### Dicas

- **Stop** é um encerramento ordenado. O aplicativo primeiro tenta fechar os clientes corretamente.
- Se uma conta está em partida, termine as ações dentro do jogo primeiro e depois pare.

## 5.5. Criar um grupo e colocá-lo na fila

**Objetivo.** Formar um grupo de várias contas e colocá-las na fila de matchmaking juntas.

**O que você precisa.** Várias contas em execução (**Running**) que já fizeram login.

### Passo 1 — Crie um grupo

Vá para a tela **Matchmaking** e clique em **Create Party**. Você também pode pressionar `Ctrl+N`.

**Resultado esperado.** Abre uma janela onde você pode adicionar contas ao grupo e dar um nome a ele.

### Passo 2 — Adicione membros e salve

Adicione de 2 a 5 contas ao grupo, defina um nome e salve.

**Resultado esperado.** O novo grupo aparece na lista à esquerda.

### Passo 3 — Verifique o quórum

Selecione o grupo e olhe os membros à direita. Confirme que o grupo está no estado **Quorum** — ou seja, todos os membros estão logados e prontos.

**Resultado esperado.** O grupo exibe uma etiqueta **✓ Quorum**. Se um membro tiver um problema (por exemplo, um login lento), ele é mostrado em uma linha separada.

### Passo 4 — Coloque o grupo na fila

Clique em **Queue** para o grupo selecionado (ou `Ctrl+Q`). Para colocar todos os grupos na fila de uma vez, use **Queue All** na barra de ferramentas.

**Resultado esperado.** Antes de colocar na fila, o aplicativo faz suas verificações. Depois, todos os membros entram na fila, com suas posições e a latência de rede exibidas.

**Sinal de sucesso.** Os membros estão no estado de fila, com um contador de tempo de espera em andamento.

### Dicas

- Escolha a região e o modo na barra de ferramentas (por exemplo, `EU` e `Premier`) antes de colocar na fila.
- Se o grupo entrar no estado **Desync**, use a ação **Re-sync** para pausar a fila e aguardar um estado consistente.

![um grupo na fila com as posições dos membros](../images/matchmaking-party-queue.png)

## 5.6. O que acontece quando uma partida é encontrada

**Objetivo.** Entender o que o aplicativo faz no momento em que uma partida é encontrada.

**O que você precisa.** Um grupo que esteja na fila.

### A aceitação da partida é automática

Quando o Steam encontra uma partida, aparece uma faixa destacada **MATCH FOUND** para o grupo. **Você não precisa clicar em nada** — o aplicativo confirma a prontidão de todos os membros do grupo dentro do prazo. Nenhuma ação sua é necessária.

**Resultado esperado.** Os membros do grupo aceitam a partida automaticamente; o estado deles muda para **✓ Accepted**.

**Sinal de sucesso.** Todos os membros mostram **Accepted**, e a partida começa.

> **Dica.** Quer saber que uma partida foi encontrada sem olhar para a tela? Ative um alerta sonoro para **Match found** em **Settings → Notifications**. A aceitação continua acontecendo automaticamente — o som serve apenas para manter você informado.

### O que fazer se o grupo dessincronizar

Às vezes uma partida não pode ser confirmada para todos — por exemplo, se um membro saiu da fila. O grupo então entra no estado **Desync**. Use a ação **Re-sync** e, se necessário, remova o membro problemático com **Drop member**, e coloque os demais na fila de novo.

![a faixa Match Found](../images/matchmaking-match-found.png)

## 5.7. Recuperar após uma queda ou reinício do aplicativo

**Objetivo.** Devolver o farm a um estado operacional após a queda de um cliente, ou depois que o aplicativo foi fechado e aberto de novo.

**O que você precisa.** Nada além do normal — a recuperação acontece em grande parte automaticamente.

### O que acontece automaticamente

- **Após a queda de um cliente.** Se o Steam ou o CS2 fecham inesperadamente, o aplicativo percebe, marca a conta com o status **Crashed** e mostra uma notificação com um botão **Restart**. A recuperação muitas vezes ocorre sozinha em poucos segundos.
- **Após um reinício do aplicativo.** Ao iniciar, o aplicativo procura processos Steam e CS2 que sobraram da sessão anterior e os retoma sob seu gerenciamento. Durante isso, um indicador **Recovering** aparece na barra de status. As contas readotadas são marcadas com “Reattached” por um breve período.

### O que fazer manualmente

1. Abra o **Dashboard** e olhe a tabela **Failures & Crashes**.
2. Para uma conta que caiu, clique em **Restart** na notificação, na linha da conta ou no painel de detalhes.
3. Se o aplicativo reportar um processo órfão (**Orphan process**) no centro de notificações, escolha **Adopt** ou **Kill**.

**Sinal de sucesso.** As contas estão novamente no status **Running**, as marcas vermelhas de queda desapareceram e não há um indicador **Recovering** ativo na barra de status.

### Dicas

- Não reinicie tudo manualmente logo após uma queda — primeiro dê alguns segundos à recuperação automática.
- Se as quedas se repetirem, abra o **Monitoring** para ver a carga: talvez você esteja rodando mais contas do que este computador aguenta.

![o indicador Recovering na barra de status](../images/status-recovering.png)

---

# 6. Tarefas comuns («Quero…»)

Respostas curtas para objetivos comuns. Para instruções completas, siga os links para a seção 5.

## «Quero adicionar novas contas»

- **Quando você precisa.** Você tem novas contas Steam.
- **O que fazer.** Para uma conta, use o botão **Add Account** na tela **Accounts**. Para muitas de uma vez, use o botão **Import** e o assistente de importação.
- **O que acontece.** As contas aparecem na tabela e ficam prontas para iniciar (assim que tiverem uma sandbox).
- Mais: [5.1](#51-adicionar-uma-única-conta), [5.2](#52-importar-uma-lista-de-contas-de-um-arquivo).

## «Quero iniciar o Steam»

- **Quando você precisa.** Você precisa que uma conta entre no Steam.
- **O que fazer.** Selecione a conta na tela **Accounts** e clique em **Start**.
- **O que acontece.** O aplicativo inicia o Steam na sandbox da conta e faz login. O status vai de **Starting → Running**.

## «Quero iniciar o CS2»

- **Quando você precisa.** O Steam já está em execução e você precisa iniciar o jogo.
- **O que fazer.** Iniciar a conta com **Start** a leva por todo o cenário, incluindo iniciar o CS2 (se o workflow atribuído incluir isso).
- **O que acontece.** Após entrar no Steam, o aplicativo inicia o CS2. Você pode acompanhar os passos na tela **Workflows**.

## «Quero criar um lobby»

- **Quando você precisa.** Você precisa reunir contas em um lobby de jogo.
- **O que fazer.** Forme um grupo na tela **Matchmaking** com **Create Party** e adicione membros.
- **O que acontece.** O aplicativo combina as contas selecionadas em um grupo e ajuda a levá-las a um estado consistente (quórum).
- Mais: [5.5](#55-criar-um-grupo-e-colocá-lo-na-fila).

## «Quero iniciar o matchmaking»

- **Quando você precisa.** O grupo está formado e pronto.
- **O que fazer.** Selecione o grupo e clique em **Queue** (ou **Queue All** para todos).
- **O que acontece.** Os membros entram na fila; você vê suas posições e o tempo de espera.

## «Quero parar todas as sessões em execução»

- **Quando você precisa.** É hora de encerrar.
- **O que fazer.** Selecione as contas (`Ctrl+A`) e clique em **Stop**.
- **O que acontece.** O aplicativo fecha os clientes de forma ordenada, e os status passam a **Stopped**.
- Mais: [5.4](#54-parar-todas-as-contas-em-execução).

## «Quero recuperar após uma queda»

- **Quando você precisa.** Um cliente caiu ou o aplicativo foi reiniciado.
- **O que fazer.** Dê alguns segundos à recuperação automática; se necessário, clique em **Restart** para a conta que caiu.
- **O que acontece.** O aplicativo devolve as contas ao trabalho.
- Mais: [5.7](#57-recuperar-após-uma-queda-ou-reinício-do-aplicativo).

## «Quero organizar as janelas na tela»

- **Quando você precisa.** Você quer dispor as janelas do CS2 de forma organizada no seu monitor.
- **O que fazer.** Na tela **Layouts**, crie uma predefinição e clique em **Apply** / **Snap windows**.
- **O que acontece.** As janelas em execução se movem para os lugares definidos.

---

# 7. Referência de funcionalidades

Esta seção cobre funcionalidades individuais com seu propósito, localização e particularidades.

## 7.1. Busca e filtros de contas

**Propósito.** Encontrar rapidamente as contas que você precisa em uma lista grande.

**Localização.** A barra de ferramentas da tela **Accounts**: o campo de busca e o botão **Filters**.

**Como usar.**
- Digite no campo de busca (`Ctrl+F`). Você pode buscar por partes: `login:alex`, `status:running`, `rank:>=gold`, `tag:prime`.
- Clique em **Filters** (`Ctrl+K` nesta tela abre a janela de filtros), defina condições por status, rank, sandbox, workflow ou tags, e salve o conjunto como uma predefinição.

**Comportamento esperado.** A tabela mostra imediatamente apenas as contas correspondentes. Os filtros ativos aparecem como uma linha de chips abaixo da barra de ferramentas.

**Dica.** Salve conjuntos de condições usados com frequência como predefinições — eles ficam disponíveis no menu suspenso da barra de ferramentas.

## 7.2. Agrupamento e configuração de colunas

**Propósito.** Organizar a tabela conforme sua tarefa.

**Localização.** A barra de ferramentas da tela **Accounts**: os botões **Density**, **Columns** e **Group**.

**Como usar.**
- **Group** permite agrupar as contas por status, workflow, sandbox, tag ou rank. Os grupos mostram contadores, por exemplo `Running (24)`.
- **Columns** — o conjunto de colunas visíveis. Há conjuntos prontos: **Operational**, **Identity**, **Audit**, **Compact**. Você pode salvar o seu.
- **Density** — a altura das linhas (mais compacta ou mais espaçosa).

## 7.3. Menu de contexto da conta

**Propósito.** Acesso rápido a todas as ações de uma conta.

**Localização.** Clique com o botão direito em uma linha de conta.

**O que está disponível.** Editar, copiar o login ou o Steam ID, iniciar/parar/reiniciar, vincular e desvincular uma sandbox, atribuir um workflow, reautenticar (**Re-auth**), testar o login (**Probe login now**), trabalhar com tags, exportar, clonar e excluir.

## 7.4. Operações em massa

**Propósito.** Executar uma ação em muitas contas de uma vez.

**Localização.** A barra de ferramentas da tela **Accounts** no modo de seleção (quando pelo menos uma linha está marcada).

**Como usar.** Marque as contas e clique no botão desejado: **Start**, **Stop**, **Restart**, **Bind sandbox**, **Workflow…**, **Tag…**, **Export** ou **Delete**.

**Comportamento esperado.** Aparece uma janela com o progresso de cada conta. Você pode cancelar a operação enquanto ela é executada.

**Limitação.** Ao excluir cinco ou mais contas, o aplicativo pede para confirmar digitando a palavra `DELETE`.

## 7.5. Exportar contas

**Propósito.** Salvar os dados das contas em um arquivo.

**Localização.** O botão **Export** na barra de ferramentas ou no menu de contexto.

**Como usar.** Escolha um formato: **TXT** (login:senha), **CSV** (todos os campos) ou **JSON** (o registro completo).

> **Aviso.** Exportar senhas requer consentimento separado — o aplicativo pede que você marque uma caixa. Trate esses arquivos com cuidado.

## 7.6. Clonar uma conta

**Propósito.** Criar rapidamente uma cópia de uma conta como ponto de partida.

**Localização.** Menu de contexto da linha → **Clone…**.

**Comportamento esperado.** Abre um formulário com os campos já preenchidos (o login vira `original_copy`), exceto o código do Steam Guard e o vínculo de sandbox — esses você define de novo.

## 7.7. Workflows: iniciar, pausar, parar

**Propósito.** Gerenciar cenários automatizados.

**Localização.** A tela **Workflows**.

**Como usar.**

| Ação | O que faz | Pede confirmação? |
|---|---|---|
| **Start** | Executa o cenário para as contas selecionadas | Ao iniciar mais de 10 contas |
| **Pause** | Pausa suavemente após o passo atual | Não |
| **Resume** | Continua do ponto atual | Não |
| **Stop** | Encerra o cenário com limpeza | Sim |
| **Restart** | Para e recomeça | Sim (em operação em massa) |
| **Skip step** | Marca o passo atual como concluído e avança | Sim |
| **Retry now** | Repete o passo atual imediatamente | Não |

**Dica.** A aba **State Machine** no painel de detalhes mostra claramente em que passo um cenário está.

## 7.8. Vincular a uma sandbox

**Propósito.** Reservar um ambiente isolado para uma conta, sem o qual ela não pode ser iniciada.

**Localização.** Menu de contexto → **Bind sandbox…**, ou a operação em massa **Bind sandbox**.

**Como usar.** Escolha um método: em ciclo (round-robin), preencher as vazias primeiro ou uma sandbox específica.

**Limitação.** Uma conta, uma sandbox. Se a sandbox escolhida já estiver em uso, o aplicativo oferece liberá-la da conta anterior.

## 7.9. Layouts de janelas

**Propósito.** Organizar as janelas do CS2 usando um layout predefinido.

**Localização.** A tela **Layouts**.

**Como usar.** Crie uma predefinição, posicione os slots na tela dos monitores, defina as atribuições e clique em **Apply**.

**Dica.** O botão **Revert layout** restaura as posições anteriores das janelas dentro de um minuto, caso um layout não dê certo.

## 7.10. Centro de notificações

**Propósito.** Um único lugar para todas as notificações do aplicativo.

**Localização.** O indicador de notificações na barra superior, ou `Ctrl+Shift+N`.

**Como usar.** O painel abre à direita. Alterne entre as abas **All**, **Errors**, **Warnings** e **Info**. Em cada entrada, você pode ir até a origem, repetir ou descartar. O botão **Clear all** esvazia a lista.

**Limitação.** São mantidas as últimas 200 entradas; as mais antigas são removidas.

---

# 8. Status e indicadores

Cada status tem uma cor, um símbolo e um rótulo. Abaixo está o que cada um significa e se você precisa agir.

| Status | Símbolo | O que significa | Requer ação? |
|---|---|---|---|
| **OK / Success** | ✓ (verde) | Conta online, login bem-sucedido | Não |
| **Running** | ▶ (azul) | A conta ou o workflow está em execução | Não |
| **Starting** | ◐ (violeta) | Inicialização em andamento, um estado de transição | Aguarde terminar |
| **Queued** | ⏱ (cinza) | Aguardando na fila | Não |
| **Stopped** | ■ (cinza) | Parada, ociosa | Opcional — você pode iniciá-la |
| **Paused** | ⏸ (âmbar) | Cenário pausado | Clique em **Resume** para continuar |
| **Warning** | △ (âmbar) | Uma anomalia não crítica | Veja os detalhes; muitas vezes dá para continuar |
| **Error** | ✕ (vermelho) | Uma falha recuperável | Clique em **Retry** ou investigue a causa |
| **Crashed** | ☠ (vermelho-escuro, pulsando) | O processo encerrou inesperadamente | Clique em **Restart** |
| **Match Found** | ◎ (verde, pulsando) | Uma partida de CS2 foi encontrada | Nada — o aplicativo confirma a prontidão automaticamente |
| **Desync** | ⛓ (laranja) | Os membros do grupo estão dessincronizados | Execute **Re-sync** |
| **Info** | ⓘ (azul) | Uma mensagem neutra | Não |

**Indicadores adicionais:**

- **Recovering** — um indicador azul na barra de status durante a inicialização do aplicativo: os processos da sessão anterior estão sendo retomados sob gerenciamento. Aguarde terminar.
- **Reattached** — uma marca temporária em uma linha de conta: o processo foi retomado com sucesso após um reinício.
- **Frozen at HH:mm:ss** — na tela **Monitoring**, significa que a exibição dos dados está congelada (fora do modo **Live**). Para trazer de volta os dados ao vivo, mude para **Live** ou desative **Freeze**.

**Como ver os detalhes.** Passe o cursor sobre um símbolo de status para obter uma dica: desde quando o estado dura, em que passo a conta está e qual foi o último evento.

![exemplos de status na tabela de contas](../images/status-badges.png)

---

# 9. Notificações

O aplicativo informa os eventos de três formas: **toasts** (aparecem no canto e somem), a **barra de status** (um resumo permanente na parte inferior) e **faixas internas** (ligadas a uma tela específica).

## Toasts

Aparecem no canto inferior direito.

| Notificação | Por que aparece | O que significa | O que fazer | Pode ser ignorada |
|---|---|---|---|---|
| **Saved** | Você alterou um ajuste | A alteração foi salva | Nada | Sim, some sozinha |
| Sucesso de operação (verde) | Uma ação foi concluída com sucesso | Está tudo bem | Nada | Sim, some após ~5 segundos |
| Aviso (âmbar) | Uma anomalia não crítica foi detectada | Vale uma olhada | Opcionalmente, ver os detalhes | Geralmente sim, some após ~10 segundos |
| Erro (vermelho) | Uma operação falhou | É necessária uma ação | Clique em **View** ou **Retry** | Não, permanece até ser descartada |
| Queda (Crash) | Um cliente fechou inesperadamente | Uma conta caiu | Clique em **Restart** ou abra o dump | Não, permanece até ser reconhecida |

**Bom saber.**
- Passar o cursor sobre uma notificação para o cronômetro de dispensa automática — você pode lê-la com calma.
- Notificações idênticas se agrupam em uma só com um contador, por exemplo `… failed (×4)`.

## Barra de status

No lado direito da barra de status, é exibida a notificação não lida mais importante, por exemplo `● 3 errors`. Ao clicar, abre o centro de notificações.

## Faixas internas (Banners)

Aparecem no topo de uma tela e se aplicam a ela como um todo. Exemplo: `⚠ Steam network degraded — 12 accounts retrying login`. Uma faixa pode ser fechada com o botão **Dismiss** se não for bloqueante. Faixas bloqueantes (por exemplo, quando um serviço está indisponível) permanecem até o problema ser resolvido.

## Alertas sonoros

O som fica desligado por padrão. Você pode ativá-lo para eventos específicos (por exemplo, **Match found** ou **Crash**) em **Settings → Notifications**. Um som para **Match found** é útil para saber que uma partida foi encontrada sem olhar para a tela — a aceitação da partida em si acontece automaticamente.

![um toast de erro com os botões View e Retry](../images/notification-error-toast.png)

---

# 10. Erros e solução de problemas

Erros ao operar um farm são rotina, e o aplicativo ajuda você a resolvê-los. Abaixo estão situações comuns no formato “Problema → Causa possível → Solução → Resultado esperado”.

## Não é possível ativar a licença

**Problema.** Ao inserir a chave, o aplicativo não deixa você prosseguir.

| Mensagem | Causa possível | Solução |
|---|---|---|
| “License key invalid” | A chave foi inserida com um erro de digitação | Verifique a grafia. É mais fácil colar a chave com **Paste from clipboard** |
| “Used on max devices” | A licença já está em uso no número máximo de dispositivos | Libere a licença em outro dispositivo e tente de novo. O botão **Manage devices** leva ao gerenciamento de dispositivos |
| “Cannot reach license server” | Sem conexão com o servidor de licenças | Verifique sua conexão com a internet e clique em **Retry** |

**Resultado esperado.** Com uma chave correta e conexão com o servidor, a janela de ativação se fecha e o **Dashboard** abre.

## Uma conta não inicia

**Problema.** Você clicou em **Start**, mas a conta não passa para **Running**.

- **Causa possível.** A conta não está vinculada a uma sandbox.
  **Solução.** Abra o menu de contexto da conta → **Bind sandbox…** e atribua uma sandbox.
- **Causa possível.** É necessária reautenticação (dados de login desatualizados); há uma marca “Reauth required” ao lado da linha.
  **Solução.** Menu de contexto → **Re-auth (Steam Guard)**.
- **Causa possível.** O Steam limitou temporariamente a frequência de logins.
  **Solução.** Aguarde cerca de um minuto e clique em **Retry**.

**Resultado esperado.** O status vai de **Starting → Running**.

## O Steam fica muito tempo em Waiting/Starting

**Problema.** A conta está presa na etapa de login.

- **Causa possível.** Um login lento ou problemas temporários da rede do Steam.
  **Solução.** Dê um tempo. Se aparecer um status **Error**, clique em **Retry**. Se a rede do Steam estiver instável, uma faixa de aviso aparece no topo — aguarde a recuperação.

**Resultado esperado.** A conta faz login e passa para **Running**.

## Um cliente caiu

**Problema.** A conta recebeu o status **Crashed**.

- **Causa possível.** O cliente do CS2 ou do Steam encerrou inesperadamente.
  **Solução.** Na notificação que aparece, clique em **Restart**. A recuperação muitas vezes já está em andamento automaticamente. Os detalhes da queda estão na tela **Monitoring**, no feed **Crashes & Warnings**.

**Resultado esperado.** A conta reinicia e volta para **Running**.

## Um grupo entrou em Desync

**Problema.** O grupo está no estado **Desync** — os membros estão em um estado inconsistente.

- **Causa possível.** Um membro aceitou uma partida e outro não a tempo, ou alguém saiu da fila.
  **Solução.** Clique em **Re-sync** para pausar a fila e aguardar a consistência. Se uma conta está causando problema, remova-a com **Drop member** e coloque as demais na fila de novo.

**Resultado esperado.** O grupo volta ao estado **Quorum** e está pronto para a fila de novo.

## Uma inicialização em massa terminou com erros

**Problema.** Após um **Start** em massa, algumas contas não iniciaram.

- **Solução.** No resumo, clique em **Filter to failed** — a tabela mostra apenas as contas problemáticas. Resolva cada uma pelas causas acima e inicie de novo.

**Resultado esperado.** Depois de resolvidas as causas, um **Start** repetido leva as contas para **Running**.

## Os dados de uma tela não carregam

**Problema.** Em vez do conteúdo da tela, há uma faixa ou uma mensagem de que um serviço está indisponível.

- **Causa possível.** Um serviço em segundo plano está temporariamente indisponível.
  **Solução.** Clique em **Retry**. Se não ajudar, clique em **Open logs** para ver os detalhes, ou reinicie o aplicativo.

**Resultado esperado.** A tela carrega e mostra dados atuais.

## O aplicativo reporta um processo órfão

**Problema.** No centro de notificações, uma mensagem como “Orphan process … — Adopt or Kill?”.

- **Causa possível.** Sobrou um processo da sessão anterior que não pôde ser vinculado automaticamente a uma conta.
  **Solução.** Escolha **Adopt** (colocar sob gerenciamento) se o processo é necessário, ou **Kill** (encerrar) se não.

**Resultado esperado.** A lista de processos fica em ordem.

## O computador está lento e as quedas estão aumentando

**Problema.** Instabilidade geral, falhas frequentes.

- **Causa possível.** Há mais contas em execução do que o computador aguenta.
  **Solução.** Abra o **Monitoring** e olhe **CPU** e **RAM**. Se os valores estiverem perto dos limites, pare algumas contas com **Stop**.

**Resultado esperado.** A carga cai e a operação se estabiliza.

> **Códigos de erro.** Os detalhes dos erros incluem um código curto como `[E-1042]`. Você pode copiá-lo e usá-lo ao contatar o suporte. Uma referência completa dos códigos está disponível em **Help → Error reference**.

![um exemplo de tela de erro com os botões Retry / Open logs](../images/error-screen.png)

---

# 11. Boas práticas

## Preparar contas

- Adicione as contas como lista via **Import** — é mais rápido e há menos erros de digitação.
- Deixe a atribuição de sandbox em **Auto-assign**, a menos que precise de um vínculo específico.
- Use **Tags** para agrupar contas e filtrá-las rapidamente.

## Iniciar muitas contas

- Inicie em lotes: comece com um grupo pequeno, confirme a estabilidade e depois adicione mais.
- Mantenha o **Dashboard** ou o **Monitoring** aberto para acompanhar a carga em tempo real.
- Mire nas 4–10 contas de CS2 recomendadas por vez; você pode rodar mais em um PC potente e menos em máquinas mais fracas.

## Trabalhar com layouts

- Prepare várias predefinições de antemão para diferentes situações (por exemplo, “4-stack”, “um em foco”).
- Se um layout der errado, use **Revert layout** de imediato, enquanto a janela de reversão de um minuto está ativa.

## Parar com segurança

- Pare as contas com o botão **Stop** (um encerramento ordenado) em vez de fechar as janelas manualmente.
- Antes de sair do aplicativo, pare as contas ativas. Se você tentar fechar o aplicativo com cenários em execução, ele avisa.

## Evitar interrupções

- Antes de colocar na fila, confirme que o grupo está no estado **Quorum**.
- Fique de olho nas faixas sobre o estado da rede do Steam — quando estiver instável, é melhor esperar.

## Manter uma operação estável

- Verifique o **Dashboard** regularmente — ele mostra o estado geral em segundos.
- Mantenha o número de contas em execução simultânea dentro da capacidade do seu computador.
- Deixe a recuperação automática trabalhar por alguns segundos antes de intervir manualmente.

---

# 12. Perguntas frequentes

**Por que não consigo iniciar uma conta?**
O mais provável é que a conta não esteja vinculada a uma sandbox — sem uma, não é possível iniciar. Vincule uma pelo menu de contexto → **Bind sandbox…**. Um início também pode ser bloqueado pela necessidade de reautenticar (uma marca “Reauth required”) — nesse caso, execute **Re-auth**.

**Por que o Steam fica muito tempo em estado de espera?**
Isso normalmente é um login lento ou atrasos temporários da rede do Steam. Dê um tempo. Se aparecer um status **Error**, clique em **Retry**.

**Como reinicio um workflow?**
Selecione as contas ou instâncias desejadas e clique em **Restart** (ou `Ctrl+Shift+R`). Em uma operação em massa, o aplicativo pede confirmação.

**O que acontece se o aplicativo fechar?**
Suas contas e ajustes ficam salvos. Na próxima execução, o aplicativo tenta retomar os processos da sessão anterior sob gerenciamento — um indicador **Recovering** aparece na barra de status. Se havia cenários ativos ao fechar, o aplicativo avisa com antecedência.

**Como sei que está tudo funcionando?**
Verifique a barra de status na parte inferior e o **Dashboard**. Sinais de operação normal: contas no status **Running**, sem marcas vermelhas no cartão **Errors** ou na tabela **Failures & Crashes**, e carga de **CPU** e **RAM** dentro de faixas normais.

**Onde ficam guardadas as minhas senhas?**
Apenas no seu computador. São criptografadas com a proteção nativa do Windows, nunca são salvas em texto puro e nunca são enviadas a lugar nenhum.

**O FarmPanel joga por mim?**
Não. Não é um bot nem um autofarm. O aplicativo gerencia a inicialização, o monitoramento, a montagem de lobbies e a recuperação, enquanto todas as ações dentro do jogo são feitas por você.

**Preciso digitar a chave de licença toda vez?**
Não. A chave é digitada uma única vez, na primeira ativação. Depois disso, o aplicativo abre direto no **Dashboard**.

**Como encontro rapidamente uma ação se esqueci onde fica o botão?**
Pressione `Ctrl+K` para abrir a paleta de comandos. Comece a digitar o nome de uma ação, tela ou login de conta e escolha o item desejado na lista.

**Posso mover o monitoramento para um segundo monitor?**
Sim. Na tela **Monitoring**, clique no botão de desacoplar — a tela abre como uma janela separada que você pode colocar em um segundo monitor. A posição dela é memorizada.

**Como restauro os ajustes para os padrões?**
Em **Settings → Advanced** há **Reset to defaults**. Para proteger contra cliques acidentais, o aplicativo pede que você confirme digitando um texto.

---

*Fim do guia do usuário do FarmPanel.*
