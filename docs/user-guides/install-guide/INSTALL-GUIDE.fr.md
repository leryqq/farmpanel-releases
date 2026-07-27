# Installation de FarmPanel

**Guide d'installation pas à pas pour Windows**

Version du document : 1.0

🌐 [English](INSTALL-GUIDE.md) · [Русский](INSTALL-GUIDE.ru.md) · [Español](INSTALL-GUIDE.es.md) · [Português](INSTALL-GUIDE.pt.md) · **Français** · [Türkçe](INSTALL-GUIDE.tr.md) · [Bahasa Indonesia](INSTALL-GUIDE.id.md) · [Tiếng Việt](INSTALL-GUIDE.vi.md) · [हिन्दी](INSTALL-GUIDE.hi.md) · [中文](INSTALL-GUIDE.zh.md) · [العربية](INSTALL-GUIDE.ar.md)

---

Ce guide vous accompagne du téléchargement du programme jusqu'au premier lancement. Suivez les étapes dans l'ordre — rien de compliqué, cela ne prend que quelques minutes.

> **En bref.** Téléchargez `Setup.exe` → lancez-le → activez votre licence avec la clé → c'est terminé. Aucun droit d'administrateur n'est requis, et rien d'autre n'a besoin d'être installé séparément.

## Sommaire

1. [Ce dont vous aurez besoin](#1-ce-dont-vous-aurez-besoin)
2. [Configuration requise](#2-configuration-requise)
3. [Étape 1. Téléchargez l'installeur](#étape-1-téléchargez-linstalleur)
4. [Étape 2. Lancez l'installation](#étape-2-lancez-linstallation)
5. [Étape 3. Ouvrez l'application](#étape-3-ouvrez-lapplication)
6. [Étape 4. Configuration initiale — emplacements de Steam et de Sandboxie](#étape-4-configuration-initiale--emplacements-de-steam-et-de-sandboxie)
7. [Étape 5. Activez votre licence](#étape-5-activez-votre-licence)
8. [Étape 6. Vérifiez que tout fonctionne](#étape-6-vérifiez-que-tout-fonctionne)
9. [Mises à jour](#mises-à-jour)
10. [Comment désinstaller](#comment-désinstaller)
11. [Dépannage de l'installation](#dépannage-de-linstallation)
12. [Foire aux questions](#foire-aux-questions)

---

# 1. Ce dont vous aurez besoin

- **Un ordinateur sous Windows 10 ou 11** (64 bits).
- **Une connexion internet** — pour télécharger le programme et activer la licence.
- **Une clé de licence** — vous la recevez avec votre achat. Elle se présente ainsi :
  `XXXX-XXXX-XXXX-XXXX-XXXX` (cinq groupes de quatre caractères).
- **Environ 10 minutes de votre temps.**

> Vous **n'avez pas besoin** d'installer quoi que ce soit d'autre séparément (comme .NET) — tout le nécessaire est déjà inclus dans l'installeur.

---

# 2. Configuration requise

| Élément | Minimum | Recommandé |
|---|---|---|
| Système d'exploitation | Windows 10 ou 11 (64 bits) | Windows 10 / 11 (64 bits) |
| Mémoire | 8 Go | 32 Go |
| Disque | N'importe lequel | SSD |
| Espace libre | environ 500 Mo | 1 Go ou plus |
| Comptes simultanés | 2 | 4–10 comptes CS2 |
| Résolution d'écran | au moins 1280 pixels de large | Full HD (1920×1080) ou plus |

Si votre ordinateur atteint le minimum, l'application fonctionnera. Plus votre ordinateur est puissant, plus vous pouvez faire tourner de comptes en même temps.

---

# Étape 1. Téléchargez l'installeur

1. Ouvrez la page de téléchargement officielle :
   **[Télécharger pour Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   (vous trouverez aussi le lien de téléchargement sur le site [farmpanel.cc](https://farmpanel.cc)).
2. Repérez le fichier nommé quelque chose comme **`Setup.exe`** (dans la section **Assets** si vous êtes sur la page des releases) et cliquez dessus pour le télécharger.
3. Attendez la fin du téléchargement. Le fichier fait environ 50–80 Mo, donc sur une connexion rapide cela prend moins d'une minute.

**Ce qui se passe ensuite.** Le fichier `Setup.exe` apparaît dans votre dossier **Téléchargements**.

> **Astuce.** Ne téléchargez l'installeur que depuis la page officielle indiquée ci-dessus. Vous obtenez ainsi la version authentique et vérifiée du programme.

![la page de téléchargement avec le fichier Setup.exe](../images/install-download-page.png)

---

# Étape 2. Lancez l'installation

1. Ouvrez votre dossier **Téléchargements** et double-cliquez sur le fichier **`Setup.exe`**.
2. L'installation démarre automatiquement. **Les droits d'administrateur ne sont pas requis** — l'application s'installe uniquement pour votre compte d'utilisateur.
3. Attendez la fin. Cela prend généralement moins d'une minute. Il n'y a pas de boutons « Suivant » à cliquer — l'installeur fait tout tout seul.

**Ce qui se passe ensuite.** L'application est installée et une icône **FarmPanel** apparaît sur votre bureau et dans le menu Démarrer. L'application s'ouvre souvent juste après l'installation.

> **Si une fenêtre bleue « Windows a protégé votre ordinateur » (SmartScreen) apparaît** — c'est un avertissement courant pour les nouveaux programmes, pas une erreur. Que faire :
> 1. Cliquez sur **Informations complémentaires**.
> 2. Cliquez sur le bouton **Exécuter quand même** qui apparaît.
>
> L'installation continue normalement. Plus de détails dans [Dépannage de l'installation](#dépannage-de-linstallation).

---

# Étape 3. Ouvrez l'application

Si l'application ne s'est pas ouverte d'elle-même, double-cliquez sur l'icône **FarmPanel** de votre bureau ou trouvez-la dans le menu Démarrer.

**Ce que vous verrez.** Au tout premier lancement, l'application vous guide à travers une brève configuration initiale et l'activation de la licence — ce sont les prochaines étapes.

---

# Étape 4. Configuration initiale — emplacements de Steam et de Sandboxie

Au premier lancement, l'application vous demande d'indiquer où se trouvent **Steam** et **Sandboxie-Plus** sur votre ordinateur. Sans ces chemins, l'application ne peut pas lancer ni isoler les comptes.

> **Important.** Sandboxie-Plus doit déjà être installé à ce stade. Si ce n'est pas encore fait, consultez le guide séparé [Installation de Sandboxie-Plus](../install-sandboxie-plus/INSTALL-SANDBOXIE-PLUS.fr.md).

1. **Emplacement de Steam.** Cliquez sur le bouton de sélection de dossier (**Browse…** / icône de dossier) à côté du champ Steam et sélectionnez le dossier où Steam est installé. Il s'agit généralement de `C:\Program Files (x86)\Steam`.
2. **Emplacement de Sandboxie.** Cliquez sur le bouton de sélection de dossier à côté du champ Sandboxie et sélectionnez le dossier où Sandboxie-Plus est installé. Il s'agit généralement de `C:\Program Files\Sandboxie-Plus`.
3. Confirmez la configuration (le bouton **Save** / **Continue**).

**Ce qui se passe ensuite.** L'application retient ces chemins et les utilise chaque fois qu'elle lance des comptes.

**Signe de réussite.** Les deux chemins sont définis et l'application n'affiche aucun avertissement indiquant que Steam ou Sandboxie sont introuvables.

> **Astuce.** Vous pouvez modifier ces chemins plus tard, à tout moment, dans **Settings** (Paramètres).

![configuration initiale — emplacements de Steam et de Sandboxie](../images/initial-setup-locations.png)

---

# Étape 5. Activez votre licence

L'activation n'est nécessaire qu'une seule fois — au premier lancement.

1. Saisissez ou collez votre clé de licence dans le champ de saisie.
   Pour la coller depuis le presse-papiers, cliquez sur **Paste from clipboard** (Coller depuis le presse-papiers).
2. L'application vérifie le format de la clé à mesure que vous tapez. Quand le format est correct, le bouton d'activation devient disponible.
3. Cliquez sur **Activate** (Activer).

**Ce qui se passe ensuite.** L'application contacte le serveur et vérifie la clé. Cela prend quelques secondes — vous verrez l'état **Activating** (Activation en cours).

**Signe de réussite.** La fenêtre d'activation se ferme et l'écran principal de l'application — **Dashboard** — s'ouvre. Votre licence est active. Vous n'aurez pas à saisir la clé de nouveau lors des prochains lancements.

> **Si la clé n'est pas acceptée** — vérifiez que vous l'avez saisie sans faute (il est plus simple de la coller avec **Paste from clipboard**) et que vous avez internet. Les messages courants sont traités dans [Dépannage de l'installation](#dépannage-de-linstallation).

![la fenêtre d'activation de la licence](../images/license-activation.png)

---

# Étape 6. Vérifiez que tout fonctionne

Après l'activation, vous arrivez sur l'écran principal. Vérifiez que l'installation a réussi :

1. En haut de la fenêtre, vous voyez la **barre latérale** avec les sections (**Dashboard**, **Accounts**, **Workflows** et d'autres).
2. En bas de la fenêtre se trouve la **barre d'état** — une fine bande avec un résumé et la version de l'application (par exemple, `v1.0.1`).
3. L'application s'ouvre et passe d'une section à l'autre sans erreur.

Si tout cela est en place — **l'installation est terminée et vous pouvez commencer à utiliser l'application**.

**La suite.** Ajoutez vos comptes Steam et lancez votre première ferme. Pour des instructions pas à pas, consultez le [Guide de l'utilisateur](../user-guide/USER-GUIDE.fr.md) (la section « Flux de travail principaux »).

![l'écran principal après l'installation](../images/dashboard-overview.png)

---

# Mises à jour

FarmPanel se met à jour **automatiquement** — vous n'avez rien à télécharger à la main.

- L'application vérifie s'il existe de nouvelles versions au démarrage et de temps à autre pendant l'utilisation.
- Une nouvelle version est téléchargée discrètement, en arrière-plan, sans interrompre votre travail.
- La mise à jour est appliquée au prochain redémarrage de l'application.

**Ce que vous faites.** Rien de particulier. Fermez et rouvrez l'application de temps en temps, et la dernière version sera installée. La version actuelle est toujours visible dans la barre d'état, en bas, et dans **Settings → About** (Paramètres → À propos).

---

# Comment désinstaller

Si vous devez supprimer FarmPanel :

1. Ouvrez **Paramètres de Windows** → **Applications** → **Applications installées**
   (ou « Panneau de configuration » → « Programmes et fonctionnalités »).
2. Trouvez **FarmPanel** dans la liste.
3. Cliquez sur **Désinstaller** et confirmez.

**Ce qui se passe ensuite.** L'application est supprimée de votre ordinateur. Aucun droit d'administrateur n'est requis pour la désinstaller.

---

# Dépannage de l'installation

Voici des situations courantes et la marche à suivre.

## Une fenêtre « Windows a protégé votre ordinateur » (SmartScreen) est apparue

**Cause.** Windows affiche cet avertissement pour les programmes téléchargés récemment et que le système ne connaît pas encore bien. Cela ne signifie pas qu'il y a un problème avec le fichier.

**Solution.**
1. Cliquez sur **Informations complémentaires**.
2. Cliquez sur **Exécuter quand même**.

L'installation continue. S'il n'y a pas de bouton **Informations complémentaires**, vérifiez que vous avez téléchargé le fichier depuis la page officielle et réessayez.

## Un antivirus a bloqué ou supprimé le fichier

**Cause.** Certains antivirus traitent les nouveaux installeurs avec prudence et peuvent déclencher une fausse alerte.

**Solution.**
1. Vérifiez que vous avez téléchargé `Setup.exe` depuis la page officielle (le lien est à l'[Étape 1](#étape-1-téléchargez-linstalleur)).
2. Si nécessaire, ajoutez le fichier aux exclusions de votre antivirus et téléchargez-le de nouveau.
3. En cas de doute, contactez le support (voir [Foire aux questions](#foire-aux-questions)).

## Le navigateur refuse de télécharger le fichier

**Cause.** Le navigateur peut lui aussi se montrer prudent lors du téléchargement d'un `.exe`.

**Solution.** Dans le panneau de téléchargements du navigateur, choisissez **Conserver** (Keep) à côté du fichier. Il finira alors de se télécharger.

## L'installeur ne démarre pas au double-clic

**Solution.**
- Vérifiez que le fichier s'est téléchargé complètement (environ 50–80 Mo).
- Faites un clic droit sur le fichier et choisissez **Ouvrir**.
- Retéléchargez l'installeur si le fichier est endommagé.

## La clé de licence n'est pas acceptée

| Message | Ce que cela signifie | Que faire |
|---|---|---|
| « License key invalid » | La clé a été saisie avec une faute | Vérifiez l'orthographe. Il est plus simple de coller la clé avec **Paste from clipboard** |
| « Used on max devices » | La licence est déjà utilisée sur le nombre maximal d'appareils | Libérez la licence sur un autre appareil, puis réessayez. Le bouton **Manage devices** mène à la gestion des appareils |
| « Cannot reach license server » | Pas de connexion au serveur | Vérifiez votre connexion internet et cliquez sur **Retry** |

## L'application ne s'ouvre pas après l'installation

**Solution.**
- Ouvrez-la manuellement : l'icône **FarmPanel** sur le bureau ou dans le menu Démarrer.
- Redémarrez l'ordinateur et réessayez.
- Si cela n'aide pas, réinstallez l'application : désinstallez-la (voir [Comment désinstaller](#comment-désinstaller)) et réinstallez-la.

---

# Foire aux questions

**Ai-je besoin de droits d'administrateur pour installer ?**
Non. FarmPanel s'installe uniquement pour votre compte d'utilisateur et ne nécessite pas de droits d'administrateur.

**Dois-je installer .NET ou d'autres composants séparément ?**
Non. Tout le nécessaire est déjà inclus dans l'installeur — lancez simplement `Setup.exe`.

**Où l'application est-elle installée ?**
Dans le dossier personnel de votre utilisateur. Vous n'avez pas à choisir un dossier manuellement — l'installeur s'en charge.

**Est-il sûr de cliquer sur « Exécuter quand même » dans la fenêtre SmartScreen ?**
Oui, si vous avez téléchargé `Setup.exe` depuis la page officielle indiquée dans ce guide. L'avertissement apparaît simplement parce que le programme est nouveau pour le système.

**Où sont stockés mes mots de passe après l'installation ?**
Uniquement sur votre ordinateur. Ils sont chiffrés avec la protection intégrée de Windows, ne sont jamais stockés en clair et ne sont jamais envoyés ailleurs.

**Dois-je saisir la clé de licence à chaque fois ?**
Non. La clé est saisie une seule fois, lors de la première activation. Ensuite, l'application s'ouvre directement sur l'écran principal.

**Comment mettre à jour l'application vers une nouvelle version ?**
Il n'y a rien à faire — FarmPanel se met à jour automatiquement. Redémarrez simplement l'application de temps en temps pour que la dernière version soit installée (voir [Mises à jour](#mises-à-jour)).

**Où m'adresser si quelque chose n'a pas fonctionné ?**
Contactez le support sur Telegram : [t.me/farmpanel_fr](https://t.me/farmpanel_fr). Décrivez le problème et, si vous en avez un, joignez le texte du message d'erreur.

---

Après l'installation, passez au [Guide de l'utilisateur](../user-guide/USER-GUIDE.fr.md) — il explique en détail comment ajouter des comptes, les lancer et utiliser l'application.

*Fin du guide d'installation de FarmPanel.*
