# Instalação do FarmPanel

**Guia de instalação passo a passo para Windows**

Versão do documento: 1.0

🌐 [English](INSTALL-GUIDE.md) · [Русский](INSTALL-GUIDE.ru.md) · [Español](INSTALL-GUIDE.es.md) · **Português** · [Français](INSTALL-GUIDE.fr.md) · [Türkçe](INSTALL-GUIDE.tr.md) · [Bahasa Indonesia](INSTALL-GUIDE.id.md) · [Tiếng Việt](INSTALL-GUIDE.vi.md) · [हिन्दी](INSTALL-GUIDE.hi.md) · [中文](INSTALL-GUIDE.zh.md) · [العربية](INSTALL-GUIDE.ar.md)

---

Este guia leva você do download do programa até a primeira execução. Siga os passos na ordem — nada complicado, leva apenas alguns minutos.

> **Em resumo.** Baixe o `Setup.exe` → execute → ative sua licença com a chave → pronto. Não são necessários direitos de administrador, e nada mais precisa ser instalado separadamente.

## Conteúdo

1. [O que você vai precisar](#1-o-que-você-vai-precisar)
2. [Requisitos do sistema](#2-requisitos-do-sistema)
3. [Passo 1. Baixe o instalador](#passo-1-baixe-o-instalador)
4. [Passo 2. Execute a instalação](#passo-2-execute-a-instalação)
5. [Passo 3. Abra o aplicativo](#passo-3-abra-o-aplicativo)
6. [Passo 4. Configuração inicial — locais do Steam e do Sandboxie](#passo-4-configuração-inicial--locais-do-steam-e-do-sandboxie)
7. [Passo 5. Ative sua licença](#passo-5-ative-sua-licença)
8. [Passo 6. Verifique se está tudo funcionando](#passo-6-verifique-se-está-tudo-funcionando)
9. [Atualizações](#atualizações)
10. [Como desinstalar](#como-desinstalar)
11. [Solução de problemas de instalação](#solução-de-problemas-de-instalação)
12. [Perguntas frequentes](#perguntas-frequentes)

---

# 1. O que você vai precisar

- **Um computador com Windows 10 ou 11** (64 bits).
- **Uma conexão com a internet** — para baixar o programa e ativar a licença.
- **Uma chave de licença** — você a recebe com a compra. Ela tem este formato:
  `XXXX-XXXX-XXXX-XXXX-XXXX` (cinco grupos de quatro caracteres).
- **Cerca de 10 minutos do seu tempo.**

> Você **não precisa** instalar mais nada separadamente (como o .NET) — tudo o que é necessário já vem incluído no instalador.

---

# 2. Requisitos do sistema

| Item | Mínimo | Recomendado |
|---|---|---|
| Sistema operacional | Windows 10 ou 11 (64 bits) | Windows 10 / 11 (64 bits) |
| Memória | 8 GB | 32 GB |
| Disco | Qualquer | SSD |
| Espaço livre | cerca de 500 MB | 1 GB ou mais |
| Contas simultâneas | 2 | 4–10 contas de CS2 |
| Resolução de tela | pelo menos 1280 pixels de largura | Full HD (1920×1080) ou superior |

Se o seu computador atende ao mínimo, o aplicativo vai funcionar. Quanto mais potente o computador, mais contas você pode manter em execução ao mesmo tempo.

---

# Passo 1. Baixe o instalador

1. Abra a página de download oficial:
   **[Baixar para Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   (você também encontra o link de download no site [farmpanel.cc](https://farmpanel.cc)).
2. Encontre o arquivo com um nome parecido com **`Setup.exe`** (na seção **Assets**, se você estiver na página de releases) e clique nele para baixar.
3. Aguarde o download terminar. O arquivo tem cerca de 50–80 MB, então em uma conexão rápida leva menos de um minuto.

**O que acontece em seguida.** O arquivo `Setup.exe` aparece na sua pasta **Downloads**.

> **Dica.** Baixe o instalador apenas da página oficial indicada acima. Assim você obtém a versão autêntica e verificada do programa.

![a página de download com o arquivo Setup.exe](../images/install-download-page.png)

---

# Passo 2. Execute a instalação

1. Abra a pasta **Downloads** e dê um clique duplo no arquivo **`Setup.exe`**.
2. A instalação começa automaticamente. **Direitos de administrador não são necessários** — o aplicativo é instalado apenas para a sua conta de usuário.
3. Aguarde terminar. Isso normalmente leva menos de um minuto. Não há botões “Avançar” separados para clicar — o instalador faz tudo sozinho.

**O que acontece em seguida.** O aplicativo é instalado e um ícone do **FarmPanel** aparece na sua área de trabalho e no menu Iniciar. Muitas vezes o aplicativo abre logo após a instalação.

> **Se aparecer uma janela azul “O Windows protegeu o seu PC” (SmartScreen)** — esse é um aviso comum para programas novos, não um erro. O que fazer:
> 1. Clique em **Mais informações**.
> 2. Clique no botão **Executar assim mesmo** que aparece.
>
> A instalação continua normalmente. Mais detalhes em [Solução de problemas de instalação](#solução-de-problemas-de-instalação).

---

# Passo 3. Abra o aplicativo

Se o aplicativo não abriu sozinho, dê um clique duplo no ícone do **FarmPanel** na área de trabalho ou procure-o no menu Iniciar.

**O que você verá.** Na primeira execução, o aplicativo conduz você por uma breve configuração inicial e pela ativação da licença — são os próximos passos.

---

# Passo 4. Configuração inicial — locais do Steam e do Sandboxie

Na primeira execução, o aplicativo pede que você indique onde o **Steam** e o **Sandboxie-Plus** estão localizados no seu computador. Sem esses caminhos, o aplicativo não consegue iniciar e isolar as contas.

> **Importante.** O Sandboxie-Plus já deve estar instalado a esta altura. Se você ainda não o instalou, consulte o guia separado [Instalação do Sandboxie-Plus](../install-sandboxie-plus/INSTALL-SANDBOXIE-PLUS.pt.md).

1. **Local do Steam.** Clique no botão de seleção de pasta (**Browse…** / ícone de pasta) ao lado do campo Steam e selecione a pasta onde o Steam está instalado. Normalmente é `C:\Program Files (x86)\Steam`.
2. **Local do Sandboxie.** Clique no botão de seleção de pasta ao lado do campo Sandboxie e selecione a pasta onde o Sandboxie-Plus está instalado. Normalmente é `C:\Program Files\Sandboxie-Plus`.
3. Confirme a configuração (o botão **Save** / **Continue**).

**O que acontece em seguida.** O aplicativo memoriza esses caminhos e os usa sempre que inicia contas.

**Sinal de sucesso.** Os dois caminhos estão definidos e o aplicativo não mostra avisos de que o Steam ou o Sandboxie não foram encontrados.

> **Dica.** Você pode alterar esses caminhos depois, a qualquer momento, em **Settings** (Configurações).

![configuração inicial — locais do Steam e do Sandboxie](../images/initial-setup-locations.png)

---

# Passo 5. Ative sua licença

A ativação é necessária apenas uma vez — na primeira execução.

1. Digite ou cole sua chave de licença no campo de entrada.
   Para colá-la da área de transferência, clique em **Paste from clipboard** (Colar da área de transferência).
2. O aplicativo verifica o formato da chave enquanto você digita. Quando o formato está correto, o botão de ativação fica disponível.
3. Clique em **Activate** (Ativar).

**O que acontece em seguida.** O aplicativo entra em contato com o servidor e verifica a chave. Isso leva alguns segundos — você verá o estado **Activating** (Ativando).

**Sinal de sucesso.** A janela de ativação se fecha e a tela principal do aplicativo — **Dashboard** — abre. Sua licença está ativa. Você não precisará digitar a chave novamente nas próximas execuções.

> **Se a chave não for aceita** — confira se você a digitou sem erros (é mais fácil colá-la com **Paste from clipboard**) e se você tem internet. As mensagens mais comuns estão em [Solução de problemas de instalação](#solução-de-problemas-de-instalação).

![a janela de ativação da licença](../images/license-activation.png)

---

# Passo 6. Verifique se está tudo funcionando

Após a ativação, você chega à tela principal. Confirme que a instalação foi bem-sucedida:

1. Na parte superior da janela você vê a **barra lateral** com as seções (**Dashboard**, **Accounts**, **Workflows** e outras).
2. Na parte inferior da janela está a **barra de status** — uma faixa fina com um resumo e a versão do aplicativo (por exemplo, `v1.0.1`).
3. O aplicativo abre e alterna entre as seções sem erros.

Se tudo isso estiver presente — **a instalação está concluída e você já pode usar o aplicativo**.

**O que vem a seguir.** Adicione suas contas Steam e inicie seu primeiro farm. Para instruções passo a passo, consulte o [Guia do usuário](../user-guide/USER-GUIDE.pt.md) (a seção “Fluxos de trabalho principais”).

![a tela principal após a instalação](../images/dashboard-overview.png)

---

# Atualizações

O FarmPanel se atualiza **automaticamente** — você não precisa baixar nada manualmente.

- O aplicativo verifica se há novas versões ao iniciar e de tempos em tempos durante o uso.
- Uma nova versão é baixada silenciosamente, em segundo plano, sem interromper seu trabalho.
- A atualização é aplicada na próxima vez que o aplicativo é reiniciado.

**O que você faz.** Nada de especial. Basta fechar e reabrir o aplicativo de vez em quando, e a versão mais recente será instalada. A versão atual está sempre visível na barra de status, na parte inferior, e em **Settings → About** (Configurações → Sobre).

---

# Como desinstalar

Se precisar remover o FarmPanel:

1. Abra **Configurações do Windows** → **Aplicativos** → **Aplicativos instalados**
   (ou “Painel de Controle” → “Programas e Recursos”).
2. Encontre **FarmPanel** na lista.
3. Clique em **Desinstalar** e confirme.

**O que acontece em seguida.** O aplicativo é removido do seu computador. Direitos de administrador não são necessários para desinstalar.

---

# Solução de problemas de instalação

Abaixo estão situações comuns e o que fazer em cada uma.

## Apareceu uma janela “O Windows protegeu o seu PC” (SmartScreen)

**Causa.** O Windows mostra esse aviso para programas baixados recentemente e que o sistema ainda não conhece bem. Isso não significa que haja algo errado com o arquivo.

**Solução.**
1. Clique em **Mais informações**.
2. Clique em **Executar assim mesmo**.

A instalação continua. Se não houver o botão **Mais informações**, verifique se você baixou o arquivo da página oficial e tente novamente.

## Um antivírus bloqueou ou excluiu o arquivo

**Causa.** Alguns antivírus tratam instaladores novos com cautela e podem disparar um alarme falso.

**Solução.**
1. Verifique se você baixou o `Setup.exe` da página oficial (o link está no [Passo 1](#passo-1-baixe-o-instalador)).
2. Se necessário, adicione o arquivo às exceções do antivírus e baixe-o novamente.
3. Em caso de dúvida, entre em contato com o suporte (veja [Perguntas frequentes](#perguntas-frequentes)).

## O navegador não deixa baixar o arquivo

**Causa.** O navegador também pode ser cauteloso ao baixar um `.exe`.

**Solução.** No painel de downloads do navegador, escolha **Manter** (Keep) ao lado do arquivo. Ele então terminará de baixar.

## O instalador não inicia com o clique duplo

**Solução.**
- Verifique se o arquivo foi baixado por completo (cerca de 50–80 MB).
- Clique com o botão direito no arquivo e escolha **Abrir**.
- Baixe o instalador novamente se o arquivo estiver corrompido.

## A chave de licença não é aceita

| Mensagem | O que significa | O que fazer |
|---|---|---|
| “License key invalid” | A chave foi digitada com um erro | Confira a grafia. É mais fácil colar a chave com **Paste from clipboard** |
| “Used on max devices” | A licença já está em uso no número máximo de dispositivos | Libere a licença em outro dispositivo e tente de novo. O botão **Manage devices** leva ao gerenciamento de dispositivos |
| “Cannot reach license server” | Sem conexão com o servidor | Verifique sua conexão com a internet e clique em **Retry** |

## O aplicativo não abre após a instalação

**Solução.**
- Abra-o manualmente: o ícone do **FarmPanel** na área de trabalho ou no menu Iniciar.
- Reinicie o computador e tente novamente.
- Se não ajudar, reinstale o aplicativo: desinstale-o (veja [Como desinstalar](#como-desinstalar)) e instale-o de novo.

---

# Perguntas frequentes

**Preciso de direitos de administrador para instalar?**
Não. O FarmPanel é instalado apenas para a sua conta de usuário e não requer direitos de administrador.

**Preciso instalar o .NET ou outros componentes separadamente?**
Não. Tudo o que é necessário já vem incluído no instalador — basta executar o `Setup.exe`.

**Onde o aplicativo é instalado?**
Na pasta pessoal do seu usuário. Você não precisa escolher uma pasta manualmente — o instalador cuida disso.

**É seguro clicar em “Executar assim mesmo” na janela do SmartScreen?**
Sim, se você baixou o `Setup.exe` da página oficial indicada neste guia. O aviso aparece simplesmente porque o programa é novo para o sistema.

**Onde ficam guardadas as minhas senhas após a instalação?**
Apenas no seu computador. Elas são criptografadas com a proteção nativa do Windows, nunca ficam em texto puro e nunca são enviadas a lugar nenhum.

**Preciso digitar a chave de licença toda vez?**
Não. A chave é digitada uma única vez, na primeira ativação. Depois disso o aplicativo abre direto na tela principal.

**Como atualizo o aplicativo para uma nova versão?**
Não há nada a fazer — o FarmPanel se atualiza automaticamente. Basta reiniciar o aplicativo de vez em quando para que a versão mais recente seja instalada (veja [Atualizações](#atualizações)).

**Para onde recorrer se algo não funcionou?**
Fale com o suporte no Telegram: [t.me/farmpanel_br](https://t.me/farmpanel_br). Descreva o problema e, se tiver, inclua o texto da mensagem de erro.

---

Após a instalação, siga para o [Guia do usuário](../user-guide/USER-GUIDE.pt.md) — ele explica em detalhe como adicionar contas, iniciá-las e trabalhar com o aplicativo.

*Fim do guia de instalação do FarmPanel.*
