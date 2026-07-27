<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="Aplicación de escritorio FarmPanel, pantalla Accounts: navegación lateral (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) y una tabla de cuentas con estado, login, apodo, workflow, sandbox y último inicio de sesión"/>

<br/>

# FARMPANEL

**Panel para granjas de cuentas Steam y CS2 — orquestación multicuenta para Windows**

`arranque · aislamiento · monitoreo · recuperación`

FarmPanel es el panel de escritorio para Windows que lleva una **granja
multicuenta de Steam** en serio: arranca, aísla en sandboxes, vigila y
reinicia automáticamente cada **cuenta de CS2** de tu granja —de cinco
cuentas a varios cientos— desde una sola ventana, sin autofarm y sin bots.

[**Descargar para Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Sitio web](https://farmpanel.cc) ·
[Producto](https://farmpanel.cc/es/product) ·
[Telegram](https://t.me/farmpanel_es)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=versi%C3%B3n&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=descargas&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__es-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_es)

Disponible también en: [English](./README.md) · [Русский](./README.ru.md) · [Português](./README.pt.md) · [Français](./README.fr.md) · [Türkçe](./README.tr.md) · [Bahasa Indonesia](./README.id.md) · [Tiếng Việt](./README.vi.md) · [हिन्दी](./README.hi.md) · [中文](./README.zh.md) · [العربية](./README.ar.md)

</div>

---

## Qué es FarmPanel

Si manejas más de una cuenta de Steam, ya conoces la rutina: una docena de
ventanas abiertas a la vez, un cliente de CS2 que se cae y hay que
reiniciar a mano, y ninguna forma sencilla de saber quién sigue cargando y
quién ya lleva rato en partida. Cuantas más cuentas suma tu granja, peor se
pone esa rutina.

**FarmPanel es un panel para granjas de cuentas de Steam y CS2** creado
para quitarte justo ese trabajo de encima. Es una aplicación de escritorio
para Windows que arranca, aísla y vigila toda una granja multicuenta desde
una sola ventana — una alternativa real a gestionar cuentas de Steam a
mano o a montar una mezcla de scripts y máquinas virtuales.

FarmPanel **no es un bot de autofarm**. No juega por ti ni simula acciones
dentro del juego: gestiona todo lo que pasa *alrededor* del juego —
arrancar los clientes, enviar invitaciones de lobby, recuperar sesiones
caídas y darte visibilidad en vivo de cada cuenta. Cada acción dentro del
juego la hace una persona real, así que tu granja se comporta —y parece—
jugadores reales, porque lo son.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Por qué los dueños de granjas eligen FarmPanel

**01 — Sin autofarm. Nunca.**
FarmPanel jamás juega por ti. Cada acción dentro del juego se hace a mano,
así que tus cuentas parecen humanas, porque lo son.

**02 — Configúralo una vez.**
Cada arranque e inicio de sesión sigue la misma secuencia determinista.
Lo que funcionó ayer funciona mañana, sin sorpresas.

**03 — Los fallos se arreglan solos.**
Si Steam o CS2 se cae, FarmPanel lo detecta y lo levanta en segundos, sin
que tengas que intervenir.

**04 — Aislamiento real en sandboxes.**
Cada cuenta funciona en su propio entorno aislado: sin sesiones
compartidas, sin archivos compartidos, sin mezcla de huellas entre cuentas.

**05 — Tus contraseñas no salen de tu PC.**
Las credenciales se cifran con la seguridad integrada de Windows y se
guardan solo en tu equipo, nunca se envían a ninguna parte.

**06 — Visibilidad en vivo de cada cuenta.**
Un panel en tiempo real por cuenta: estado, partida, tiempo activo. Sin
adivinar qué hace la granja.

**07 — Ruta de red propia por cuenta.**
Elige la mejor región de servidor para cada cuenta; FarmPanel configura la
red por ti.

**08 — Crece con tu granja.**
Empieza con cinco cuentas y escala a cientos. El mismo panel, el mismo
proceso, todo el camino.

## Cómo empezar

1. Descarga el instalador — botón **[Descargar para Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   arriba, o desde la sección [Releases](https://github.com/leryqq/farmpanel-releases/releases)
   de este repositorio.
2. Ejecuta `Setup.exe`. FarmPanel revisa tu sistema y te guía paso a paso.
3. Añade tus cuentas de Steam y lanza tu primera granja.

```
requisitos:      Windows 10/11 (64-bit) · .NET 8
recomendado:     32 GB de RAM · SSD · 16-32 cuentas de CS2 simultáneas
actualizaciones: automáticas, desde este repositorio
```

## Preguntas frecuentes

**¿FarmPanel juega por mí?**
No, y esa es la gracia. No hay bots ni autofarm. FarmPanel gestiona las
cuentas: las arranca, las vigila, monta los lobbies y arregla los fallos.
Todo lo que pasa dentro del juego lo haces tú, así que tus cuentas se
comportan como jugadores reales, porque lo son.

**¿Dónde se guardan mis contraseñas?**
Solo en tu ordenador. Se cifran con la seguridad integrada de Windows,
nunca se guardan en texto plano y nunca se envían a ninguna parte.

**¿Solo funciona con CS2?**
CS2 tiene hoy el soporte más completo, incluida la telemetría de partidas
en vivo. Más juegos están en camino.

**¿Cuánto cuesta?**
El precio depende del tamaño de tu granja. [Escríbenos por Telegram](https://t.me/farmpanel_es)
y armamos el plan adecuado para ti: desde montajes pequeños hasta cientos
de cuentas.

Más respuestas en el [FAQ del producto](https://farmpanel.cc/es/product#faq).

## Guías y recursos

- [Cómo usar varias cuentas de Steam de forma segura](https://farmpanel.cc/es/guides/run-multiple-steam-accounts-safely)
- [Sandbox de Steam: aislar cuentas de granja](https://farmpanel.cc/es/guides/steam-account-sandboxing)
- [¿Cuántas cuentas de CS2 por PC en una granja?](https://farmpanel.cc/es/guides/how-many-cs2-accounts-per-pc)
- [Drop semanal de CS2: cómo funciona](https://farmpanel.cc/es/guides/cs2-weekly-drop-explained)
- [Baneos en CS2: riesgos para granjas](https://farmpanel.cc/es/guides/cs2-multi-account-ban-risks)
- [Cuentas Prime para granjas de CS2](https://farmpanel.cc/es/guides/prime-accounts-for-cs2-farming)
- [Economía del farmeo de cajas de CS2](https://farmpanel.cc/es/guides/cs2-case-farming-economics)
- [Vender drops de CS2 y sacar el dinero](https://farmpanel.cc/es/guides/sell-cs2-drops-steam-market)
- [Granja de CS2: a mano o con un panel](https://farmpanel.cc/es/compare/manual-multi-accounting)

## Enlaces

| | |
| --- | --- |
| Sitio web | [farmpanel.cc](https://farmpanel.cc) |
| Producto | [farmpanel.cc/es/product](https://farmpanel.cc/es/product) |
| Registro de cambios | [farmpanel.cc/es/changelog](https://farmpanel.cc/es/changelog) |
| Telegram | [t.me/farmpanel_es](https://t.me/farmpanel_es) |

---

<div align="center">

Este repositorio distribuye únicamente binarios firmados de FarmPanel.
El código fuente de la aplicación es propietario y cerrado.

`estado del sistema · todo operativo`

**FarmPanel Systems** · Todos los derechos reservados

</div>
