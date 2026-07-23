<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="Десктопное приложение FarmPanel, экран Accounts: боковая навигация (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) и таблица аккаунтов со статусом, логином, ником, воркфлоу, песочницей и временем последнего входа"/>

<br/>

# FARMPANEL

**Панель для фермы аккаунтов Steam и CS2 — оркестрация мультиаккаунтов на Windows**

`запуск · изоляция · мониторинг · восстановление`

FarmPanel — десктопная панель для Windows, которая держит **ферму
аккаунтов Steam** на серьёзном уровне: запускает, изолирует в песочницах,
следит и автоматически перезапускает каждый **аккаунт CS2** в вашей ферме —
от пяти аккаунтов до нескольких сотен — из одного окна, без автофарма
и без ботов.

[**Скачать для Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Сайт](https://farmpanel.cc) ·
[О продукте](https://farmpanel.cc/product) ·
[Telegram](https://t.me/farmpanel_ru)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=%D1%81%D0%BA%D0%B0%D1%87%D0%B8%D0%B2%D0%B0%D0%BD%D0%B8%D0%B9&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__ru-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_ru)

Также доступно на: [English](./README.md) · [Español](./README.es.md)

</div>

---

## Что такое FarmPanel

Если у вас больше одного аккаунта Steam — вы знаете эту рутину: десяток
окон открыты одновременно, упавший CS2 нужно заметить и перезапустить
вручную, и нет простого способа понять, кто уже завис на загрузке, а кто
давно в матче. Чем больше аккаунтов в ферме, тем тяжелее эта рутина.

**FarmPanel — панель для фермы аккаунтов Steam и CS2**, созданная именно
для того, чтобы убрать эту рутину. Это десктопное приложение для Windows,
которое запускает, изолирует и держит под наблюдением всю ферму
мультиаккаунтов Steam из одного окна — реальная альтернатива ручному
управлению аккаунтами или связке из скриптов и виртуальных машин.

FarmPanel — **не автофарм и не бот**. Он не играет за вас и не имитирует
действия в игре — он управляет всем, что происходит *вокруг* игры: запуском
клиентов, приглашениями в лобби, восстановлением после сбоев и живой
видимостью по каждому аккаунту. Все игровые действия остаются за живым
человеком, поэтому ферма ведёт себя — и выглядит — как настоящие игроки,
ведь так и есть.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Почему владельцы ферм выбирают FarmPanel

**01 — Без автофарма. Совсем.**
FarmPanel никогда не играет за вас. Все действия в игре выполняются
вручную, поэтому аккаунты выглядят живыми, ведь так и есть.

**02 — Настройте один раз.**
Каждый запуск и вход проходит по одному и тому же детерминированному
сценарию. Что сработало вчера, сработает и завтра, без сюрпризов.

**03 — Сбои чинятся сами.**
Если Steam или CS2 упали, FarmPanel заметит и поднимет их за считанные
секунды, без вашего участия.

**04 — Настоящая изоляция в песочницах.**
Каждый аккаунт работает в своём изолированном окружении: ни общих сессий,
ни общих файлов, ни пересечения отпечатков между аккаунтами.

**05 — Пароли не покидают ваш ПК.**
Данные для входа зашифрованы встроенной защитой Windows и хранятся только
на вашем компьютере — никуда не отправляются.

**06 — Видимость по каждому аккаунту.**
Живая панель в реальном времени: статус, состояние матча, время работы.
Не нужно гадать, чем занята ферма.

**07 — Свой сетевой маршрут для каждого аккаунта.**
Выбирайте лучший регион для каждого аккаунта — настройку сети FarmPanel
возьмёт на себя.

**08 — Растёт вместе с фермой.**
Начните с пяти аккаунтов и дорастите до сотен. Одна и та же панель,
один и тот же процесс — от начала и до конца.

## Как начать

1. Скачайте установщик — кнопка **[Скачать для Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   выше или раздел [Releases](https://github.com/leryqq/farmpanel-releases/releases)
   этого репозитория.
2. Запустите `Setup.exe` — FarmPanel сам проверит систему и настроит всё
   по шагам.
3. Добавьте свои аккаунты Steam и запустите первую ферму.

```
требования:     Windows 10/11 (64-bit) · .NET 8
рекомендуется:  32 ГБ ОЗУ · SSD · 16-32 аккаунта CS2 одновременно
обновления:     автоматически, из этого репозитория
```

## Частые вопросы

**FarmPanel играет за меня?**
Нет, и в этом суть. Ботов и автофарма здесь нет. FarmPanel управляет
аккаунтами — запускает их, следит за ними, собирает лобби и чинит сбои.
В игре всё делаете вы, поэтому аккаунты ведут себя как живые игроки, ведь
так и есть.

**Где хранятся мои пароли?**
Только на вашем компьютере. Они зашифрованы встроенной защитой Windows,
не сохраняются открытым текстом и никуда не отправляются.

**Работает только с CS2?**
Сейчас глубже всего поддерживается CS2, включая живую информацию о матчах.
Другие игры на подходе.

**Сколько это стоит?**
Стоимость зависит от размера фермы. [Напишите нам в Telegram](https://t.me/farmpanel_ru) —
подберём тариф: от небольших конфигураций до сотен аккаунтов.

Больше вопросов и ответов — на [сайте](https://farmpanel.cc/product#faq).

## Гайды и полезные материалы

- [Как безопасно запускать несколько аккаунтов Steam](https://farmpanel.cc/ru/guides/run-multiple-steam-accounts-safely)
- [Песочница Steam: изоляция аккаунтов фермы](https://farmpanel.cc/ru/guides/steam-account-sandboxing)
- [Сколько аккаунтов CS2 тянет один ПК для фермы](https://farmpanel.cc/ru/guides/how-many-cs2-accounts-per-pc)
- [Еженедельный дроп CS2: как он работает](https://farmpanel.cc/ru/guides/cs2-weekly-drop-explained)
- [Баны CS2: риски для фермы аккаунтов](https://farmpanel.cc/ru/guides/cs2-multi-account-ban-risks)
- [Prime-аккаунты для фермы CS2: нужны ли](https://farmpanel.cc/ru/guides/prime-accounts-for-cs2-farming)
- [Экономика фарма кейсов CS2: доход фермы](https://farmpanel.cc/ru/guides/cs2-case-farming-economics)
- [Как продать дроп CS2 и вывести деньги](https://farmpanel.cc/ru/guides/sell-cs2-drops-steam-market)
- [Ферма CS2 вручную или через панель: сравнение](https://farmpanel.cc/ru/compare/manual-multi-accounting)

## Ссылки

| | |
| --- | --- |
| Сайт | [farmpanel.cc](https://farmpanel.cc) |
| О продукте | [farmpanel.cc/product](https://farmpanel.cc/product) |
| История изменений | [farmpanel.cc/changelog](https://farmpanel.cc/changelog) |
| Telegram | [t.me/farmpanel_ru](https://t.me/farmpanel_ru) |

---

<div align="center">

Этот репозиторий — публичный дистрибутив подписанных бинарников FarmPanel.
Исходный код приложения распространяется отдельно и закрыт.

`статус системы · все системы работают`

**FarmPanel Systems** · Все права защищены

</div>
