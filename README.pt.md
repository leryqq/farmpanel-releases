<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="Aplicativo de desktop FarmPanel, tela de Contas: navegação lateral (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) e uma grade de contas com colunas de status, login, apelido, workflow, sandbox e último acesso"/>

<br/>

# FARMPANEL

**Painel para farm de contas Steam e CS2 — orquestração de multicontas no Windows**

`iniciar · isolar · monitorar · recuperar`

FarmPanel é o painel de desktop para Windows que mantém um **farm de contas
Steam** em escala: inicia, isola em sandboxes, acompanha e reinicia
automaticamente cada **conta de CS2** do seu farm — de cinco contas a várias
centenas — a partir de uma única janela, sem autofarm e sem bots.

[**Baixar para Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Site](https://farmpanel.cc) ·
[Produto](https://farmpanel.cc/pt/product) ·
[Telegram](https://t.me/farmpanel_br)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__br-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_br)

Também disponível em: [English](./README.md) · [Русский](./README.ru.md) · [Español](./README.es.md) · [Français](./README.fr.md) · [Türkçe](./README.tr.md) · [Bahasa Indonesia](./README.id.md) · [Tiếng Việt](./README.vi.md) · [हिन्दी](./README.hi.md) · [中文](./README.zh.md) · [العربية](./README.ar.md)

</div>

---

## O que é o FarmPanel

Se você usa mais de uma conta Steam, já conhece a rotina: uma dúzia de
janelas abertas ao mesmo tempo, um cliente de CS2 que travou e você precisa
perceber e reabrir na mão, e nenhum jeito prático de saber quem ficou preso
no carregamento e quem já está em partida. Quanto mais contas no farm, pior
fica a tarefa.

**O FarmPanel é um painel para farm de contas Steam e CS2 criado justamente
para eliminar essa rotina.** É um aplicativo de desktop para Windows que
inicia, isola e monitora um farm inteiro de multicontas a partir de uma única
janela — uma alternativa real a gerenciar contas Steam na mão ou a se virar
com uma colcha de retalhos de scripts e máquinas virtuais.

O FarmPanel **não é um bot de autofarm**. Ele não joga por você nem simula
ações dentro do jogo — ele gerencia tudo o que acontece *em volta* do jogo:
iniciar clientes, enviar convites de lobby, recuperar sessões que travaram e
dar visibilidade em tempo real de cada conta. Toda ação dentro do jogo
continua nas mãos de uma pessoa real, então seu farm se comporta — e parece —
com jogadores reais, porque é isso que ele é.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Por que os donos de farm escolhem o FarmPanel

**01 — Nada de autofarm, nunca.**
O FarmPanel nunca joga por você. Toda ação no jogo é feita na mão, então as
contas parecem humanas, porque são.

**02 — Configure uma vez.**
Cada início e login segue a mesma sequência determinística. O que funcionou
ontem funciona amanhã, sem surpresas.

**03 — Falhas se resolvem sozinhas.**
Se o Steam ou o CS2 cair, o FarmPanel percebe e o traz de volta em segundos,
sem intervenção.

**04 — Isolamento real em sandbox.**
Cada conta roda em seu próprio ambiente isolado — sem sessões
compartilhadas, sem arquivos compartilhados, sem mistura de impressões
digitais entre contas.

**05 — As senhas nunca saem do seu PC.**
As credenciais são criptografadas com a segurança nativa do Windows e ficam
apenas na sua máquina, nunca são enviadas a lugar nenhum.

**06 — Visibilidade em tempo real de cada conta.**
Um painel em tempo real por conta: status, estado da partida, tempo de
atividade. Sem adivinhar o que o farm está fazendo.

**07 — Roteamento de rede por conta.**
Escolha a melhor região de servidor para cada conta; o FarmPanel configura a
rede para você.

**08 — Cresce junto com o farm.**
Comece com cinco contas e escale para centenas. O mesmo painel, o mesmo
fluxo de trabalho, do começo ao fim.

## Como começar

1. Baixe o instalador — **[Baixar para Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   acima, ou na página de [Releases](https://github.com/leryqq/farmpanel-releases/releases) deste repositório.
2. Execute o `Setup.exe`. O FarmPanel verifica seu sistema e conduz a configuração passo a passo.
3. Adicione suas contas Steam e inicie seu primeiro farm.

```
requisitos:   Windows 10/11 (64 bits) · .NET 8
recomendado:  32 GB de RAM · SSD · 16-32 contas de CS2 simultâneas
atualizações: automáticas, a partir deste repositório
```

## Perguntas frequentes

**O FarmPanel joga o jogo por mim?**
Não — esse é justamente o ponto. Não há bots nem autofarm. O FarmPanel
gerencia as contas: inicia, monitora, monta lobbies e conserta travamentos.
Tudo dentro do jogo é feito por você, então suas contas se comportam como
jogadores reais, porque são.

**Onde ficam guardadas as minhas senhas?**
Apenas na sua máquina. São criptografadas com a segurança nativa do Windows,
nunca ficam em texto puro e nunca são enviadas a lugar nenhum.

**Ele funciona só com CS2?**
Hoje o CS2 tem o suporte mais profundo, incluindo telemetria de partida em
tempo real. Mais jogos estão a caminho.

**Quanto custa?**
O preço depende do tamanho do farm. [Fale conosco no Telegram](https://t.me/farmpanel_br)
e encontramos um plano para a sua configuração — de setups pequenos a
centenas de contas.

Mais respostas no [FAQ do produto](https://farmpanel.cc/pt/product#faq).

## Guias e recursos

- [Como usar várias contas Steam com segurança](https://farmpanel.cc/pt/guides/run-multiple-steam-accounts-safely)
- [Sandbox de contas Steam, explicado](https://farmpanel.cc/pt/guides/steam-account-sandboxing)
- [Quantas contas de CS2 um PC aguenta?](https://farmpanel.cc/pt/guides/how-many-cs2-accounts-per-pc)
- [O drop semanal do CS2, explicado](https://farmpanel.cc/pt/guides/cs2-weekly-drop-explained)
- [Riscos de banimento com multicontas no CS2](https://farmpanel.cc/pt/guides/cs2-multi-account-ban-risks)
- [Você precisa de contas Prime para farmar CS2?](https://farmpanel.cc/pt/guides/prime-accounts-for-cs2-farming)
- [A economia do farm de caixas no CS2](https://farmpanel.cc/pt/guides/cs2-case-farming-economics)
- [Vender drops de CS2 e sacar o dinheiro](https://farmpanel.cc/pt/guides/sell-cs2-drops-steam-market)
- [Farm de CS2: na mão vs. com um painel](https://farmpanel.cc/pt/compare/manual-multi-accounting)

## Links

| | |
| --- | --- |
| Site | [farmpanel.cc](https://farmpanel.cc) |
| Produto | [farmpanel.cc/pt/product](https://farmpanel.cc/pt/product) |
| Changelog | [farmpanel.cc/pt/changelog](https://farmpanel.cc/pt/changelog) |
| Telegram | [t.me/farmpanel_br](https://t.me/farmpanel_br) |

---

<div align="center">

Este repositório distribui apenas binários assinados do FarmPanel.
O código-fonte do aplicativo é proprietário e fechado.

`status do sistema · todos os sistemas operacionais`

**FarmPanel Systems** · Todos os direitos reservados

</div>
