<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="FarmPanel desktop app, Accounts screen: sidebar navigation (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) and an account grid with status, login, nickname, workflow, sandbox and last-login columns"/>

<br/>

# FARMPANEL

**Steam & CS2 account farm panel — multi-account orchestration for Windows**

`launch · isolate · monitor · recover`

FarmPanel is the Windows desktop panel for running a **Steam multi-account
farm** at scale. It launches, sandboxes, watches and auto-restarts every
**CS2 account** in your farm — from five accounts to several hundred — from
one window, with no autofarm and no bots involved.

[**Download for Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Website](https://farmpanel.cc) ·
[Product](https://farmpanel.cc/en/product) ·
[Telegram](https://t.me/farmpanel_en)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__en-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_en)

Also available in: [Русский](./README.ru.md) · [Español](./README.es.md)

</div>

---

## What is FarmPanel

If you run more than one Steam account, you already know the drill: a dozen
windows open at once, a crashed CS2 client you have to notice and relaunch
by hand, no clean way to tell who's stuck loading and who's already in a
match. The more accounts you add to your farm, the worse the chore gets.

**FarmPanel is a Steam and CS2 account farm panel built to remove exactly
that chore.** It's a Windows desktop application that launches, isolates and
watches an entire multi-account farm from a single window — a real
alternative to running Steam multi-account setups by hand, or juggling a
patchwork of scripts and virtual machines.

FarmPanel is **not an autofarm bot**. It does not play the game or simulate
in-game actions for you — it manages everything *around* the game: starting
clients, sending lobby invites, recovering crashed sessions, and giving you
live visibility into every account. Every in-game action stays in the hands
of a real person, so your farm behaves — and looks — like real players,
because it is.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Why farm owners choose FarmPanel

**01 — No autofarm, ever.**
FarmPanel never plays for you. Every in-game action is done by hand, so
accounts look human, because they are.

**02 — Set it up once.**
Every launch and login runs the same deterministic sequence. What worked
yesterday works tomorrow, with no surprises.

**03 — Crashes fix themselves.**
If Steam or CS2 goes down, FarmPanel notices and brings it back within
seconds, unattended.

**04 — True sandbox isolation.**
Every account runs in its own isolated environment — no shared sessions,
no shared files, no cross-account fingerprint mixing.

**05 — Passwords never leave your PC.**
Credentials are encrypted with Windows' built-in security and stored only
on your machine, never sent anywhere.

**06 — Live visibility into every account.**
A real-time dashboard per account: status, match state, uptime. No guessing
what the farm is doing.

**07 — Per-account network routing.**
Pick the best server region for each account; FarmPanel configures the
network for you.

**08 — Grows with your farm.**
Start with five accounts, scale to hundreds. Same panel, same workflow,
the whole way.

## Getting started

1. Download the installer — **[Download for Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   above, or from this repo's [Releases](https://github.com/leryqq/farmpanel-releases/releases) page.
2. Run `Setup.exe`. FarmPanel checks your system and walks you through setup.
3. Add your Steam accounts and launch your first farm.

```
requirements: Windows 10/11 (64-bit) · .NET 8
recommended:  32GB RAM · SSD · 16-32 CS2 accounts concurrent
updates:      automatic, from this repository
```

## FAQ

**Does FarmPanel play the game for me?**
No — that's the whole point. There are no bots and no autofarm. FarmPanel
manages the accounts: launching, watching, assembling lobbies, fixing
crashes. Everything inside the game is done by you, so your accounts behave
like real players, because they are.

**Where are my passwords stored?**
Only on your machine. They're encrypted with Windows' built-in security,
never stored in plain text, and never sent anywhere.

**Does it only support CS2?**
CS2 has the deepest support today, including live match telemetry. More
games are on the way.

**How much does it cost?**
Pricing depends on farm size. [Message us on Telegram](https://t.me/farmpanel_en)
and we'll match a plan to your setup — from small configurations to
hundreds of accounts.

More answers on the [product FAQ](https://farmpanel.cc/en/product#faq).

## Guides & resources

- [How to run multiple Steam accounts safely](https://farmpanel.cc/en/guides/run-multiple-steam-accounts-safely)
- [Steam account sandboxing, explained](https://farmpanel.cc/en/guides/steam-account-sandboxing)
- [How many CS2 accounts can one PC run?](https://farmpanel.cc/en/guides/how-many-cs2-accounts-per-pc)
- [CS2 weekly drop, explained](https://farmpanel.cc/en/guides/cs2-weekly-drop-explained)
- [CS2 multi-account ban risks](https://farmpanel.cc/en/guides/cs2-multi-account-ban-risks)
- [Do you need Prime accounts to farm CS2?](https://farmpanel.cc/en/guides/prime-accounts-for-cs2-farming)
- [CS2 case farming economics](https://farmpanel.cc/en/guides/cs2-case-farming-economics)
- [Selling CS2 drops and cashing out](https://farmpanel.cc/en/guides/sell-cs2-drops-steam-market)
- [CS2 farm: by hand vs. a farm panel](https://farmpanel.cc/en/compare/manual-multi-accounting)

## Links

| | |
| --- | --- |
| Website | [farmpanel.cc](https://farmpanel.cc) |
| Product | [farmpanel.cc/en/product](https://farmpanel.cc/en/product) |
| Changelog | [farmpanel.cc/en/changelog](https://farmpanel.cc/en/changelog) |
| Telegram | [t.me/farmpanel_en](https://t.me/farmpanel_en) |

---

<div align="center">

This repository distributes signed FarmPanel binaries only.
The application's source code is proprietary and closed.

`system status · all systems operational`

**FarmPanel Systems** · All rights reserved

</div>
