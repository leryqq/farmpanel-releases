<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="Application de bureau FarmPanel, écran Comptes : navigation latérale (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) et une grille de comptes avec les colonnes statut, identifiant, pseudo, workflow, sandbox et dernière connexion"/>

<br/>

# FARMPANEL

**Panneau de gestion de ferme de comptes Steam et CS2 — orchestration multicompte sous Windows**

`lancer · isoler · surveiller · récupérer`

FarmPanel est le panneau de bureau Windows qui fait tourner une **ferme de
comptes Steam** à grande échelle. Il lance, isole en sandbox, surveille et
redémarre automatiquement chaque **compte CS2** de votre ferme — de cinq
comptes à plusieurs centaines — depuis une seule fenêtre, sans autofarm et
sans bots.

[**Télécharger pour Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Site web](https://farmpanel.cc) ·
[Produit](https://farmpanel.cc/fr/product) ·
[Telegram](https://t.me/farmpanel_fr)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__fr-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_fr)

Également disponible en : [English](./README.md) · [Русский](./README.ru.md) · [Español](./README.es.md) · [Português](./README.pt.md) · [Türkçe](./README.tr.md) · [Bahasa Indonesia](./README.id.md) · [Tiếng Việt](./README.vi.md) · [हिन्दी](./README.hi.md) · [中文](./README.zh.md) · [العربية](./README.ar.md)

</div>

---

## Qu'est-ce que FarmPanel

Si vous gérez plus d'un compte Steam, vous connaissez déjà le refrain : une
dizaine de fenêtres ouvertes en même temps, un client CS2 planté qu'il faut
repérer et relancer à la main, aucun moyen simple de savoir qui est bloqué au
chargement et qui est déjà en partie. Plus vous ajoutez de comptes à votre
ferme, plus la corvée s'alourdit.

**FarmPanel est un panneau de gestion de ferme de comptes Steam et CS2 conçu
précisément pour supprimer cette corvée.** C'est une application de bureau
Windows qui lance, isole et surveille une ferme multicompte entière depuis
une seule fenêtre — une vraie alternative à la gestion manuelle de comptes
Steam ou à un bricolage de scripts et de machines virtuelles.

FarmPanel **n'est pas un bot d'autofarm**. Il ne joue pas à votre place et ne
simule pas d'actions en jeu — il gère tout ce qui se passe *autour* du jeu :
démarrer les clients, envoyer les invitations de lobby, récupérer les
sessions plantées et vous offrir une visibilité en temps réel sur chaque
compte. Chaque action en jeu reste entre les mains d'une personne réelle,
donc votre ferme se comporte — et ressemble — à de vrais joueurs, parce que
c'en est.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Pourquoi les gérants de ferme choisissent FarmPanel

**01 — Jamais d'autofarm.**
FarmPanel ne joue jamais à votre place. Chaque action en jeu est faite à la
main, donc les comptes paraissent humains, parce qu'ils le sont.

**02 — Configurez une seule fois.**
Chaque lancement et chaque connexion suit la même séquence déterministe. Ce
qui marchait hier marche demain, sans surprise.

**03 — Les plantages se corrigent tout seuls.**
Si Steam ou CS2 tombe, FarmPanel le détecte et le relance en quelques
secondes, sans intervention.

**04 — Un vrai isolement en sandbox.**
Chaque compte tourne dans son propre environnement isolé — pas de sessions
partagées, pas de fichiers partagés, pas de mélange d'empreintes entre
comptes.

**05 — Les mots de passe ne quittent jamais votre PC.**
Les identifiants sont chiffrés avec la sécurité intégrée de Windows et
stockés uniquement sur votre machine, jamais envoyés ailleurs.

**06 — Une visibilité en temps réel sur chaque compte.**
Un tableau de bord en temps réel par compte : statut, état de la partie,
temps d'activité. Fini les devinettes sur ce que fait la ferme.

**07 — Un routage réseau par compte.**
Choisissez la meilleure région de serveur pour chaque compte ; FarmPanel
configure le réseau pour vous.

**08 — Évolue avec votre ferme.**
Commencez avec cinq comptes, passez à des centaines. Le même panneau, le
même flux de travail, du début à la fin.

## Pour commencer

1. Téléchargez l'installeur — **[Télécharger pour Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   ci-dessus, ou depuis la page [Releases](https://github.com/leryqq/farmpanel-releases/releases) de ce dépôt.
2. Lancez `Setup.exe`. FarmPanel vérifie votre système et vous guide dans la configuration.
3. Ajoutez vos comptes Steam et lancez votre première ferme.

```
prérequis :     Windows 10/11 (64 bits) · .NET 8
recommandé :    32 Go de RAM · SSD · 16-32 comptes CS2 simultanés
mises à jour :  automatiques, depuis ce dépôt
```

## FAQ

**FarmPanel joue-t-il à ma place ?**
Non — c'est tout l'intérêt. Il n'y a ni bots ni autofarm. FarmPanel gère les
comptes : lancement, surveillance, montage des lobbies, réparation des
plantages. Tout ce qui se passe en jeu est fait par vous, donc vos comptes se
comportent comme de vrais joueurs, parce qu'ils le sont.

**Où sont stockés mes mots de passe ?**
Uniquement sur votre machine. Ils sont chiffrés avec la sécurité intégrée de
Windows, jamais stockés en clair et jamais envoyés ailleurs.

**Est-ce que ça ne fonctionne qu'avec CS2 ?**
CS2 bénéficie aujourd'hui du support le plus poussé, y compris la télémétrie
de partie en temps réel. D'autres jeux arrivent.

**Combien ça coûte ?**
Le tarif dépend de la taille de la ferme. [Écrivez-nous sur Telegram](https://t.me/farmpanel_fr)
et nous adapterons une formule à votre configuration — des petites
installations à des centaines de comptes.

Plus de réponses dans la [FAQ produit](https://farmpanel.cc/fr/product#faq).

## Guides et ressources

- [Comment utiliser plusieurs comptes Steam en toute sécurité](https://farmpanel.cc/fr/guides/run-multiple-steam-accounts-safely)
- [Le sandboxing des comptes Steam, expliqué](https://farmpanel.cc/fr/guides/steam-account-sandboxing)
- [Combien de comptes CS2 un PC peut-il faire tourner ?](https://farmpanel.cc/fr/guides/how-many-cs2-accounts-per-pc)
- [Le drop hebdomadaire de CS2, expliqué](https://farmpanel.cc/fr/guides/cs2-weekly-drop-explained)
- [Les risques de bannissement en multicompte CS2](https://farmpanel.cc/fr/guides/cs2-multi-account-ban-risks)
- [Faut-il des comptes Prime pour farmer CS2 ?](https://farmpanel.cc/fr/guides/prime-accounts-for-cs2-farming)
- [L'économie du farm de caisses CS2](https://farmpanel.cc/fr/guides/cs2-case-farming-economics)
- [Vendre ses drops CS2 et retirer l'argent](https://farmpanel.cc/fr/guides/sell-cs2-drops-steam-market)
- [Ferme CS2 : à la main vs. avec un panneau](https://farmpanel.cc/fr/compare/manual-multi-accounting)

## Liens

| | |
| --- | --- |
| Site web | [farmpanel.cc](https://farmpanel.cc) |
| Produit | [farmpanel.cc/fr/product](https://farmpanel.cc/fr/product) |
| Changelog | [farmpanel.cc/fr/changelog](https://farmpanel.cc/fr/changelog) |
| Telegram | [t.me/farmpanel_fr](https://t.me/farmpanel_fr) |

---

<div align="center">

Ce dépôt ne distribue que des binaires FarmPanel signés.
Le code source de l'application est propriétaire et fermé.

`état du système · tous les systèmes opérationnels`

**FarmPanel Systems** · Tous droits réservés

</div>
