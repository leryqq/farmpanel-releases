# Instalação do Sandboxie-Plus

**Guia de instalação passo a passo para Windows**

Versão do documento: 1.0 · Versão do Sandboxie-Plus: **1.17.5**

🌐 [English](INSTALL-SANDBOXIE-PLUS.md) · [Русский](INSTALL-SANDBOXIE-PLUS.ru.md) · [Español](INSTALL-SANDBOXIE-PLUS.es.md) · **Português** · [Français](INSTALL-SANDBOXIE-PLUS.fr.md) · [Türkçe](INSTALL-SANDBOXIE-PLUS.tr.md) · [Bahasa Indonesia](INSTALL-SANDBOXIE-PLUS.id.md) · [Tiếng Việt](INSTALL-SANDBOXIE-PLUS.vi.md) · [हिन्दी](INSTALL-SANDBOXIE-PLUS.hi.md) · [中文](INSTALL-SANDBOXIE-PLUS.zh.md) · [العربية](INSTALL-SANDBOXIE-PLUS.ar.md)

---

O FarmPanel mantém cada conta em sua própria **sandbox** — um ambiente isolado onde o Steam e o CS2 não se sobrepõem a outras contas. Esse isolamento é feito por um programa gratuito chamado **Sandboxie-Plus**. Você o instala uma vez, antes de começar a iniciar contas no FarmPanel.

Este guia acompanha você pela instalação passo a passo. Nada complicado — leva alguns minutos.

> **Em resumo.** Baixe o instalador do **Sandboxie-Plus 1.17.5** → execute-o → aceite as configurações padrão → permita a instalação (são necessários direitos de administrador) → pronto.

> **Importante.** Ao contrário do próprio FarmPanel, o Sandboxie-Plus **exige direitos de administrador** para ser instalado — isso é normal, porque o programa se integra profundamente ao Windows para isolar os aplicativos de forma confiável.

## Conteúdo

1. [O que você vai precisar](#1-o-que-você-vai-precisar)
2. [Passo 1. Baixe o instalador](#passo-1-baixe-o-instalador)
3. [Passo 2. Execute a instalação](#passo-2-execute-a-instalação)
4. [Passo 3. Percorra o assistente de instalação](#passo-3-percorra-o-assistente-de-instalação)
5. [Passo 4. Primeira execução do Sandboxie-Plus](#passo-4-primeira-execução-do-sandboxie-plus)
6. [Passo 5. Verifique se está tudo funcionando](#passo-5-verifique-se-está-tudo-funcionando)
7. [Passo 6. Conecte-o ao FarmPanel](#passo-6-conecte-o-ao-farmpanel)
8. [Como desinstalar o Sandboxie-Plus](#como-desinstalar-o-sandboxie-plus)
9. [Solução de problemas](#solução-de-problemas)
10. [Perguntas frequentes](#perguntas-frequentes)

---

# 1. O que você vai precisar

- **Um computador com Windows 10 ou 11** (64 bits).
- **Direitos de administrador** neste computador (um aviso aparece durante a instalação — você precisa clicar em **Sim**).
- **Uma conexão com a internet** — para baixar o programa.
- **Cerca de 5 minutos do seu tempo.**

> O Sandboxie-Plus é gratuito. Alguns recursos extras estão disponíveis para quem apoia o projeto, mas você **não precisa** deles para trabalhar com o FarmPanel — a versão gratuita comum é suficiente.

---

# Passo 1. Baixe o instalador

1. Abra a página oficial da versão que você precisa:
   **[Sandboxie-Plus 1.17.5 no GitHub](https://github.com/sandboxie-plus/Sandboxie/releases/tag/v1.17.5)**
2. Role para baixo até a seção **Assets**.
3. Encontre e baixe o arquivo com um nome parecido com **`Sandboxie-Plus-x64-v1.17.5.exe`** — este é o instalador para um Windows comum de 64 bits.

**Como escolher o arquivo certo:**

| Arquivo | Para quem é |
|---|---|
| **`Sandboxie-Plus-x64-v1.17.5.exe`** | **A maioria dos usuários** — um Windows comum em processador Intel ou AMD. Baixe este. |
| `Sandboxie-Plus-arm64-v1.17.5.exe` | Apenas para computadores com processador ARM (raro). |
| `Sandboxie-Classic-…` | A variante de interface antiga. **Não é necessária** para o FarmPanel — escolha o **Plus**. |
| Arquivos `.7z` | Versões portáteis para usuários avançados. **Não são necessárias** para a instalação. |

**O que acontece em seguida.** O arquivo aparece na sua pasta **Downloads**.

> **Dica.** Baixe o instalador apenas da página oficial do GitHub indicada acima. Assim você obtém a versão autêntica e verificada.

![a página de release 1.17.5 com a seção Assets](../images/sandboxie/github-release-assets.png)

---

# Passo 2. Execute a instalação

1. Abra a pasta **Downloads** e dê um clique duplo no arquivo baixado **`Sandboxie-Plus-x64-v1.17.5.exe`**.
2. O Windows mostra o aviso **“Deseja permitir que este aplicativo faça alterações no seu dispositivo?”** — clique em **Sim**. Esse é o aviso de direitos de administrador; sem ele, o Sandboxie-Plus não pode ser instalado.

> **Se aparecer uma janela azul do SmartScreen** (“O Windows protegeu o seu PC”) — clique em **Mais informações** e depois em **Executar assim mesmo**. Esse é um aviso comum para programas baixados, não um erro.

**O que acontece em seguida.** A janela do assistente de instalação abre.

---

# Passo 3. Percorra o assistente de instalação

O assistente de instalação conduz você por algumas telas simples. Na maioria dos casos, basta deixar tudo nos valores padrão e clicar em **Next**.

1. **Seleção de idioma.** Se aparecer uma janela de seleção de idioma, escolha português (ou seu idioma) e clique em **OK**.
2. **Acordo de licença.** Leia-o e clique em **I Agree** ou **Next**.
3. **Pasta de instalação.** Deixe a pasta padrão (`C:\Program Files\Sandboxie-Plus`) e clique em **Next**. Não há necessidade de mudá-la.
4. **Opções de instalação.** Nada precisa ser alterado — apenas clique em **Next** / **Install**.
5. Aguarde terminar. A instalação leva menos de um minuto.
6. Na última tela, clique em **Finish**. Deixe a caixa “iniciar o Sandboxie-Plus” marcada, se houver.

**O que acontece em seguida.** O Sandboxie-Plus é instalado e o ícone dele aparece na sua área de trabalho e no menu Iniciar. O programa geralmente inicia logo após a instalação.

> **É preciso reiniciar?** Normalmente não. Mas se o assistente pedir para reiniciar o computador, faça isso, para que o isolamento funcione corretamente.

![a tela do assistente de instalação com a pasta padrão](../images/sandboxie/installer-wizard.png)

---

# Passo 4. Primeira execução do Sandboxie-Plus

Na primeira vez que você abre o Sandboxie-Plus, ele mostra um **Setup Wizard** (assistente de configuração). Percorra-o passo a passo — apenas repita o que está descrito abaixo.

Se uma janela de **seleção de idioma da interface** aparecer antes do assistente, escolha seu idioma e clique em **OK**.

Em seguida, o assistente conduz você por várias telas.

### Tela 1 — Introduction

Selecione **“Personally, for private non-commercial use”** (Para uso pessoal, não comercial) e clique em **Next**.

![Setup Wizard — a tela Introduction com “Personally, for private non-commercial use” selecionado](../images/sandboxie/wizard-1-introduction.png)

### Tela 2 — Support certificate

Deixe o campo **vazio** e clique em **Next**. Um certificado não é necessário para trabalhar com o FarmPanel.

![Setup Wizard — a tela Support certificate com o campo vazio](../images/sandboxie/wizard-2-support-certificate.png)

### Tela 3 — Configure UI

Deixe os valores nos **padrões** (**Advanced UI for experts** já está selecionado) e clique em **Next**.

![Setup Wizard — a tela de configuração da interface com os valores padrão](../images/sandboxie/wizard-3-ui-configuration.png)

### Tela 4 — Shell integration

**Desmarque todas as caixas** e clique em **Next**.

![Setup Wizard — a tela Shell integration com todas as caixas desmarcadas](../images/sandboxie/wizard-4-shell-integration.png)

### Tela 5 — Updater

**Desmarque todas as caixas** e clique em **Next**.

![Setup Wizard — a tela Updater com todas as caixas desmarcadas](../images/sandboxie/wizard-5-updater.png)

### Tela 6 — Complete

Clique em **Finish** para aplicar as configurações e fechar o assistente.

![Setup Wizard — a tela final com o botão Finish](../images/sandboxie/wizard-6-complete.png)

> **Dica.** Se estiver em dúvida em alguma tela, desmarque as caixas e clique em **Next**. O FarmPanel não precisa das integrações extras nem dos lembretes de atualização.

**O que acontece em seguida.** A janela principal do Sandboxie-Plus abre — a lista de sandboxes e o painel de controle.

![a janela principal do Sandboxie-Plus após a primeira execução](../images/sandboxie/main-window.png)

---

# Passo 5. Verifique se está tudo funcionando

Confirme que o Sandboxie-Plus foi instalado corretamente:

1. Abra o Sandboxie-Plus (o ícone na área de trabalho ou no menu Iniciar).
2. A janela principal mostra uma lista de sandboxes — normalmente há uma sandbox padrão com um nome parecido com **DefaultBox**.
3. O programa abre e não mostra mensagens de erro.

Se tudo isso estiver presente — **o Sandboxie-Plus está instalado e pronto para uso**.

---

# Passo 6. Conecte-o ao FarmPanel

Uma vez que o Sandboxie-Plus está instalado, o FarmPanel pode usá-lo para isolar as contas.

1. Abra o **FarmPanel**.
2. Vá para **Settings → Sandboxes**.
3. Confirme que o caminho da pasta das sandboxes está definido. Se o campo estiver vazio, escolha uma pasta para as sandboxes; se já estiver preenchido, não há nada a mudar.
4. Volte para a tela **Accounts**. Agora, ao adicionar contas, você pode escolher como as sandboxes são atribuídas (**Auto-assign** e outras), e as contas podem ser iniciadas.

> **Como isso se conecta.** No FarmPanel, cada conta precisa estar vinculada a uma sandbox, senão não pode ser iniciada. É o Sandboxie-Plus que cria e mantém esses ambientes isolados “por baixo dos panos”. Para saber mais sobre sandboxes e a inicialização de contas, veja o [Guia do usuário do FarmPanel](../user-guide/USER-GUIDE.pt.md).

**Sinal de sucesso.** Uma conta no FarmPanel inicia e passa para o status **Running** — o que significa que o isolamento pelo Sandboxie-Plus está funcionando.

---

# Como desinstalar o Sandboxie-Plus

Se precisar remover o programa:

1. Primeiro, feche todos os programas em execução nas sandboxes (no FarmPanel, pare as contas com **Stop**).
2. Abra **Configurações do Windows** → **Aplicativos** → **Aplicativos instalados**
   (ou “Painel de Controle” → “Programas e Recursos”).
3. Encontre **Sandboxie-Plus** na lista.
4. Clique em **Desinstalar** e confirme. Direitos de administrador também são necessários para desinstalar.

> **Observação.** Depois que o Sandboxie-Plus é removido, o FarmPanel não consegue iniciar contas até o programa ser instalado de novo.

---

# Solução de problemas

## O Windows não deixa instalar — sem direitos de administrador

**Causa.** O Sandboxie-Plus exige estritamente direitos de administrador.

**Solução.** Entre com uma conta que tenha direitos de administrador, ou peça ao administrador do computador para instalar o programa. Quando aparecer o aviso **“Deseja permitir alterações?”**, clique em **Sim**.

## Apareceu uma janela do SmartScreen

**Causa.** O Windows avisa sobre programas baixados recentemente. Não é um erro.

**Solução.** Clique em **Mais informações** e depois em **Executar assim mesmo**.

## Um antivírus bloqueou o instalador

**Causa.** Alguns antivírus são cautelosos com softwares que se integram ao sistema.

**Solução.**
1. Confirme que você baixou o arquivo da página oficial do GitHub (o link está no [Passo 1](#passo-1-baixe-o-instalador)).
2. Se necessário, adicione temporariamente o arquivo às exceções do antivírus e baixe-o de novo.

## Baixou o arquivo errado

**Causa.** Há vários arquivos na página de release.

**Solução.** Para um Windows comum, você precisa do arquivo chamado **`Sandboxie-Plus-x64-v1.17.5.exe`**. Não use as variantes **arm64**, **Classic** ou **.7z**. Volte ao [Passo 1](#passo-1-baixe-o-instalador) e baixe o arquivo certo.

## O FarmPanel não inicia contas após a instalação

**Solução.**
1. Confirme que o Sandboxie-Plus está instalado e abre (veja o [Passo 5](#passo-5-verifique-se-está-tudo-funcionando)).
2. No FarmPanel, abra **Settings → Sandboxes** e verifique se o caminho da pasta das sandboxes está definido.
3. Reinicie o FarmPanel.
4. Se o problema persistir, contate o suporte (veja [Perguntas frequentes](#perguntas-frequentes)).

## O computador pede reinício após a instalação

**Solução.** Reinicie o computador — isso conclui a instalação e ativa o isolamento. Após reiniciar, abra o FarmPanel de novo.

---

# Perguntas frequentes

**É obrigatório instalar o Sandboxie-Plus?**
Sim, se você quiser iniciar contas no FarmPanel. É o Sandboxie-Plus que fornece o isolamento de cada conta em um ambiente separado.

**O Sandboxie-Plus é pago?**
Não, a versão básica é gratuita e é suficiente para trabalhar com o FarmPanel. Recursos extras estão disponíveis para quem apoia o projeto, mas não são obrigatórios.

**Por que a instalação exige direitos de administrador e o FarmPanel não?**
O Sandboxie-Plus se integra profundamente ao Windows para isolar os programas de forma confiável, por isso precisa de direitos de administrador. O FarmPanel, por outro lado, é instalado apenas para a sua conta de usuário e não os exige.

**Preciso configurar as sandboxes eu mesmo?**
Não. Basta instalar o Sandboxie-Plus. O FarmPanel cria e configura as sandboxes para as contas automaticamente.

**Preciso de um certificado de apoio (supporter certificate)?**
Não. Você pode pular essa tela na primeira execução. Ele não é necessário para o FarmPanel.

**Qual versão exata devo instalar?**
A versão **1.17.5** — o link está no [Passo 1](#passo-1-baixe-o-instalador). Instale exatamente essa para uma compatibilidade previsível com o FarmPanel.

**Para onde recorrer se algo não funcionou?**
Contate o suporte do FarmPanel no Telegram: [t.me/farmpanel_br](https://t.me/farmpanel_br). Descreva o problema e inclua o texto da mensagem de erro, se você tiver uma.

---

Depois de instalar o Sandboxie-Plus, volte ao [guia de instalação do FarmPanel](../install-guide/INSTALL-GUIDE.pt.md) ou vá direto ao [Guia do usuário](../user-guide/USER-GUIDE.pt.md) para adicionar contas e iniciar seu primeiro farm.

*Fim do guia de instalação do Sandboxie-Plus.*
