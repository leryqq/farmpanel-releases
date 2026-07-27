# Installation de Sandboxie-Plus

**Guide d'installation pas à pas pour Windows**

Version du document : 1.0 · Version de Sandboxie-Plus : **1.17.5**

🌐 [English](INSTALL-SANDBOXIE-PLUS.md) · [Русский](INSTALL-SANDBOXIE-PLUS.ru.md) · [Español](INSTALL-SANDBOXIE-PLUS.es.md) · [Português](INSTALL-SANDBOXIE-PLUS.pt.md) · **Français** · [Türkçe](INSTALL-SANDBOXIE-PLUS.tr.md) · [Bahasa Indonesia](INSTALL-SANDBOXIE-PLUS.id.md) · [Tiếng Việt](INSTALL-SANDBOXIE-PLUS.vi.md) · [हिन्दी](INSTALL-SANDBOXIE-PLUS.hi.md) · [中文](INSTALL-SANDBOXIE-PLUS.zh.md) · [العربية](INSTALL-SANDBOXIE-PLUS.ar.md)

---

FarmPanel garde chaque compte dans sa propre **sandbox** — un environnement isolé où Steam et CS2 ne se mélangent pas avec les autres comptes. Cet isolement est assuré par un programme gratuit appelé **Sandboxie-Plus**. Vous l'installez une fois, avant de commencer à lancer des comptes dans FarmPanel.

Ce guide vous accompagne dans l'installation pas à pas. Rien de compliqué — cela prend quelques minutes.

> **En bref.** Téléchargez l'installeur de **Sandboxie-Plus 1.17.5** → lancez-le → acceptez les réglages par défaut → autorisez l'installation (des droits d'administrateur sont requis) → c'est terminé.

> **Important.** Contrairement à FarmPanel, Sandboxie-Plus **requiert des droits d'administrateur** pour s'installer — c'est normal, car le programme s'intègre en profondeur à Windows pour isoler les applications de façon fiable.

## Sommaire

1. [Ce dont vous aurez besoin](#1-ce-dont-vous-aurez-besoin)
2. [Étape 1. Téléchargez l'installeur](#étape-1-téléchargez-linstalleur)
3. [Étape 2. Lancez l'installation](#étape-2-lancez-linstallation)
4. [Étape 3. Parcourez l'assistant d'installation](#étape-3-parcourez-lassistant-dinstallation)
5. [Étape 4. Premier lancement de Sandboxie-Plus](#étape-4-premier-lancement-de-sandboxie-plus)
6. [Étape 5. Vérifiez que tout fonctionne](#étape-5-vérifiez-que-tout-fonctionne)
7. [Étape 6. Reliez-le à FarmPanel](#étape-6-reliez-le-à-farmpanel)
8. [Comment désinstaller Sandboxie-Plus](#comment-désinstaller-sandboxie-plus)
9. [Dépannage](#dépannage)
10. [Foire aux questions](#foire-aux-questions)

---

# 1. Ce dont vous aurez besoin

- **Un ordinateur sous Windows 10 ou 11** (64 bits).
- **Des droits d'administrateur** sur cet ordinateur (une invite apparaît pendant l'installation — vous devez cliquer sur **Oui**).
- **Une connexion internet** — pour télécharger le programme.
- **Environ 5 minutes de votre temps.**

> Sandboxie-Plus est gratuit. Quelques fonctions supplémentaires sont réservées à ceux qui soutiennent le projet, mais vous **n'en avez pas besoin** pour utiliser FarmPanel — la version gratuite habituelle suffit.

---

# Étape 1. Téléchargez l'installeur

1. Ouvrez la page officielle de la version dont vous avez besoin :
   **[Sandboxie-Plus 1.17.5 sur GitHub](https://github.com/sandboxie-plus/Sandboxie/releases/tag/v1.17.5)**
2. Faites défiler jusqu'à la section **Assets**.
3. Repérez et téléchargez le fichier nommé quelque chose comme **`Sandboxie-Plus-x64-v1.17.5.exe`** — c'est l'installeur pour un Windows 64 bits classique.

**Comment choisir le bon fichier :**

| Fichier | Pour qui |
|---|---|
| **`Sandboxie-Plus-x64-v1.17.5.exe`** | **La plupart des utilisateurs** — un Windows classique sur processeur Intel ou AMD. Téléchargez celui-ci. |
| `Sandboxie-Plus-arm64-v1.17.5.exe` | Uniquement pour les ordinateurs à processeur ARM (rare). |
| `Sandboxie-Classic-…` | La variante d'interface ancienne. **Inutile** pour FarmPanel — choisissez **Plus**. |
| Fichiers `.7z` | Versions portables pour utilisateurs avancés. **Inutiles** pour l'installation. |

**Ce qui se passe ensuite.** Le fichier apparaît dans votre dossier **Téléchargements**.

> **Astuce.** Ne téléchargez l'installeur que depuis la page GitHub officielle indiquée ci-dessus. Vous obtenez ainsi la version authentique et vérifiée.

![la page de release 1.17.5 avec la section Assets](../images/sandboxie/github-release-assets.png)

---

# Étape 2. Lancez l'installation

1. Ouvrez votre dossier **Téléchargements** et double-cliquez sur le fichier téléchargé **`Sandboxie-Plus-x64-v1.17.5.exe`**.
2. Windows affiche l'invite **« Voulez-vous autoriser cette application à apporter des modifications à votre appareil ? »** — cliquez sur **Oui**. C'est l'invite de droits d'administrateur ; sans elle, Sandboxie-Plus ne peut pas être installé.

> **Si une fenêtre bleue SmartScreen apparaît** (« Windows a protégé votre ordinateur ») — cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**. C'est un avertissement courant pour les programmes téléchargés, pas une erreur.

**Ce qui se passe ensuite.** La fenêtre de l'assistant d'installation s'ouvre.

---

# Étape 3. Parcourez l'assistant d'installation

L'assistant d'installation vous guide à travers quelques écrans simples. Dans la plupart des cas, il suffit de tout laisser aux valeurs par défaut et de cliquer sur **Next**.

1. **Sélection de la langue.** Si une fenêtre de sélection de langue apparaît, choisissez le français (ou votre langue) et cliquez sur **OK**.
2. **Contrat de licence.** Lisez-le et cliquez sur **I Agree** ou **Next**.
3. **Dossier d'installation.** Laissez le dossier par défaut (`C:\Program Files\Sandboxie-Plus`) et cliquez sur **Next**. Il n'y a pas besoin de le modifier.
4. **Options d'installation.** Rien à changer — cliquez simplement sur **Next** / **Install**.
5. Attendez la fin. L'installation prend moins d'une minute.
6. Sur le dernier écran, cliquez sur **Finish**. Laissez la case « lancer Sandboxie-Plus » cochée, s'il y en a une.

**Ce qui se passe ensuite.** Sandboxie-Plus est installé et son icône apparaît sur votre bureau et dans le menu Démarrer. Le programme se lance généralement juste après l'installation.

> **Faut-il redémarrer ?** En général non. Mais si l'assistant vous demande de redémarrer l'ordinateur, faites-le, afin que l'isolement fonctionne correctement.

![l'écran de l'assistant d'installation avec le dossier par défaut](../images/sandboxie/installer-wizard.png)

---

# Étape 4. Premier lancement de Sandboxie-Plus

La première fois que vous ouvrez Sandboxie-Plus, il affiche un **Setup Wizard** (assistant de configuration). Parcourez-le pas à pas — reproduisez simplement ce qui est décrit ci-dessous.

Si une fenêtre de **sélection de la langue de l'interface** apparaît avant l'assistant, choisissez votre langue et cliquez sur **OK**.

L'assistant vous guide ensuite à travers plusieurs écrans.

### Écran 1 — Introduction

Sélectionnez **« Personally, for private non-commercial use »** (Personnellement, pour un usage privé non commercial) et cliquez sur **Next**.

![Setup Wizard — l'écran Introduction avec « Personally, for private non-commercial use » sélectionné](../images/sandboxie/wizard-1-introduction.png)

### Écran 2 — Support certificate

Laissez le champ **vide** et cliquez sur **Next**. Un certificat n'est pas nécessaire pour utiliser FarmPanel.

![Setup Wizard — l'écran Support certificate avec le champ vide](../images/sandboxie/wizard-2-support-certificate.png)

### Écran 3 — Configure UI

Laissez les valeurs **par défaut** (**Advanced UI for experts** est déjà sélectionné) et cliquez sur **Next**.

![Setup Wizard — l'écran de configuration de l'interface avec les valeurs par défaut](../images/sandboxie/wizard-3-ui-configuration.png)

### Écran 4 — Shell integration

**Décochez toutes les cases** et cliquez sur **Next**.

![Setup Wizard — l'écran Shell integration avec toutes les cases décochées](../images/sandboxie/wizard-4-shell-integration.png)

### Écran 5 — Updater

**Décochez toutes les cases** et cliquez sur **Next**.

![Setup Wizard — l'écran Updater avec toutes les cases décochées](../images/sandboxie/wizard-5-updater.png)

### Écran 6 — Complete

Cliquez sur **Finish** pour appliquer les réglages et fermer l'assistant.

![Setup Wizard — l'écran final avec le bouton Finish](../images/sandboxie/wizard-6-complete.png)

> **Astuce.** En cas de doute sur un écran, décochez les cases et cliquez sur **Next**. FarmPanel n'a pas besoin des intégrations supplémentaires ni des rappels de mise à jour.

**Ce qui se passe ensuite.** La fenêtre principale de Sandboxie-Plus s'ouvre — la liste des sandboxes et le panneau de contrôle.

![la fenêtre principale de Sandboxie-Plus après le premier lancement](../images/sandboxie/main-window.png)

---

# Étape 5. Vérifiez que tout fonctionne

Assurez-vous que Sandboxie-Plus est correctement installé :

1. Ouvrez Sandboxie-Plus (l'icône sur le bureau ou dans le menu Démarrer).
2. La fenêtre principale affiche une liste de sandboxes — il y a généralement une sandbox par défaut nommée quelque chose comme **DefaultBox**.
3. Le programme s'ouvre et n'affiche aucun message d'erreur.

Si tout cela est en place — **Sandboxie-Plus est installé et prêt à l'emploi**.

---

# Étape 6. Reliez-le à FarmPanel

Une fois Sandboxie-Plus installé, FarmPanel peut l'utiliser pour isoler les comptes.

1. Ouvrez **FarmPanel**.
2. Allez dans **Settings → Sandboxes**.
3. Vérifiez que le chemin du dossier des sandboxes est défini. Si le champ est vide, choisissez un dossier pour les sandboxes ; s'il est déjà rempli, il n'y a rien à changer.
4. Revenez à l'écran **Accounts**. Désormais, en ajoutant des comptes, vous pouvez choisir comment les sandboxes sont attribuées (**Auto-assign** et autres), et les comptes peuvent être lancés.

> **Comment cela se relie.** Dans FarmPanel, chaque compte doit être lié à une sandbox, sinon il ne peut pas être lancé. C'est Sandboxie-Plus qui crée et entretient ces environnements isolés « en coulisses ». Pour en savoir plus sur les sandboxes et le lancement des comptes, consultez le [Guide de l'utilisateur de FarmPanel](../user-guide/USER-GUIDE.fr.md).

**Signe de réussite.** Un compte dans FarmPanel se lance et passe au statut **Running** — ce qui signifie que l'isolement via Sandboxie-Plus fonctionne.

---

# Comment désinstaller Sandboxie-Plus

Si vous devez supprimer le programme :

1. D'abord, fermez tous les programmes en cours d'exécution dans les sandboxes (dans FarmPanel, arrêtez les comptes avec **Stop**).
2. Ouvrez **Paramètres de Windows** → **Applications** → **Applications installées**
   (ou « Panneau de configuration » → « Programmes et fonctionnalités »).
3. Trouvez **Sandboxie-Plus** dans la liste.
4. Cliquez sur **Désinstaller** et confirmez. Des droits d'administrateur sont également requis pour désinstaller.

> **Remarque.** Une fois Sandboxie-Plus supprimé, FarmPanel ne peut plus lancer de comptes tant que le programme n'est pas réinstallé.

---

# Dépannage

## Windows refuse l'installation — pas de droits d'administrateur

**Cause.** Sandboxie-Plus requiert strictement des droits d'administrateur.

**Solution.** Connectez-vous avec un compte disposant de droits d'administrateur, ou demandez à l'administrateur de l'ordinateur d'installer le programme. Quand l'invite **« Voulez-vous autoriser les modifications ? »** apparaît, cliquez sur **Oui**.

## Une fenêtre SmartScreen est apparue

**Cause.** Windows avertit à propos des programmes téléchargés récemment. Ce n'est pas une erreur.

**Solution.** Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.

## Un antivirus a bloqué l'installeur

**Cause.** Certains antivirus sont prudents avec les logiciels qui s'intègrent au système.

**Solution.**
1. Vérifiez que vous avez téléchargé le fichier depuis la page GitHub officielle (le lien est à l'[Étape 1](#étape-1-téléchargez-linstalleur)).
2. Si nécessaire, ajoutez temporairement le fichier aux exclusions de votre antivirus et téléchargez-le de nouveau.

## Mauvais fichier téléchargé

**Cause.** Il y a plusieurs fichiers sur la page de release.

**Solution.** Pour un Windows classique, il vous faut le fichier nommé **`Sandboxie-Plus-x64-v1.17.5.exe`**. Ne prenez pas les variantes **arm64**, **Classic** ou **.7z**. Revenez à l'[Étape 1](#étape-1-téléchargez-linstalleur) et téléchargez le bon fichier.

## FarmPanel ne lance pas les comptes après l'installation

**Solution.**
1. Vérifiez que Sandboxie-Plus est installé et s'ouvre (voir l'[Étape 5](#étape-5-vérifiez-que-tout-fonctionne)).
2. Dans FarmPanel, ouvrez **Settings → Sandboxes** et vérifiez que le chemin du dossier des sandboxes est défini.
3. Redémarrez FarmPanel.
4. Si le problème persiste, contactez le support (voir [Foire aux questions](#foire-aux-questions)).

## L'ordinateur demande un redémarrage après l'installation

**Solution.** Redémarrez l'ordinateur — cela termine l'installation et active l'isolement. Après le redémarrage, rouvrez FarmPanel.

---

# Foire aux questions

**L'installation de Sandboxie-Plus est-elle obligatoire ?**
Oui, si vous voulez lancer des comptes dans FarmPanel. C'est Sandboxie-Plus qui assure l'isolement de chaque compte dans un environnement distinct.

**Sandboxie-Plus est-il payant ?**
Non, la version de base est gratuite et suffit pour utiliser FarmPanel. Des fonctions supplémentaires sont réservées à ceux qui soutiennent le projet, mais elles ne sont pas requises.

**Pourquoi l'installation requiert-elle des droits d'administrateur alors que FarmPanel non ?**
Sandboxie-Plus s'intègre en profondeur à Windows pour isoler les programmes de façon fiable, il a donc besoin de droits d'administrateur. FarmPanel, lui, s'installe uniquement pour votre compte d'utilisateur et n'en a pas besoin.

**Dois-je configurer les sandboxes moi-même ?**
Non. Installez simplement Sandboxie-Plus. FarmPanel crée et configure les sandboxes des comptes automatiquement.

**Ai-je besoin d'un certificat de soutien (supporter certificate) ?**
Non. Vous pouvez passer cet écran au premier lancement. Il n'est pas nécessaire pour FarmPanel.

**Quelle version exacte dois-je installer ?**
La version **1.17.5** — le lien est à l'[Étape 1](#étape-1-téléchargez-linstalleur). Installez exactement celle-ci pour une compatibilité prévisible avec FarmPanel.

**Où m'adresser si quelque chose n'a pas fonctionné ?**
Contactez le support de FarmPanel sur Telegram : [t.me/farmpanel_fr](https://t.me/farmpanel_fr). Décrivez le problème et joignez le texte du message d'erreur si vous en avez un.

---

Après avoir installé Sandboxie-Plus, revenez au [guide d'installation de FarmPanel](../install-guide/INSTALL-GUIDE.fr.md) ou passez directement au [Guide de l'utilisateur](../user-guide/USER-GUIDE.fr.md) pour ajouter des comptes et lancer votre première ferme.

*Fin du guide d'installation de Sandboxie-Plus.*
