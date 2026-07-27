# Installing Sandboxie-Plus

**Step-by-step installation guide for Windows**

Document version: 1.0 · Sandboxie-Plus version: **1.17.5**

🌐 **English** · [Русский](INSTALL-SANDBOXIE-PLUS.ru.md) · [Español](INSTALL-SANDBOXIE-PLUS.es.md) · [Português](INSTALL-SANDBOXIE-PLUS.pt.md) · [Français](INSTALL-SANDBOXIE-PLUS.fr.md) · [Türkçe](INSTALL-SANDBOXIE-PLUS.tr.md) · [Bahasa Indonesia](INSTALL-SANDBOXIE-PLUS.id.md) · [Tiếng Việt](INSTALL-SANDBOXIE-PLUS.vi.md) · [हिन्दी](INSTALL-SANDBOXIE-PLUS.hi.md) · [中文](INSTALL-SANDBOXIE-PLUS.zh.md) · [العربية](INSTALL-SANDBOXIE-PLUS.ar.md)

---

FarmPanel keeps each account in its own **sandbox** — an isolated environment where Steam and CS2 do not overlap with other accounts. This isolation is handled by a free program called **Sandboxie-Plus**. You install it once, before you start launching accounts in FarmPanel.

This guide walks you through the installation step by step. Nothing complicated — it takes a few minutes.

> **In short.** Download the **Sandboxie-Plus 1.17.5** installer → run it → accept the default settings → allow the installation (administrator rights are required) → done.

> **Important.** Unlike FarmPanel itself, Sandboxie-Plus **requires administrator rights** to install — this is normal, because the program integrates deeply into Windows to reliably isolate applications.

## Contents

1. [What You'll Need](#1-what-youll-need)
2. [Step 1. Download the Installer](#step-1-download-the-installer)
3. [Step 2. Run the Installation](#step-2-run-the-installation)
4. [Step 3. Go Through the Setup Wizard](#step-3-go-through-the-setup-wizard)
5. [Step 4. First Launch of Sandboxie-Plus](#step-4-first-launch-of-sandboxie-plus)
6. [Step 5. Check That Everything Works](#step-5-check-that-everything-works)
7. [Step 6. Connect It to FarmPanel](#step-6-connect-it-to-farmpanel)
8. [How to Uninstall Sandboxie-Plus](#how-to-uninstall-sandboxie-plus)
9. [Troubleshooting](#troubleshooting)
10. [Frequently Asked Questions](#frequently-asked-questions)

---

# 1. What You'll Need

- **A computer running Windows 10 or 11** (64-bit).
- **Administrator rights** on this computer (a prompt appears during installation — you need to click **Yes**).
- **An internet connection** — to download the program.
- **About 5 minutes of your time.**

> Sandboxie-Plus is free. Some extra features are available to those who support the project, but you **do not need** them to work with FarmPanel — the regular free version is enough.

---

# Step 1. Download the Installer

1. Open the official page for the version you need:
   **[Sandboxie-Plus 1.17.5 on GitHub](https://github.com/sandboxie-plus/Sandboxie/releases/tag/v1.17.5)**
2. Scroll down to the **Assets** section.
3. Find and download the file named something like **`Sandboxie-Plus-x64-v1.17.5.exe`** — this is the installer for a regular 64-bit Windows.

**How to choose the right file:**

| File | Who it's for |
|---|---|
| **`Sandboxie-Plus-x64-v1.17.5.exe`** | **Most users** — a regular Windows on an Intel or AMD processor. Download this one. |
| `Sandboxie-Plus-arm64-v1.17.5.exe` | Only for computers with an ARM processor (rare). |
| `Sandboxie-Classic-…` | The old interface variant. **Not needed** for FarmPanel — choose **Plus**. |
| `.7z` files | Portable versions for advanced users. **Not needed** for installation. |

**What happens next.** The file appears in your **Downloads** folder.

> **Tip.** Download the installer only from the official GitHub page linked above. That way you get the genuine, verified version.

![the 1.17.5 release page with the Assets section](../images/sandboxie/github-release-assets.png)

---

# Step 2. Run the Installation

1. Open your **Downloads** folder and double-click the downloaded **`Sandboxie-Plus-x64-v1.17.5.exe`** file.
2. Windows shows the prompt **“Do you want to allow this app to make changes to your device?”** — click **Yes**. This is the administrator-rights prompt; without it, Sandboxie-Plus cannot be installed.

> **If a blue SmartScreen window appears** (“Windows protected your PC”) — click **More info**, then **Run anyway**. This is a routine warning for downloaded programs, not an error.

**What happens next.** The installation wizard window opens.

---

# Step 3. Go Through the Setup Wizard

The installation wizard walks you through a few simple screens. In most cases you can just leave everything at the defaults and click **Next**.

1. **Language selection.** If a language selection window appears, choose English (or your language) and click **OK**.
2. **License agreement.** Read it and click **I Agree** or **Next**.
3. **Install folder.** Leave the default folder (`C:\Program Files\Sandboxie-Plus`) and click **Next**. There's no need to change it.
4. **Install options.** Nothing needs to be changed — just click **Next** / **Install**.
5. Wait for it to finish. Installation takes less than a minute.
6. On the last screen, click **Finish**. Leave the “launch Sandboxie-Plus” checkbox enabled if there is one.

**What happens next.** Sandboxie-Plus is installed, and its icon appears on your desktop and in the Start menu. The program usually launches right after installation.

> **Is a restart needed?** Usually not. But if the wizard asks you to restart the computer, do so, so the isolation works correctly.

![the installation wizard screen with the default folder](../images/sandboxie/installer-wizard.png)

---

# Step 4. First Launch of Sandboxie-Plus

The first time you open Sandboxie-Plus, it shows a **Setup Wizard**. Go through it step by step — just repeat what's described below.

If a **UI language selection** window appears before the wizard, choose your language and click **OK**.

The wizard then guides you through several screens.

### Screen 1 — Introduction

Select **“Personally, for private non-commercial use”** and click **Next**.

![Setup Wizard — the Introduction screen with “Personally, for private non-commercial use” selected](../images/sandboxie/wizard-1-introduction.png)

### Screen 2 — Support certificate

Leave the field **empty** and click **Next**. A certificate is not needed to work with FarmPanel.

![Setup Wizard — the Support certificate screen with an empty field](../images/sandboxie/wizard-2-support-certificate.png)

### Screen 3 — Configure UI

Leave the values at their **defaults** (**Advanced UI for experts** is already selected) and click **Next**.

![Setup Wizard — the UI configuration screen with default values](../images/sandboxie/wizard-3-ui-configuration.png)

### Screen 4 — Shell integration

**Clear all checkboxes** and click **Next**.

![Setup Wizard — the Shell integration screen with all checkboxes cleared](../images/sandboxie/wizard-4-shell-integration.png)

### Screen 5 — Updater

**Clear all checkboxes** and click **Next**.

![Setup Wizard — the Updater screen with all checkboxes cleared](../images/sandboxie/wizard-5-updater.png)

### Screen 6 — Complete

Click **Finish** to apply the settings and close the wizard.

![Setup Wizard — the final screen with the Finish button](../images/sandboxie/wizard-6-complete.png)

> **Tip.** If you're unsure on any screen, clear the checkboxes and click **Next**. FarmPanel does not need the extra integrations or update reminders.

**What happens next.** The main Sandboxie-Plus window opens — the list of sandboxes and the control panel.

![the main Sandboxie-Plus window after first launch](../images/sandboxie/main-window.png)

---

# Step 5. Check That Everything Works

Make sure Sandboxie-Plus is installed correctly:

1. Open Sandboxie-Plus (the icon on the desktop or in the Start menu).
2. The main window shows a list of sandboxes — there is usually a default sandbox named something like **DefaultBox**.
3. The program opens and shows no error messages.

If all of this is in place — **Sandboxie-Plus is installed and ready to use**.

---

# Step 6. Connect It to FarmPanel

Once Sandboxie-Plus is installed, FarmPanel can use it to isolate accounts.

1. Open **FarmPanel**.
2. Go to **Settings → Sandboxes**.
3. Make sure the sandbox folder path is set. If the field is empty, choose a folder for sandboxes; if it is already filled in, there's nothing to change.
4. Go back to the **Accounts** screen. Now, when adding accounts, you can choose how sandboxes are assigned (**Auto-assign** and others), and the accounts can be launched.

> **How this connects.** In FarmPanel, every account must be bound to a sandbox, otherwise it cannot be launched. It is Sandboxie-Plus that creates and maintains these isolated environments “under the hood”. For more about sandboxes and launching accounts, see the [FarmPanel User Guide](../user-guide/USER-GUIDE.md).

**Sign of success.** An account in FarmPanel launches and moves to the **Running** status — which means isolation through Sandboxie-Plus is working.

---

# How to Uninstall Sandboxie-Plus

If you need to remove the program:

1. First, close all programs running in sandboxes (in FarmPanel, stop the accounts with **Stop**).
2. Open **Windows Settings** → **Apps** → **Installed apps**
   (or “Control Panel” → “Programs and Features”).
3. Find **Sandboxie-Plus** in the list.
4. Click **Uninstall** and confirm. Administrator rights are also required to uninstall.

> **Note.** After Sandboxie-Plus is removed, FarmPanel cannot launch accounts until the program is installed again.

---

# Troubleshooting

## Windows won't let you install — no administrator rights

**Cause.** Sandboxie-Plus strictly requires administrator rights.

**Solution.** Sign in with an account that has administrator rights, or ask the computer's administrator to install the program. When the **“Do you want to allow changes?”** prompt appears, click **Yes**.

## A SmartScreen window appeared

**Cause.** Windows warns about recently downloaded programs. It is not an error.

**Solution.** Click **More info**, then **Run anyway**.

## An antivirus blocked the installer

**Cause.** Some antivirus programs are cautious about software that integrates into the system.

**Solution.**
1. Make sure you downloaded the file from the official GitHub page (the link is in [Step 1](#step-1-download-the-installer)).
2. If needed, temporarily add the file to your antivirus exclusions and download it again.

## Downloaded the wrong file

**Cause.** There are several files on the release page.

**Solution.** For a regular Windows you need the file named **`Sandboxie-Plus-x64-v1.17.5.exe`**. Do not take the **arm64**, **Classic**, or **.7z** variants. Go back to [Step 1](#step-1-download-the-installer) and download the right file.

## FarmPanel won't launch accounts after installation

**Solution.**
1. Make sure Sandboxie-Plus is installed and opens (see [Step 5](#step-5-check-that-everything-works)).
2. In FarmPanel, open **Settings → Sandboxes** and check that the sandbox folder path is set.
3. Restart FarmPanel.
4. If the problem persists, contact support (see [Frequently Asked Questions](#frequently-asked-questions)).

## The computer asks for a restart after installation

**Solution.** Restart the computer — this completes the installation and enables isolation. After the restart, open FarmPanel again.

---

# Frequently Asked Questions

**Is installing Sandboxie-Plus mandatory?**
Yes, if you want to launch accounts in FarmPanel. It is Sandboxie-Plus that provides the isolation of each account in a separate environment.

**Is Sandboxie-Plus paid?**
No, the basic version is free and it is enough to work with FarmPanel. Extra features are available to those who support the project, but they are not required.

**Why does installation require administrator rights while FarmPanel doesn't?**
Sandboxie-Plus integrates deeply into Windows to reliably isolate programs, so it needs administrator rights. FarmPanel, on the other hand, installs for your user account only and does not require them.

**Do I need to configure the sandboxes myself?**
No. Just install Sandboxie-Plus. FarmPanel creates and configures the sandboxes for accounts automatically.

**Do I need a supporter certificate?**
No. You can skip that screen on first launch. It is not needed for FarmPanel.

**Which exact version should I install?**
Version **1.17.5** — the link is in [Step 1](#step-1-download-the-installer). Install exactly this one for predictable compatibility with FarmPanel.

**Where do I go if something didn't work?**
Contact FarmPanel support on Telegram: [t.me/farmpanel_en](https://t.me/farmpanel_en). Describe the problem and include the text of the error message if you have one.

---

After installing Sandboxie-Plus, go back to the [FarmPanel installation guide](../install-guide/INSTALL-GUIDE.md) or straight to the [User Guide](../user-guide/USER-GUIDE.md) to add accounts and launch your first farm.

*End of the Sandboxie-Plus installation guide.*
