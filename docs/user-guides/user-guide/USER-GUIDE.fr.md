# Guide de l'utilisateur de FarmPanel

**Panneau de contrôle pour votre ferme de comptes Steam et CS2 sous Windows**

Version du document : 1.0

🌐 [English](USER-GUIDE.md) · [Русский](USER-GUIDE.ru.md) · [Español](USER-GUIDE.es.md) · [Português](USER-GUIDE.pt.md) · **Français** · [Türkçe](USER-GUIDE.tr.md) · [Bahasa Indonesia](USER-GUIDE.id.md) · [Tiếng Việt](USER-GUIDE.vi.md) · [हिन्दी](USER-GUIDE.hi.md) · [中文](USER-GUIDE.zh.md) · [العربية](USER-GUIDE.ar.md)

---

> **Comment lire ce guide.** Les boutons, onglets et statuts apparaissent dans l'application exactement comme ils sont écrits en **gras** (par exemple, **Add Account**, **Start**, **Running**), afin que vous cliquiez toujours au bon endroit. Chaque procédure indique sur quoi cliquer, ce qui se passe ensuite et comment confirmer la réussite.

## Sommaire

1. [Introduction](#1-introduction)
2. [Avant de commencer](#2-avant-de-commencer)
3. [Premier lancement](#3-premier-lancement)
4. [Vue d'ensemble de l'interface](#4-vue-densemble-de-linterface)
5. [Flux de travail principaux](#5-flux-de-travail-principaux)
6. [Tâches courantes (« Je veux… »)](#6-tâches-courantes--je-veux)
7. [Référence des fonctionnalités](#7-référence-des-fonctionnalités)
8. [Statuts et indicateurs](#8-statuts-et-indicateurs)
9. [Notifications](#9-notifications)
10. [Erreurs et dépannage](#10-erreurs-et-dépannage)
11. [Bonnes pratiques](#11-bonnes-pratiques)
12. [Foire aux questions](#12-foire-aux-questions)

---

# 1. Introduction

## Qu'est-ce que FarmPanel

**FarmPanel** est une application de bureau Windows qui vous aide à gérer de nombreux comptes Steam et clients Counter-Strike 2 depuis une seule fenêtre. Au lieu d'ouvrir des dizaines de fenêtres Steam à la main, de surveiller chacune et de relancer celles qui se figent, vous gérez toute votre ferme de comptes de façon centralisée — depuis un panneau clair et unique.

FarmPanel lance les clients, isole les comptes les uns des autres, surveille leur état en temps réel et les récupère automatiquement après une panne.

> **Important.** FarmPanel **n'est pas un bot ni un autofarm**. Il ne joue pas à votre place et n'imite pas les actions en jeu. Il gère tout ce qui se passe *autour* du jeu : le lancement des clients, les invitations de lobby, la récupération après les pannes et une visibilité en temps réel pour chaque compte. Toutes les actions en jeu sont effectuées par une personne réelle.

## Quels problèmes il résout

Si vous avez plus d'un compte, cette routine vous est familière :

- vous devez lancer des dizaines de clients Steam et CS2 ;
- chaque compte doit fonctionner séparément, sans gêner les autres ;
- monter des lobbies et envoyer des invitations à la main est lent et fatigant ;
- un CS2 planté doit être repéré et relancé à temps ;
- il est difficile de savoir qui est déjà en partie et qui est bloqué au chargement.

FarmPanel supprime cette routine et réunit chaque opération dans une seule application.

## À qui il s'adresse

L'application est conçue pour toute personne devant gérer de façon centralisée de nombreux comptes Steam et CS2 — d'une poignée à plusieurs centaines — avec un lancement automatisé, une surveillance en temps réel et une récupération fiable après les pannes.

## Ce que vous pouvez faire

- Garder tous les comptes au même endroit et trouver rapidement celui qu'il vous faut.
- Démarrer et arrêter des comptes un par un ou tous à la fois.
- Isoler chaque compte dans son propre environnement protégé (une sandbox).
- Constituer des groupes (party) de comptes et les mettre en file de matchmaking ensemble.
- Surveiller la charge de l'ordinateur, la santé des processus et les plantages en temps réel.
- Récupérer automatiquement les comptes après un plantage ou après la fermeture de l'application.
- Disposer les fenêtres CS2 sur vos écrans à l'aide d'une disposition prédéfinie.

![écran principal de FarmPanel (Dashboard)](../images/dashboard-overview.png)

---

# 2. Avant de commencer

## Configuration requise

| Élément | Minimum | Recommandé |
|---|---|---|
| Système d'exploitation | Windows 10 ou 11 (64 bits) | Windows 10 / 11 (64 bits) |
| Mémoire | 8 Go | 32 Go |
| Disque | N'importe lequel | SSD |
| Comptes simultanés | 2 | 4–10 comptes CS2 |
| Résolution d'écran | zone de travail d'au moins 1280 pixels de large | Full HD (1920×1080) ou plus |

## À préparer à l'avance

- **L'installeur de FarmPanel** — un fichier nommé `Setup.exe` que vous téléchargez sur la page de téléchargement officielle.
- **Une clé de licence** — vous la recevez avec votre achat. Elle se présente ainsi : `XXXX-XXXX-XXXX-XXXX-XXXX` (cinq groupes de quatre caractères).
- **Les informations de vos comptes Steam** — identifiants et mots de passe, et codes Steam Guard si vous les utilisez. Vous pouvez les saisir un par un ou importer une liste depuis un fichier.
- **Une connexion internet** — requise au premier lancement pour activer la licence, puis pour que Steam et CS2 fonctionnent.

## Autorisations

- L'installation **ne nécessite pas de droits d'administrateur** — l'application s'installe uniquement pour votre compte d'utilisateur.
- Au premier lancement de l'installeur, Windows peut afficher une fenêtre bleue **SmartScreen** (« Windows a protégé votre ordinateur ») — c'est un avertissement courant pour les nouveaux programmes. Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.
- L'application peut avoir besoin d'un accès au réseau (pour Steam) et aux règles du Pare-feu Windows. Si une invite du pare-feu apparaît, autorisez l'accès.

## Où sont stockées vos données

Les identifiants et les mots de passe sont chiffrés avec la protection intégrée de Windows et stockés **uniquement sur votre ordinateur**. Ils ne sont jamais enregistrés en clair et ne sont jamais envoyés ailleurs.

---

# 3. Premier lancement

Voici le parcours de l'installation jusqu'à un panneau prêt à l'emploi. Suivez les étapes dans l'ordre.

## Étape 1. Installez l'application

1. Téléchargez l'installeur `Setup.exe` depuis la page de téléchargement.
2. Double-cliquez sur le fichier `Setup.exe`.
3. Si une fenêtre bleue **SmartScreen** apparaît (« Windows a protégé votre ordinateur »), cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**. C'est un avertissement courant pour les nouveaux programmes, pas une erreur.
4. Attendez la fin de l'installation. Aucun droit d'administrateur n'est requis — l'installeur vérifie votre système et prépare tout.

**Ce qui se passe ensuite.** Une icône FarmPanel apparaît sur votre bureau et dans le menu Démarrer.

![la fenêtre de l'installeur Setup.exe](../images/setup-installer.png)

## Étape 2. Ouvrez l'application

Double-cliquez sur l'icône **FarmPanel** de votre bureau.

**Ce que vous verrez.** Au tout premier lancement, tant que la licence n'est pas activée, la fenêtre d'activation (**Activation Wizard**) s'ouvre. L'écran principal n'apparaît qu'après une activation réussie.

## Étape 3. Activez votre licence

La fenêtre d'activation vous guide pas à pas.

1. Saisissez ou collez votre clé de licence dans le champ de saisie. Pour la coller depuis le presse-papiers, cliquez sur **Paste from clipboard**.
2. L'application vérifie le format de la clé à mesure que vous tapez. Quand le format est correct, le bouton d'activation devient disponible.
3. Cliquez sur **Activate**.

**Ce qui se passe ensuite.** L'application contacte le serveur de licences et vérifie la clé. Cela prend quelques secondes — vous verrez l'état **Activating**.

**Signe de réussite.** La fenêtre d'activation se ferme et l'écran principal de l'application (**Dashboard**) s'ouvre. Votre licence est active — vous n'aurez pas à ressaisir la clé lors des prochains lancements.

> **Si l'activation échoue**, l'application affiche un message clair et vous indique la marche à suivre. Les cas courants sont traités dans [10. Erreurs et dépannage](#10-erreurs-et-dépannage).

![la fenêtre d'activation de la licence](../images/license-activation.png)

## Étape 4. Vérifiez les réglages de base

Avant de lancer des comptes pour la première fois, il vaut la peine de vérifier vos réglages.

1. Cliquez sur **Settings** dans le panneau de gauche, ou appuyez sur `Ctrl+,`.
2. Ouvrez la section **Sandboxes** et, si nécessaire, choisissez un dossier pour les sandboxes.
3. Éventuellement, ouvrez **Appearance** et choisissez un thème (**System / Dark / Light**) et la densité de l'interface.

Les réglages s'enregistrent automatiquement : après chaque modification, une brève notification **Saved** apparaît.

## Étape 5. Prêt à démarrer

Vous pouvez maintenant ajouter des comptes et lancer votre première ferme. Voyez comment dans [5. Flux de travail principaux](#5-flux-de-travail-principaux).

**Signe que tout fonctionne.** La barre inférieure de la fenêtre (la barre d'état) affiche un résumé : le nombre de comptes, les processus actifs et la version actuelle de l'application.

---

# 4. Vue d'ensemble de l'interface

L'application fonctionne dans une seule fenêtre principale. Elle se compose d'éléments fixes, toujours présents, et d'une zone d'écran qui change selon la section choisie.

```
┌────────────────────────────────────────────────────────────┐
│  Barre de commandes (Command Bar)                          │
├──────────┬─────────────────────────────────────────────────┤
│          │                                                 │
│ Barre    │   Zone de travail de l'écran sélectionné        │
│ latérale │                                                 │
│          │                                                 │
├──────────┴─────────────────────────────────────────────────┤
│  Barre d'état (Status Bar)                                 │
└────────────────────────────────────────────────────────────┘
```

![structure générale de la fenêtre avec les zones étiquetées](../images/window-layout.png)

## 4.1. Barre de commandes (Command Bar)

**But.** Une bande fixe en haut de la fenêtre. Elle contient la navigation, la recherche globale et les notifications.

**Emplacement.** La toute première ligne de la fenêtre.

**Éléments principaux (de gauche à droite) :**

- **Bouton menu (☰)** — replie et déplie la barre latérale. Raccourci `Ctrl+B`.
- **Logo** — cliquer dessus vous ramène à l'écran principal (**Dashboard**).
- **Fil d'Ariane** — indique où vous êtes, par exemple `Accounts › alex_42 › Events`. Cliquez sur n'importe quel segment pour y aller.
- **Recherche / palette de commandes** — au centre. Appuyez sur `Ctrl+K` pour ouvrir la palette de commandes (voir ci-dessous).
- **Badge de notifications** — une icône avec un compteur (par exemple, `⚠ 3`). Cliquer dessus ouvre le centre de notifications.

**Quand l'utiliser.** La barre de commandes est toujours à portée : pour passer rapidement d'un écran à l'autre, chercher un compte par son identifiant ou lancer une commande sans la souris.

### Palette de commandes (Command Palette)

Appuyez sur `Ctrl+K` à tout moment pour ouvrir la palette de commandes — une zone de recherche pour chaque action et objet de l'application.

1. Commencez à taper le nom d'une commande, d'un écran, d'un identifiant de compte ou d'un workflow.
2. La liste se réduit aux résultats correspondants. Parcourez-les avec `↑` `↓`.
3. Appuyez sur `Entrée` pour exécuter l'élément sélectionné.

**Pourquoi c'est utile.** La palette de commandes est le moyen le plus rapide de trouver quoi que ce soit sans mémoriser l'emplacement des boutons.

![la palette de commandes ouverte](../images/command-palette.png)

## 4.2. Barre latérale (Sidebar)

**But.** La navigation principale de l'application.

**Emplacement.** À gauche, sur toute la hauteur de la fenêtre.

**Sections (de haut en bas) :**

| Icône | Section | Ce qu'elle affiche |
|---|---|---|
| ▤ | **Dashboard** | Vue d'ensemble de toute la ferme |
| 👥 | **Accounts** | Liste de tous les comptes (l'écran de travail principal) |
| ⚙ | **Workflows** | Scénarios de lancement automatisés et leur progression |
| ⚔ | **Matchmaking** | Groupes (party) et recherche de partie |
| 📈 | **Monitoring** | Charge de l'ordinateur et santé des processus |
| 📜 | **Logs** | Le journal des événements |
| ▣ | **Layouts** | Disposition des fenêtres CS2 sur les écrans |
| ▦ | **Sandboxes** | Sandboxes (environnements isolés) |
| ⚙ | **Settings** | Réglages de l'application |
| ? | **Help** | Aide |

Certaines sections affichent un compteur (par exemple, le nombre de comptes) ou un point actif quand il y a de l'activité.

**Actions principales :**

- Cliquez sur une section pour l'ouvrir. Vous pouvez aussi utiliser `Ctrl+1`…`Ctrl+8`.
- Le bouton de repli (ou `Ctrl+B`) réduit le panneau aux icônes pour libérer de l'espace.

**Astuce.** Passer d'une section à l'autre conserve votre état — filtres, sélection et position de défilement. En revenant sur un écran, vous le retrouvez exactement comme vous l'aviez laissé.

![la barre latérale avec toutes les sections](../images/sidebar.png)

## 4.3. Barre d'état (Status Bar)

**But.** Une fine bande en bas de la fenêtre avec un résumé rapide de l'état de toute la ferme.

**Emplacement.** La toute dernière ligne de la fenêtre.

**Ce qu'elle affiche (exemple) :**

```
[env: PROD] | ● 412 comptes (238 en cours) | ▶ 18 workflows | ◎ 7 parties | CPU 42% RAM 71% | ⚠ 3 erreurs | 14:32:08 | v1.0.1
```

- combien de comptes existent et combien sont en cours d'exécution ;
- combien de workflows et de parties actives sont en cours ;
- charge du processeur et de la mémoire ;
- le nombre d'erreurs (cliquez pour ouvrir le centre de notifications) ;
- l'heure et la version de l'application.

**Quand l'utiliser.** Jetez un œil à la barre d'état pour savoir en une seconde si tout va bien.

## 4.4. Écran Dashboard

**But.** Un écran de synthèse unique. En quelques secondes, il répond à : combien de comptes sont en ligne, combien de workflows sont en cours ou ont échoué, y a-t-il de l'activité de matchmaking, y a-t-il des plantages, et quelle est la charge de l'ordinateur.

**Emplacement.** La première section de la barre latérale. Elle s'ouvre juste après le lancement.

**Zones principales :**

- **Bandeau de KPI** — cinq cartes en haut : **Accounts**, **Workflows**, **Matches**, **Errors**, **System**. Chacune affiche un chiffre clé et un mini-graphique. Cliquer sur une carte vous mène à l'écran correspondant.
- **Live Activity Feed** — un flux en temps réel d'événements opérationnels. Utilisez le bouton pause (ou la touche `Espace`) pour mettre le défilement en pause.
- **Account State Heatmap** — une grille où chaque compte est une cellule colorée. La couleur reflète son statut. Survolez pour voir l'identifiant et le statut ; cliquez pour aller au compte.
- **Active Workflows / Matchmaking Queue / Sandboxes** — trois tuiles résumant les workflows, la file de parties et les sandboxes.
- **Failures & Crashes** — un tableau des erreurs et plantages récents de la dernière heure.

**Utilisation typique.** Le matin, ouvrez le **Dashboard** pour évaluer la ferme d'un coup d'œil, puis rendez-vous là où une attention est nécessaire.

**Astuces.**
- Les indicateurs se rafraîchissent automatiquement. Pour forcer un rafraîchissement complet, appuyez sur `F5`.
- Si quelque chose est en rouge dans la carte **Errors** ou le tableau des pannes, commencez votre investigation là.

![le Dashboard avec le bandeau de KPI et le fil d'activité](../images/dashboard-screen.png)

## 4.5. Écran Accounts

**But.** L'écran de travail principal. Ici, vous stockez les comptes, trouvez ceux qu'il vous faut et les démarrez et arrêtez.

**Emplacement.** La deuxième section de la barre latérale (`Ctrl+2`).

**Zones principales :**

- **Barre d'outils** — les boutons **Add Account**, **Import**, **Export** et **Refresh**, le champ de recherche, les filtres et les contrôles d'affichage.
- **Tableau des comptes** — une liste de tous les comptes avec des colonnes : statut, identifiant, pseudo, rang, workflow, sandbox, tags, heure de dernière connexion, et d'autres.
- **Details Pane** (panneau de détails) — à droite. Affiche les détails du compte sélectionné. Affichez-le ou masquez-le avec `Ctrl+\`.

**Ce que vous pouvez faire :**

- Ajouter des comptes un par un ou importer une liste.
- Rechercher et filtrer les comptes.
- Démarrer, arrêter et redémarrer un compte ou plusieurs à la fois.
- Lier des comptes à des sandboxes et attribuer des workflows.
- Consulter une fiche détaillée du compte : données, historique, événements et journaux.

**Utilisation typique.** Sélectionnez les comptes qu'il vous faut dans le tableau, puis effectuez une action sur eux — via la barre d'outils, le menu contextuel (clic droit) ou les raccourcis clavier.

Des instructions détaillées pas à pas se trouvent dans [5. Flux de travail principaux](#5-flux-de-travail-principaux).

![l'écran Accounts avec le tableau et le panneau de détails](../images/accounts-screen.png)

### Panneau de détails du compte (Details Pane)

À droite du tableau, une fiche du compte sélectionné apparaît avec ces onglets :

| Onglet | Ce qu'il affiche |
|---|---|
| **Overview** | Données principales, liaison à la sandbox, workflow attribué, tags, dates clés et boutons d'action |
| **Inventory** | L'inventaire du compte : nombre d'objets et valeur |
| **Workflow** | L'état actuel du scénario attribué et son étape en cours |
| **Events** | Événements récents pour ce compte |
| **Logs** | Le journal des événements filtré sur ce compte |
| **History** | Historique des modifications : création, éditions, renommages, re-liaisons de sandbox |

En bas de l'onglet **Overview** se trouve un bloc de boutons : **Start**, **Stop**, **Restart**, **Pause**, ainsi que **Edit account** et **Delete**. L'action la plus pertinente est mise en évidence : **Start** quand le compte est arrêté, et **Stop** quand il est en cours d'exécution.

## 4.6. Écran Workflows

**But.** Gérer les scénarios de lancement automatisés et observer leur exécution.

**Emplacement.** La troisième section de la barre latérale (`Ctrl+3`).

**Ce qu'est un workflow.** Un workflow est une séquence d'étapes prédéfinie que l'application effectue pour un compte : se connecter à Steam, lancer CS2, etc. Le même scénario s'exécute toujours de la même façon, donc le résultat est prévisible.

- **Definition** (définition) — le modèle de scénario : un ensemble d'étapes.
- **Instance** — une seule exécution d'une définition pour un compte donné.

**Zones principales :**

- **À gauche** — une liste de définitions (modèles) et leurs versions.
- **Au centre** — un tableau des instances en cours : quel scénario, pour quel compte, à quelle étape, combien de tentatives, quand démarrée.
- **À droite** — les détails de l'instance sélectionnée (onglets **Overview**, **State Machine**, **Steps**, **Logs**, **Retries**).
- **En bas** — une frise d'événements repliable pour les instances visibles (`Ctrl+T`).

**Quand l'utiliser.** Venez ici pour voir à quelle étape en est le lancement de chaque compte, mettre en pause ou redémarrer un scénario, ou comprendre pourquoi quelque chose n'a pas abouti.

![l'écran Workflows avec trois panneaux](../images/workflows-screen.png)

## 4.7. Écran Matchmaking

**But.** Constituer des groupes de comptes (party) et les mettre en file de matchmaking ensemble.

**Emplacement.** La quatrième section de la barre latérale (`Ctrl+4`).

**Concepts clés :**

| Terme | Signification |
|---|---|
| **Party** (groupe) | Un ensemble de comptes qui cherchent une partie ensemble |
| **Quorum** | Tous les membres du groupe sont connectés, dans la file et hors partie |
| **Queue** (file) | L'attente d'une partie : position, région, mode |
| **Match Found** (partie trouvée) | Steam a trouvé une partie. L'application confirme la disponibilité de tous les membres automatiquement — vous n'avez rien à faire |
| **Desync** (désynchronisation) | Les membres sont dans un état incohérent (par exemple, quelqu'un a quitté la file) |

**Zones principales :**

- **À gauche** — une liste de groupes avec leur état (quorum, désynchronisation, partie trouvée, inactif).
- **À droite** — les détails du groupe sélectionné : membres, leur état, position dans la file, latence réseau, sandbox.
- **En bas** — une frise des événements récents de matchmaking.

**Quand l'utiliser.** Ici, vous constituez des groupes de 2 à 5 comptes et les mettez en file. Quand une partie est trouvée, l'application confirme la disponibilité de tous les membres automatiquement.

![l'écran Matchmaking avec des groupes et des détails](../images/matchmaking-screen.png)

## 4.8. Écran Monitoring

**But.** Surveiller la charge de l'ordinateur, la santé des processus et les plantages en temps réel.

**Emplacement.** La cinquième section de la barre latérale (`Ctrl+5`).

**Zones principales :**

- **Jauges de ressources** — cartes **CPU**, **RAM**, **Disk**, **Net** et, si disponible, **GPU**, avec les valeurs actuelles et des mini-graphiques.
- **Process Explorer** — un tableau de tous les processus Steam et CS2 en cours : à quel compte chacun appartient, ce qu'il consomme, depuis combien de temps il tourne.
- **Crashes & Warnings** — un flux des pannes récentes.
- **Logs panel** — un journal en bas de l'écran, qui peut être replié.

**Contrôles de temps.** En haut, vous pouvez basculer entre **Live** (temps réel), **Last 1h / 24h** et **Custom** (une période personnalisée). Le bouton **Freeze** (`Ctrl+Espace`) fige l'image pour l'étudier tranquillement.

**Quand l'utiliser.** Si l'ordinateur commence à ralentir ou si les plantages deviennent fréquents, ouvrez **Monitoring** pour voir quel processus consomme des ressources et ce qui a exactement planté.

> **Astuce.** Vous pouvez ouvrir l'écran **Monitoring** dans une fenêtre séparée avec le bouton de détachement et le placer sur un second écran.

![l'écran Monitoring avec les jauges et la liste des processus](../images/monitoring-screen.png)

## 4.9. Écran Logs

**But.** Un journal détaillé de tous les événements de l'application — comme un flux en direct de ce qui se passe.

**Emplacement.** La sixième section de la barre latérale (`Ctrl+6`).

**Fonctions principales :**

- **Filtre par niveau** — les bascules **Error**, **Warn**, **Info**, **Debug**. Par défaut, les erreurs, avertissements et messages d'information sont affichés.
- **Filtre par source** — vous pouvez restreindre le journal à un seul compte, workflow ou sandbox.
- **Recherche** — `Ctrl+F`, avec saut entre les occurrences (`F3` / `Shift+F3`).
- **Follow** (suivi) — le journal défile automatiquement vers les nouvelles lignes. La touche `Espace` active et désactive le suivi. Si vous remontez, le suivi se met en pause et un bouton de retour en bas apparaît.
- **Export** — enregistrer les lignes visibles dans un fichier.

**Quand l'utiliser.** Quand vous avez besoin des détails : ce qui est arrivé exactement à un compte donné et dans quel ordre.

![l'écran Logs avec un journal d'événements](../images/logs-screen.png)

## 4.10. Écran Layouts

**But.** Disposer les fenêtres CS2 sur un ou plusieurs écrans à l'aide d'une disposition prédéfinie.

**Emplacement.** La septième section de la barre latérale (`Ctrl+7`).

**Concepts clés :**

- **Preset** (préréglage) — une disposition de fenêtres enregistrée.
- **Slot** (emplacement) — une zone rectangulaire sur un écran où ira une fenêtre.
- **Snap** (disposer) — la commande qui place les fenêtres en cours dans les emplacements.

**Zones principales :**

- **À gauche** — une liste de préréglages enregistrés.
- **À droite** — un canevas montrant vos écrans, sur lequel vous placez les emplacements.
- **En bas** — un tableau d'affectations : quel emplacement correspond à quel compte ou rôle.

**Comment l'utiliser.**
1. Créez un préréglage avec le bouton **New Preset**.
2. Placez les emplacements sur le canevas.
3. Définissez quel compte va dans quel emplacement.
4. Cliquez sur **Apply** ou **Snap windows** — l'application place les fenêtres CS2 en cours aux endroits définis.

> **Filet de sécurité.** Avant de disposer, l'application mémorise les positions actuelles des fenêtres. Le bouton **Revert layout** restaure les positions précédentes dans un délai d'une minute.

![l'écran Layouts avec le canevas des écrans](../images/layouts-screen.png)

## 4.11. Écran Sandboxes

**But.** Gérer les sandboxes — les environnements isolés dans lesquels les clients Steam s'exécutent.

**Emplacement.** La huitième section de la barre latérale (`Ctrl+8`).

**Ce qu'est une sandbox.** Une sandbox est un environnement distinct et protégé pour un client Steam. Les comptes dans des sandboxes différentes ne se chevauchent jamais : ils ne partagent ni sessions, ni fichiers, ni traces. Un compte est lié à une sandbox.

**Quand l'utiliser.** Ici, vous créez des sandboxes et surveillez leur état. Dans la plupart des cas, les sandboxes sont attribuées automatiquement lors de l'ajout de comptes, donc vous avez rarement besoin de venir ici exprès.

## 4.12. Écran Settings

**But.** Adapter l'application à vos préférences.

**Emplacement.** La section **Settings** en bas de la barre latérale (`Ctrl+,`).

**Disposition.** À gauche se trouve une liste de sections de réglages ; à droite, les réglages eux-mêmes. Les modifications s'enregistrent immédiatement : une brève notification **Saved** apparaît après chacune.

**Sections de réglages :**

| Section | Ce qu'elle configure |
|---|---|
| **General** | Lancement avec Windows, réduction dans la barre d'état système, canal de mise à jour |
| **Appearance** | Thème (**System / Dark / Light**), densité, échelle de police, réduction des animations |
| **Accounts** | Comportement lors de la création de comptes, rétention des comptes supprimés |
| **Workflows** | Politique de nouvelles tentatives, limites d'exécutions simultanées |
| **Sandboxes** | Dossier des sandboxes, récupération automatique |
| **Monitoring** | Fréquence de rafraîchissement des données, seuils d'avertissement |
| **Notifications** | Notifications et sons par niveau de gravité |
| **Layouts** | Dispositions par défaut, comportement multi-écran |
| **Hotkeys** | Raccourcis clavier — réassignables |
| **Advanced** | Niveau de journalisation, diagnostics, sélection d'environnement, réinitialisation |
| **About** | Version de l'application, boutons pour ouvrir les dossiers de données et de journaux |

> **Remarque.** Certains réglages (par exemple, le dossier des sandboxes ou l'environnement) ne s'appliquent qu'après un redémarrage. Ces réglages affichent un badge « Requires restart » à côté.

![l'écran Settings](../images/settings-screen.png)

---

# 5. Flux de travail principaux

C'est la section la plus importante. Elle contient des instructions complètes, pas à pas, pour les tâches principales. Chaque étape décrit ce que vous verrez et comment confirmer la réussite.

## 5.1. Ajouter un seul compte

**Objectif.** Ajouter un nouveau compte Steam à l'application.

**Ce qu'il vous faut.** L'identifiant et le mot de passe du compte. Un code Steam Guard le cas échéant.

### Étape 1 — Ouvrez le formulaire d'ajout

Allez sur l'écran **Accounts** et cliquez sur **Add Account** dans la barre d'outils. Vous pouvez aussi appuyer sur `Ctrl+N`.

**Résultat attendu.** Un formulaire avec des champs pour le nouveau compte s'ouvre.

### Étape 2 — Renseignez les informations

Remplissez les champs :

- **Login** — obligatoire, doit être unique.
- **Password** — obligatoire.
- **Steam Guard secret** — le code Steam Guard, si vous en avez un (facultatif).
- **Nickname** — facultatif ; peut être récupéré automatiquement à la première connexion.
- **Tags** — tags facultatifs pour regrouper.
- **Sandbox binding** — choisissez **Auto-assign**, une sandbox précise ou **None**.
- **Workflow** — le scénario de lancement, si vous voulez en attribuer un tout de suite.

**Résultat attendu.** Si l'identifiant est déjà pris, le champ est surligné en rouge avec une explication. Un mot de passe faible est surligné en ambre — c'est un avertissement qui n'empêche pas d'enregistrer.

### Étape 3 — Enregistrez le compte

Cliquez sur le bouton d'enregistrement du formulaire.

**Résultat attendu.** Le formulaire se ferme et le nouveau compte apparaît dans le tableau avec un statut **Draft** ou, s'il est lié à une sandbox, prêt à être lancé.

**Signe de réussite.** Le compte est visible dans le tableau de l'écran **Accounts**.

### Astuces

- Si vous activez **Validate immediately** dans le formulaire, l'application vérifie la connexion en arrière-plan et affiche le résultat en notification.
- Pour qu'un compte soit lançable, il doit être lié à une sandbox. Le choix le plus simple est **Auto-assign**.

### Erreurs courantes et comment les corriger

- **« Login already in use. »** Cet identifiant existe déjà dans l'application. Vérifiez votre liste de comptes — vous l'avez peut-être déjà ajouté.
- **Sandbox oubliée.** Un compte sans sandbox ne peut pas être lancé. Liez-en une plus tard via le menu contextuel → **Bind sandbox**.

![le formulaire d'ajout de compte](../images/accounts-add-form.png)

## 5.2. Importer une liste de comptes depuis un fichier

**Objectif.** Ajouter rapidement de nombreux comptes à la fois depuis un fichier.

**Ce qu'il vous faut.** Un fichier avec une liste de comptes (TXT, CSV ou TSV). Le format de ligne TXT le plus simple est `identifiant:motdepasse` (vous pouvez aussi utiliser `identifiant:motdepasse:steamguard:pseudo`).

### Étape 1 — Lancez l'assistant d'importation

Sur l'écran **Accounts**, cliquez sur la flèche à côté du bouton **Import** et choisissez une source — par exemple, **From file…**. Vous pouvez aussi appuyer sur `Ctrl+I`.

**Résultat attendu.** Un assistant d'importation pas à pas s'ouvre.

### Étape 2 — Choisissez la source et l'attribution des sandboxes

Indiquez le fichier avec le bouton **Browse…**. En bas, choisissez comment attribuer les sandboxes :

- **Auto-assign (round-robin)** — répartir en cycle (recommandé) ;
- **Bind to specific sandbox** — les lier toutes à une même sandbox ;
- **Leave unbound** — les laisser sans sandbox.

Cliquez sur Suivant.

### Étape 3 — Vérifiez la reconnaissance des données

L'assistant affiche les premières lignes du fichier sous forme de tableau. Assurez-vous que les données ont bien été réparties en colonnes. Si le délimiteur a été mal détecté, définissez-le manuellement.

**Résultat attendu.** Dans l'aperçu, identifiants et mots de passe sont dans leurs propres colonnes.

### Étape 4 — Mappez les champs

Glissez les en-têtes de colonnes sur les cases requises : **Login**, **Password**, **SteamGuard**, **Nickname**.

### Étape 5 — Vérifiez la validité des lignes

L'assistant marque chaque ligne : ✓ valide, ⚠ avertissement, ✕ erreur. Les lignes en erreur peuvent être corrigées ici même ou ignorées.

**Résultat attendu.** Vous voyez combien de comptes seront ajoutés, combien sont des doublons et combien comportent des erreurs.

### Étape 6 — Confirmez l'importation

Cliquez sur **Import N accounts**.

**Résultat attendu.** Une barre de progression avec un statut par ligne apparaît. Une fois terminée, les comptes apparaissent dans le tableau.

**Signe de réussite.** Le nombre de comptes dans le tableau a augmenté du nombre importé.

### Comment annuler et récupérer

Si vous annulez l'importation pendant son exécution, l'application propose d'annuler le lot déjà ajouté. Confirmez l'annulation pour revenir à l'état initial.

![l'assistant d'importation, étape de validation des lignes](../images/import-wizard-validation.png)

## 5.3. Lancer plusieurs comptes

**Objectif.** Démarrer plusieurs comptes en même temps.

**Ce qu'il vous faut.** Des comptes ajoutés et liés à des sandboxes.

### Étape 1 — Sélectionnez les comptes

Sur l'écran **Accounts**, cochez les comptes voulus dans la première colonne. Pour sélectionner tous ceux visibles, appuyez sur `Ctrl+A`.

**Résultat attendu.** La barre d'outils passe en mode groupé et indique combien de lignes sont sélectionnées, par exemple `12 selected`.

### Étape 2 — Démarrez les comptes sélectionnés

Cliquez sur **Start** dans la barre d'outils groupée. Vous pouvez aussi appuyer sur `Ctrl+R`.

**Résultat attendu.** Le statut des comptes sélectionnés passe à **Starting**. L'application prépare chaque compte et commence le lancement. Le lancement se fait par lots pour ne pas surcharger l'ordinateur.

### Étape 3 — Attendez le lancement

Surveillez la colonne de statut. Attendez que les comptes passent à l'état **Running**.

**Résultat attendu.** Les comptes lancés affichent **Running**, avec un compteur de temps d'activité à côté.

**Signe de réussite.** Tous les comptes sélectionnés affichent **Running**. Le nombre d'actifs dans la barre d'état a augmenté.

### Astuces

- Vous n'êtes pas obligé de lancer tous les comptes d'un coup. Commencez par un petit lot, assurez-vous que tout est stable, puis ajoutez-en d'autres.
- Pour lancer un seul compte : sélectionnez une ligne et cliquez sur **Start**, ou utilisez le bouton **Start** dans le panneau de détails à droite.

### Erreurs courantes et récupération

- **Un compte reste en Starting trop longtemps.** La connexion est peut-être lente. Attendez ; si le statut passe à **Error**, utilisez le bouton **Retry**.
- **Certains comptes n'ont pas démarré.** Après un lancement groupé, un résumé indique combien ont réussi et échoué. Cliquez sur **Filter to failed** pour ne traiter que ceux-là.

![lancement groupé de comptes, statuts Starting/Running](../images/accounts-bulk-start.png)

## 5.4. Arrêter tous les comptes en cours d'exécution

**Objectif.** Fermer proprement tous les comptes actifs.

### Étape 1 — Sélectionnez les comptes

Sélectionnez les comptes en cours d'exécution. Pour sélectionner tous ceux visibles, appuyez sur `Ctrl+A`.

### Étape 2 — Arrêtez-les

Cliquez sur **Stop** dans la barre d'outils groupée, ou appuyez sur `Ctrl+.` (Ctrl et point).

**Résultat attendu.** L'application ferme proprement chaque compte. Le statut passe à **Stopped**. Si un compte ne répond pas, l'application le ferme de force au bout d'un moment.

**Signe de réussite.** Tous les comptes affichent **Stopped**. Le nombre d'actifs dans la barre d'état a diminué.

### Astuces

- **Stop** est un arrêt en douceur. L'application tente d'abord de fermer les clients correctement.
- Si un compte est en partie, terminez d'abord les actions en jeu, puis arrêtez-le.

## 5.5. Créer un groupe et le mettre en file

**Objectif.** Constituer un groupe de plusieurs comptes et les mettre en file de matchmaking ensemble.

**Ce qu'il vous faut.** Plusieurs comptes en cours d'exécution (**Running**) qui se sont connectés.

### Étape 1 — Créez un groupe

Allez sur l'écran **Matchmaking** et cliquez sur **Create Party**. Vous pouvez aussi appuyer sur `Ctrl+N`.

**Résultat attendu.** Une fenêtre s'ouvre où vous pouvez ajouter des comptes au groupe et lui donner un nom.

### Étape 2 — Ajoutez des membres et enregistrez

Ajoutez de 2 à 5 comptes au groupe, définissez un nom et enregistrez.

**Résultat attendu.** Le nouveau groupe apparaît dans la liste de gauche.

### Étape 3 — Vérifiez le quorum

Sélectionnez le groupe et regardez ses membres à droite. Assurez-vous que le groupe est à l'état **Quorum** — c'est-à-dire que tous les membres sont connectés et prêts.

**Résultat attendu.** Le groupe affiche un badge **✓ Quorum**. Si un membre a un problème (par exemple, une connexion lente), il est indiqué sur une ligne à part.

### Étape 4 — Mettez le groupe en file

Cliquez sur **Queue** pour le groupe sélectionné (ou `Ctrl+Q`). Pour mettre tous les groupes en file d'un coup, utilisez **Queue All** dans la barre d'outils.

**Résultat attendu.** Avant la mise en file, l'application effectue ses vérifications. Ensuite, tous les membres entrent dans la file, avec leurs positions et la latence réseau affichées.

**Signe de réussite.** Les membres sont à l'état de file, avec un compteur de temps d'attente qui tourne.

### Astuces

- Choisissez la région et le mode dans la barre d'outils (par exemple, `EU` et `Premier`) avant la mise en file.
- Si le groupe passe à l'état **Desync**, utilisez l'action **Re-sync** pour mettre la file en pause et attendre un état cohérent.

![un groupe dans la file avec les positions des membres](../images/matchmaking-party-queue.png)

## 5.6. Ce qui se passe quand une partie est trouvée

**Objectif.** Comprendre ce que fait l'application au moment où une partie est trouvée.

**Ce qu'il vous faut.** Un groupe qui est dans la file.

### L'acceptation de la partie est automatique

Quand Steam trouve une partie, une bannière bien visible **MATCH FOUND** apparaît pour le groupe. **Vous n'avez rien à cliquer** — l'application confirme la disponibilité de tous les membres du groupe dans le délai imparti. Aucune action de votre part n'est requise.

**Résultat attendu.** Les membres du groupe acceptent la partie automatiquement ; leur état passe à **✓ Accepted**.

**Signe de réussite.** Tous les membres affichent **Accepted**, et la partie commence.

> **Astuce.** Vous voulez savoir qu'une partie a été trouvée sans regarder l'écran ? Activez une alerte sonore pour **Match found** dans **Settings → Notifications**. L'acceptation se fait quand même automatiquement — le son sert seulement à vous tenir informé.

### Que faire si le groupe se désynchronise

Parfois, une partie ne peut pas être confirmée pour tout le monde — par exemple, si un membre a quitté la file. Le groupe passe alors à l'état **Desync**. Utilisez l'action **Re-sync** et, si nécessaire, retirez le membre problématique avec **Drop member**, puis remettez les autres en file.

![la bannière Match Found](../images/matchmaking-match-found.png)

## 5.7. Récupérer après un plantage ou un redémarrage de l'application

**Objectif.** Ramener la ferme à un état opérationnel après le plantage d'un client, ou après la fermeture puis réouverture de l'application.

**Ce qu'il vous faut.** Rien de plus — la récupération se fait en grande partie automatiquement.

### Ce qui se passe automatiquement

- **Après le plantage d'un client.** Si Steam ou CS2 se ferme de façon inattendue, l'application le remarque, marque le compte du statut **Crashed** et affiche une notification avec un bouton **Restart**. La récupération se fait souvent d'elle-même en quelques secondes.
- **Après un redémarrage de l'application.** Au démarrage, l'application recherche les processus Steam et CS2 restés de la session précédente et les reprend sous sa gestion. Pendant ce temps, un indicateur **Recovering** apparaît dans la barre d'état. Les comptes repris sont marqués « Reattached » brièvement.

### Ce qu'il faut faire manuellement

1. Ouvrez le **Dashboard** et regardez le tableau **Failures & Crashes**.
2. Pour un compte planté, cliquez sur **Restart** dans la notification, dans la ligne du compte ou dans le panneau de détails.
3. Si l'application signale un processus orphelin (**Orphan process**) dans le centre de notifications, choisissez **Adopt** ou **Kill**.

**Signe de réussite.** Les comptes sont de nouveau au statut **Running**, les marqueurs rouges de plantage ont disparu, et il n'y a plus d'indicateur **Recovering** actif dans la barre d'état.

### Astuces

- Ne relancez pas tout à la main juste après un plantage — laissez d'abord quelques secondes à la récupération automatique.
- Si les plantages se répètent, ouvrez **Monitoring** pour voir la charge : vous faites peut-être tourner plus de comptes que cet ordinateur ne peut gérer.

![l'indicateur Recovering dans la barre d'état](../images/status-recovering.png)

---

# 6. Tâches courantes (« Je veux… »)

Réponses courtes à des objectifs courants. Pour des instructions complètes, suivez les liens vers la section 5.

## « Je veux ajouter de nouveaux comptes »

- **Quand en avez-vous besoin.** Vous avez de nouveaux comptes Steam.
- **Quoi faire.** Pour un compte, utilisez le bouton **Add Account** sur l'écran **Accounts**. Pour plusieurs à la fois, utilisez le bouton **Import** et l'assistant d'importation.
- **Ce qui se passe.** Les comptes apparaissent dans le tableau et sont prêts à être lancés (une fois qu'ils ont une sandbox).
- Plus : [5.1](#51-ajouter-un-seul-compte), [5.2](#52-importer-une-liste-de-comptes-depuis-un-fichier).

## « Je veux lancer Steam »

- **Quand en avez-vous besoin.** Vous avez besoin qu'un compte se connecte à Steam.
- **Quoi faire.** Sélectionnez le compte sur l'écran **Accounts** et cliquez sur **Start**.
- **Ce qui se passe.** L'application lance Steam dans la sandbox du compte et se connecte. Le statut passe de **Starting → Running**.

## « Je veux lancer CS2 »

- **Quand en avez-vous besoin.** Steam est déjà en cours d'exécution et vous devez lancer le jeu.
- **Quoi faire.** Lancer le compte avec **Start** le fait passer par tout le scénario, y compris le lancement de CS2 (si le workflow attribué le prévoit).
- **Ce qui se passe.** Après la connexion à Steam, l'application lance CS2. Vous pouvez suivre les étapes sur l'écran **Workflows**.

## « Je veux créer un lobby »

- **Quand en avez-vous besoin.** Vous devez réunir des comptes dans un lobby de jeu.
- **Quoi faire.** Constituez un groupe sur l'écran **Matchmaking** avec **Create Party** et ajoutez des membres.
- **Ce qui se passe.** L'application combine les comptes sélectionnés en un groupe et aide à les amener à un état cohérent (quorum).
- Plus : [5.5](#55-créer-un-groupe-et-le-mettre-en-file).

## « Je veux lancer le matchmaking »

- **Quand en avez-vous besoin.** Le groupe est constitué et prêt.
- **Quoi faire.** Sélectionnez le groupe et cliquez sur **Queue** (ou **Queue All** pour tous).
- **Ce qui se passe.** Les membres entrent dans la file ; vous voyez leurs positions et le temps d'attente.

## « Je veux arrêter toutes les sessions en cours »

- **Quand en avez-vous besoin.** Il est temps de terminer.
- **Quoi faire.** Sélectionnez les comptes (`Ctrl+A`) et cliquez sur **Stop**.
- **Ce qui se passe.** L'application ferme proprement les clients, et les statuts passent à **Stopped**.
- Plus : [5.4](#54-arrêter-tous-les-comptes-en-cours-dexécution).

## « Je veux récupérer après un plantage »

- **Quand en avez-vous besoin.** Un client a planté ou l'application a été redémarrée.
- **Quoi faire.** Laissez quelques secondes à la récupération automatique ; si nécessaire, cliquez sur **Restart** pour le compte planté.
- **Ce qui se passe.** L'application remet les comptes au travail.
- Plus : [5.7](#57-récupérer-après-un-plantage-ou-un-redémarrage-de-lapplication).

## « Je veux disposer les fenêtres à l'écran »

- **Quand en avez-vous besoin.** Vous voulez disposer proprement les fenêtres CS2 sur votre écran.
- **Quoi faire.** Sur l'écran **Layouts**, créez un préréglage et cliquez sur **Apply** / **Snap windows**.
- **Ce qui se passe.** Les fenêtres en cours se déplacent vers les endroits définis.

---

# 7. Référence des fonctionnalités

Cette section couvre les fonctionnalités individuelles avec leur but, leur emplacement et leurs particularités.

## 7.1. Recherche et filtres de comptes

**But.** Trouver rapidement les comptes qu'il vous faut dans une grande liste.

**Emplacement.** La barre d'outils de l'écran **Accounts** : le champ de recherche et le bouton **Filters**.

**Comment l'utiliser.**
- Tapez dans le champ de recherche (`Ctrl+F`). Vous pouvez chercher par éléments : `login:alex`, `status:running`, `rank:>=gold`, `tag:prime`.
- Cliquez sur **Filters** (`Ctrl+K` sur cet écran ouvre la fenêtre des filtres), définissez des conditions par statut, rang, sandbox, workflow ou tags, et enregistrez l'ensemble comme préréglage.

**Comportement attendu.** Le tableau n'affiche immédiatement que les comptes correspondants. Les filtres actifs apparaissent sous forme de puces sous la barre d'outils.

**Astuce.** Enregistrez les ensembles de conditions fréquemment utilisés comme préréglages — ils sont disponibles dans le menu déroulant de la barre d'outils.

## 7.2. Regroupement et configuration des colonnes

**But.** Organiser le tableau selon votre tâche.

**Emplacement.** La barre d'outils de l'écran **Accounts** : les boutons **Density**, **Columns** et **Group**.

**Comment l'utiliser.**
- **Group** permet de regrouper les comptes par statut, workflow, sandbox, tag ou rang. Les groupes affichent des compteurs, par exemple `Running (24)`.
- **Columns** — l'ensemble des colonnes visibles. Des ensembles prêts existent : **Operational**, **Identity**, **Audit**, **Compact**. Vous pouvez enregistrer le vôtre.
- **Density** — la hauteur des lignes (plus compacte ou plus aérée).

## 7.3. Menu contextuel du compte

**But.** Un accès rapide à toutes les actions d'un compte.

**Emplacement.** Cliquez droit sur une ligne de compte.

**Ce qui est disponible.** Éditer, copier l'identifiant ou le Steam ID, démarrer/arrêter/redémarrer, lier et délier une sandbox, attribuer un workflow, réauthentifier (**Re-auth**), tester la connexion (**Probe login now**), gérer les tags, exporter, cloner et supprimer.

## 7.4. Opérations groupées

**But.** Effectuer une action sur de nombreux comptes à la fois.

**Emplacement.** La barre d'outils de l'écran **Accounts** en mode sélection (quand au moins une ligne est cochée).

**Comment l'utiliser.** Cochez les comptes, puis cliquez sur le bouton voulu : **Start**, **Stop**, **Restart**, **Bind sandbox**, **Workflow…**, **Tag…**, **Export** ou **Delete**.

**Comportement attendu.** Une fenêtre apparaît avec une vue de progression par compte. Vous pouvez annuler l'opération pendant son exécution.

**Limitation.** Lors de la suppression de cinq comptes ou plus, l'application vous demande de confirmer en tapant le mot `DELETE`.

## 7.5. Exporter des comptes

**But.** Enregistrer les données des comptes dans un fichier.

**Emplacement.** Le bouton **Export** dans la barre d'outils ou le menu contextuel.

**Comment l'utiliser.** Choisissez un format : **TXT** (identifiant:motdepasse), **CSV** (tous les champs) ou **JSON** (l'enregistrement complet).

> **Avertissement.** Exporter les mots de passe requiert un consentement à part — l'application vous demande de cocher une case. Manipulez ces fichiers avec précaution.

## 7.6. Cloner un compte

**But.** Créer rapidement une copie d'un compte comme point de départ.

**Emplacement.** Menu contextuel de la ligne → **Clone…**.

**Comportement attendu.** Un formulaire s'ouvre avec les champs déjà remplis (l'identifiant devient `original_copy`), sauf le code Steam Guard et la liaison à la sandbox — que vous redéfinissez.

## 7.7. Workflows : démarrer, mettre en pause, arrêter

**But.** Gérer les scénarios automatisés.

**Emplacement.** L'écran **Workflows**.

**Comment l'utiliser.**

| Action | Ce qu'elle fait | Demande confirmation ? |
|---|---|---|
| **Start** | Exécute le scénario pour les comptes sélectionnés | Au lancement de plus de 10 comptes |
| **Pause** | Met en pause en douceur après l'étape en cours | Non |
| **Resume** | Continue depuis le point actuel | Non |
| **Stop** | Termine le scénario avec nettoyage | Oui |
| **Restart** | Arrête et recommence | Oui (pour une opération groupée) |
| **Skip step** | Marque l'étape en cours comme faite et avance | Oui |
| **Retry now** | Réessaie l'étape en cours immédiatement | Non |

**Astuce.** L'onglet **State Machine** dans le panneau de détails montre clairement à quelle étape en est un scénario.

## 7.8. Lier à une sandbox

**But.** Réserver un environnement isolé pour un compte, sans lequel il ne peut pas être lancé.

**Emplacement.** Menu contextuel → **Bind sandbox…**, ou l'opération groupée **Bind sandbox**.

**Comment l'utiliser.** Choisissez une méthode : en cycle (round-robin), remplir les vides d'abord, ou une sandbox précise.

**Limitation.** Un compte, une sandbox. Si la sandbox choisie est déjà utilisée, l'application propose de la libérer du compte précédent.

## 7.9. Dispositions de fenêtres

**But.** Disposer les fenêtres CS2 à l'aide d'une disposition prédéfinie.

**Emplacement.** L'écran **Layouts**.

**Comment l'utiliser.** Créez un préréglage, placez les emplacements sur le canevas des écrans, définissez les affectations et cliquez sur **Apply**.

**Astuce.** Le bouton **Revert layout** restaure les positions précédentes des fenêtres dans un délai d'une minute, au cas où une disposition n'aurait pas convenu.

## 7.10. Centre de notifications

**But.** Un endroit unique pour toutes les notifications de l'application.

**Emplacement.** Le badge de notifications dans la barre supérieure, ou `Ctrl+Shift+N`.

**Comment l'utiliser.** Le panneau s'ouvre à droite. Basculez entre les onglets **All**, **Errors**, **Warnings** et **Info**. Pour chaque entrée, vous pouvez aller à la source, réessayer ou ignorer. Le bouton **Clear all** vide la liste.

**Limitation.** Les 200 dernières entrées sont conservées ; les plus anciennes sont supprimées.

---

# 8. Statuts et indicateurs

Chaque statut a une couleur, un symbole et une étiquette. Voici ce que chacun signifie et s'il faut agir.

| Statut | Symbole | Ce que ça signifie | Action requise |
|---|---|---|---|
| **OK / Success** | ✓ (vert) | Compte en ligne, connexion réussie | Non |
| **Running** | ▶ (bleu) | Le compte ou le workflow est en cours | Non |
| **Starting** | ◐ (violet) | Lancement en cours, un état transitoire | Attendez la fin |
| **Queued** | ⏱ (gris) | En attente dans la file | Non |
| **Stopped** | ■ (gris) | Arrêté, inactif | Facultatif — vous pouvez le démarrer |
| **Paused** | ⏸ (ambre) | Scénario en pause | Cliquez sur **Resume** pour continuer |
| **Warning** | △ (ambre) | Une anomalie non critique | Regardez les détails ; souvent on peut continuer |
| **Error** | ✕ (rouge) | Une panne récupérable | Cliquez sur **Retry** ou cherchez la cause |
| **Crashed** | ☠ (rouge foncé, clignotant) | Le processus s'est terminé de façon inattendue | Cliquez sur **Restart** |
| **Match Found** | ◎ (vert, clignotant) | Une partie CS2 a été trouvée | Rien — l'application confirme la disponibilité automatiquement |
| **Desync** | ⛓ (orange) | Les membres du groupe sont désynchronisés | Lancez **Re-sync** |
| **Info** | ⓘ (bleu) | Un message neutre | Non |

**Indicateurs supplémentaires :**

- **Recovering** — un indicateur bleu dans la barre d'état au démarrage de l'application : les processus de la session précédente sont repris sous gestion. Attendez la fin.
- **Reattached** — un marqueur temporaire sur une ligne de compte : le processus a été repris avec succès après un redémarrage.
- **Frozen at HH:mm:ss** — sur l'écran **Monitoring**, signifie que l'affichage des données est figé (hors mode **Live**). Pour retrouver les données en direct, passez en **Live** ou désactivez **Freeze**.

**Comment voir les détails.** Survolez un symbole de statut pour obtenir une infobulle : depuis quand l'état dure, à quelle étape en est le compte et quel a été le dernier événement.

![exemples de statuts dans le tableau des comptes](../images/status-badges.png)

---

# 9. Notifications

L'application signale les événements de trois façons : les **toasts** (apparaissent dans le coin et disparaissent), la **barre d'état** (un résumé permanent en bas) et les **bannières intégrées** (liées à un écran précis).

## Toasts

Ils apparaissent dans le coin inférieur droit.

| Notification | Pourquoi elle apparaît | Ce que ça signifie | Quoi faire | Peut-on l'ignorer |
|---|---|---|---|---|
| **Saved** | Vous avez modifié un réglage | La modification a été enregistrée | Rien | Oui, disparaît d'elle-même |
| Réussite d'opération (vert) | Une action s'est terminée avec succès | Tout va bien | Rien | Oui, disparaît après ~5 secondes |
| Avertissement (ambre) | Une anomalie non critique a été détectée | Mérite un coup d'œil | Éventuellement voir les détails | Généralement oui, disparaît après ~10 secondes |
| Erreur (rouge) | Une opération a échoué | Une action est requise | Cliquez sur **View** ou **Retry** | Non, reste jusqu'à sa fermeture |
| Plantage (Crash) | Un client s'est fermé de façon inattendue | Un compte a planté | Cliquez sur **Restart** ou ouvrez le dump | Non, reste jusqu'à acquittement |

**Bon à savoir.**
- Survoler une notification arrête le minuteur de disparition automatique — vous pouvez la lire tranquillement.
- Les notifications identiques se regroupent en une seule avec un compteur, par exemple `… failed (×4)`.

## Barre d'état

Sur le côté droit de la barre d'état, la notification non lue la plus importante est affichée, par exemple `● 3 errors`. Cliquer dessus ouvre le centre de notifications.

## Bannières intégrées (Banners)

Elles apparaissent en haut d'un écran et s'appliquent à celui-ci dans son ensemble. Exemple : `⚠ Steam network degraded — 12 accounts retrying login`. Une bannière peut être fermée avec le bouton **Dismiss** si elle est non bloquante. Les bannières bloquantes (par exemple, quand un service est indisponible) restent jusqu'à la résolution du problème.

## Alertes sonores

Le son est désactivé par défaut. Vous pouvez l'activer pour des événements précis (par exemple, **Match found** ou **Crash**) dans **Settings → Notifications**. Un son pour **Match found** est pratique pour savoir qu'une partie a été trouvée sans regarder l'écran — l'acceptation de la partie, elle, se fait automatiquement.

![un toast d'erreur avec les boutons View et Retry](../images/notification-error-toast.png)

---

# 10. Erreurs et dépannage

Les erreurs pendant l'exploitation d'une ferme sont courantes, et l'application vous aide à les résoudre. Voici des situations courantes au format « Problème → Cause possible → Solution → Résultat attendu ».

## Impossible d'activer la licence

**Problème.** À la saisie de la clé, l'application ne vous laisse pas continuer.

| Message | Cause possible | Solution |
|---|---|---|
| « License key invalid » | La clé a été saisie avec une faute | Vérifiez l'orthographe. Il est plus simple de coller la clé avec **Paste from clipboard** |
| « Used on max devices » | La licence est déjà utilisée sur le nombre maximal d'appareils | Libérez la licence sur un autre appareil, puis réessayez. Le bouton **Manage devices** mène à la gestion des appareils |
| « Cannot reach license server » | Pas de connexion au serveur de licences | Vérifiez votre connexion internet et cliquez sur **Retry** |

**Résultat attendu.** Avec une clé correcte et une connexion au serveur, la fenêtre d'activation se ferme et le **Dashboard** s'ouvre.

## Un compte ne se lance pas

**Problème.** Vous avez cliqué sur **Start**, mais le compte ne passe pas à **Running**.

- **Cause possible.** Le compte n'est pas lié à une sandbox.
  **Solution.** Ouvrez le menu contextuel du compte → **Bind sandbox…** et attribuez une sandbox.
- **Cause possible.** Une réauthentification est requise (identifiants périmés) ; un marqueur « Reauth required » est à côté de la ligne.
  **Solution.** Menu contextuel → **Re-auth (Steam Guard)**.
- **Cause possible.** Steam a temporairement limité la fréquence des connexions.
  **Solution.** Attendez environ une minute et cliquez sur **Retry**.

**Résultat attendu.** Le statut passe de **Starting → Running**.

## Steam reste longtemps en Waiting/Starting

**Problème.** Le compte est bloqué à l'étape de connexion.

- **Cause possible.** Une connexion lente ou des problèmes temporaires du réseau Steam.
  **Solution.** Laissez un peu de temps. Si un statut **Error** apparaît, cliquez sur **Retry**. Si le réseau Steam est instable, une bannière d'avertissement apparaît en haut — attendez qu'il se rétablisse.

**Résultat attendu.** Le compte se connecte et passe à **Running**.

## Un client a planté

**Problème.** Le compte a reçu le statut **Crashed**.

- **Cause possible.** Le client CS2 ou Steam s'est terminé de façon inattendue.
  **Solution.** Dans la notification qui apparaît, cliquez sur **Restart**. La récupération est souvent déjà en cours automatiquement. Les détails du plantage sont sur l'écran **Monitoring**, dans le flux **Crashes & Warnings**.

**Résultat attendu.** Le compte redémarre et revient à **Running**.

## Un groupe est passé en Desync

**Problème.** Le groupe est à l'état **Desync** — les membres sont dans un état incohérent.

- **Cause possible.** Un membre a accepté une partie et un autre pas à temps, ou quelqu'un a quitté la file.
  **Solution.** Cliquez sur **Re-sync** pour mettre la file en pause et attendre la cohérence. Si un compte pose problème, retirez-le avec **Drop member** et remettez les autres en file.

**Résultat attendu.** Le groupe revient à l'état **Quorum** et est prêt à être remis en file.

## Un lancement groupé s'est terminé avec des erreurs

**Problème.** Après un **Start** groupé, certains comptes ne se sont pas lancés.

- **Solution.** Dans le résumé, cliquez sur **Filter to failed** — le tableau n'affiche que les comptes problématiques. Résolvez chacun selon les causes ci-dessus et relancez.

**Résultat attendu.** Une fois les causes résolues, un **Start** répété fait passer les comptes à **Running**.

## Les données d'un écran ne se chargent pas

**Problème.** Au lieu du contenu de l'écran, il y a une bannière ou un message indiquant qu'un service est indisponible.

- **Cause possible.** Un service en arrière-plan est temporairement indisponible.
  **Solution.** Cliquez sur **Retry**. Si ça n'aide pas, cliquez sur **Open logs** pour voir les détails, ou redémarrez l'application.

**Résultat attendu.** L'écran se charge et affiche des données à jour.

## L'application signale un processus orphelin

**Problème.** Dans le centre de notifications, un message comme « Orphan process … — Adopt or Kill? ».

- **Cause possible.** Un processus de la session précédente est resté sans pouvoir être lié automatiquement à un compte.
  **Solution.** Choisissez **Adopt** (le reprendre sous gestion) si le processus est nécessaire, ou **Kill** (le terminer) sinon.

**Résultat attendu.** La liste des processus est remise en ordre.

## L'ordinateur est lent et les plantages augmentent

**Problème.** Instabilité générale, pannes fréquentes.

- **Cause possible.** Plus de comptes sont en cours d'exécution que l'ordinateur ne peut gérer.
  **Solution.** Ouvrez **Monitoring** et regardez **CPU** et **RAM**. Si les valeurs sont proches de leurs limites, arrêtez quelques comptes avec **Stop**.

**Résultat attendu.** La charge baisse et le fonctionnement se stabilise.

> **Codes d'erreur.** Les détails des erreurs comportent un code court comme `[E-1042]`. Vous pouvez le copier et l'utiliser en contactant le support. Une référence complète des codes est disponible via **Help → Error reference**.

![un exemple d'écran d'erreur avec les boutons Retry / Open logs](../images/error-screen.png)

---

# 11. Bonnes pratiques

## Préparer les comptes

- Ajoutez les comptes en liste via **Import** — c'est plus rapide et il y a moins de fautes de frappe.
- Laissez l'attribution de sandbox sur **Auto-assign**, sauf si vous avez besoin d'une liaison précise.
- Utilisez les **Tags** pour regrouper les comptes et les filtrer rapidement.

## Lancer beaucoup de comptes

- Lancez par lots : commencez par un petit groupe, confirmez la stabilité, puis ajoutez-en d'autres.
- Gardez le **Dashboard** ou **Monitoring** ouvert pour surveiller la charge en temps réel.
- Visez les 4–10 comptes CS2 recommandés à la fois ; vous pouvez en faire tourner plus sur un PC puissant et moins sur des machines plus faibles.

## Travailler avec les dispositions

- Préparez plusieurs préréglages à l'avance pour différentes situations (par exemple, « 4-stack », « un en focus »).
- Si une disposition tourne mal, utilisez **Revert layout** aussitôt, tant que la fenêtre d'annulation d'une minute est active.

## Arrêter en toute sécurité

- Arrêtez les comptes avec le bouton **Stop** (un arrêt en douceur) plutôt que de fermer les fenêtres à la main.
- Avant de quitter l'application, arrêtez les comptes actifs. Si vous tentez de fermer l'application alors que des scénarios sont en cours, elle vous avertit.

## Éviter les interruptions

- Avant la mise en file, assurez-vous que le groupe est à l'état **Quorum**.
- Surveillez les bannières sur l'état du réseau Steam — quand il est instable, mieux vaut attendre.

## Maintenir un fonctionnement stable

- Consultez le **Dashboard** régulièrement — il montre l'état général en quelques secondes.
- Gardez le nombre de comptes en cours d'exécution simultanée dans les capacités de votre ordinateur.
- Laissez la récupération automatique travailler quelques secondes avant d'intervenir à la main.

---

# 12. Foire aux questions

**Pourquoi je n'arrive pas à lancer un compte ?**
Le plus probable est que le compte n'est pas lié à une sandbox — sans elle, il ne peut pas se lancer. Liez-en une via le menu contextuel → **Bind sandbox…**. Un lancement peut aussi être bloqué par le besoin de se réauthentifier (un marqueur « Reauth required ») — dans ce cas, lancez **Re-auth**.

**Pourquoi Steam reste-t-il longtemps en attente ?**
C'est généralement une connexion lente ou des délais temporaires du réseau Steam. Laissez un peu de temps. Si un statut **Error** apparaît, cliquez sur **Retry**.

**Comment redémarrer un workflow ?**
Sélectionnez les comptes ou instances voulus et cliquez sur **Restart** (ou `Ctrl+Shift+R`). Pour une opération groupée, l'application demande confirmation.

**Que se passe-t-il si l'application se ferme ?**
Vos comptes et réglages sont enregistrés. Au lancement suivant, l'application tente de reprendre les processus de la session précédente sous gestion — un indicateur **Recovering** apparaît dans la barre d'état. Si des scénarios étaient actifs à la fermeture, l'application vous avertit à l'avance.

**Comment savoir que tout fonctionne ?**
Consultez la barre d'état en bas et le **Dashboard**. Signes d'un fonctionnement normal : comptes au statut **Running**, aucun marqueur rouge dans la carte **Errors** ou le tableau **Failures & Crashes**, et charge **CPU** et **RAM** dans des plages normales.

**Où sont stockés mes mots de passe ?**
Uniquement sur votre ordinateur. Ils sont chiffrés avec la protection intégrée de Windows, ne sont jamais enregistrés en clair et ne sont jamais envoyés ailleurs.

**FarmPanel joue-t-il à ma place ?**
Non. Ce n'est ni un bot ni un autofarm. L'application gère le lancement, la surveillance, le montage des lobbies et la récupération, tandis que toutes les actions en jeu sont effectuées par vous.

**Dois-je saisir la clé de licence à chaque fois ?**
Non. La clé est saisie une seule fois, lors de la première activation. Ensuite, l'application s'ouvre directement sur le **Dashboard**.

**Comment trouver rapidement une action si j'ai oublié où est le bouton ?**
Appuyez sur `Ctrl+K` pour ouvrir la palette de commandes. Commencez à taper le nom d'une action, d'un écran ou d'un identifiant de compte, et choisissez celui qu'il vous faut dans la liste.

**Puis-je déplacer le monitoring sur un second écran ?**
Oui. Sur l'écran **Monitoring**, cliquez sur le bouton de détachement — l'écran s'ouvre dans une fenêtre séparée que vous pouvez placer sur un second écran. Sa position est mémorisée.

**Comment réinitialiser les réglages par défaut ?**
Dans **Settings → Advanced** se trouve **Reset to defaults**. Pour se prémunir des clics accidentels, l'application vous demande de confirmer en tapant un texte.

---

*Fin du guide de l'utilisateur de FarmPanel.*
