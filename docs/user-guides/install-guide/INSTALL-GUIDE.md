# Installing FarmPanel

**Step-by-step installation guide for Windows**

Document version: 1.0

🌐 **English** · [Русский](INSTALL-GUIDE.ru.md) · [Español](INSTALL-GUIDE.es.md) · [Português](INSTALL-GUIDE.pt.md) · [Français](INSTALL-GUIDE.fr.md) · [Türkçe](INSTALL-GUIDE.tr.md) · [Bahasa Indonesia](INSTALL-GUIDE.id.md) · [Tiếng Việt](INSTALL-GUIDE.vi.md) · [हिन्दी](INSTALL-GUIDE.hi.md) · [中文](INSTALL-GUIDE.zh.md) · [العربية](INSTALL-GUIDE.ar.md)

---

This guide takes you from downloading the program to your first launch. Follow the steps in order — nothing complicated, it only takes a few minutes.

> **In short.** Download `Setup.exe` → run it → activate your license with the key → done. No administrator rights are needed, and nothing else has to be installed separately.

## Contents

1. [What You'll Need](#1-what-youll-need)
2. [System Requirements](#2-system-requirements)
3. [Step 1. Download the Installer](#step-1-download-the-installer)
4. [Step 2. Run the Installation](#step-2-run-the-installation)
5. [Step 3. Open the App](#step-3-open-the-app)
6. [Step 4. Initial Setup — Steam & Sandboxie Locations](#step-4-initial-setup--steam--sandboxie-locations)
7. [Step 5. Activate Your License](#step-5-activate-your-license)
8. [Step 6. Check That Everything Works](#step-6-check-that-everything-works)
9. [Updates](#updates)
10. [How to Uninstall](#how-to-uninstall)
11. [Installation Troubleshooting](#installation-troubleshooting)
12. [Frequently Asked Questions](#frequently-asked-questions)

---

# 1. What You'll Need

- **A computer running Windows 10 or 11** (64-bit).
- **An internet connection** — to download the program and activate the license.
- **A license key** — you receive it with your purchase. It looks like this:
  `XXXX-XXXX-XXXX-XXXX-XXXX` (five groups of four characters).
- **About 10 minutes of your time.**

> You **do not need** to install anything else separately (such as .NET) — everything required is already included in the installer.

---

# 2. System Requirements

| Item | Minimum | Recommended |
|---|---|---|
| Operating system | Windows 10 or 11 (64-bit) | Windows 10 / 11 (64-bit) |
| Memory | 8 GB | 32 GB |
| Disk | Any | SSD |
| Free space | about 500 MB | 1 GB or more |
| Simultaneous accounts | 2 | 4–10 CS2 accounts |
| Screen resolution | at least 1280 pixels wide | Full HD (1920×1080) or higher |

If your computer meets the minimum, the app will run. The more powerful your computer, the more accounts you can keep running at once.

---

# Step 1. Download the Installer

1. Open the official download page:
   **[Download for Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   (you can also find the download link on the [farmpanel.cc](https://farmpanel.cc) website).
2. Find the file named something like **`Setup.exe`** (in the **Assets** section if you are on the releases page) and click it to download.
3. Wait for the download to finish. The file is about 50–80 MB, so on a fast connection it takes less than a minute.

**What happens next.** The `Setup.exe` file appears in your **Downloads** folder.

> **Tip.** Download the installer only from the official page linked above. That way you get the genuine, verified version of the program.

![the download page with the Setup.exe file](../images/install-download-page.png)

---

# Step 2. Run the Installation

1. Open your **Downloads** folder and double-click the **`Setup.exe`** file.
2. Installation starts automatically. **Administrator rights are not required** — the app installs for your user account only.
3. Wait for it to finish. This usually takes less than a minute. There are no separate “Next” buttons to click — the installer does everything itself.

**What happens next.** The app is installed, and a **FarmPanel** icon appears on your desktop and in the Start menu. The app often opens right after installation.

> **If a blue “Windows protected your PC” (SmartScreen) window appears** — this is a routine warning for new programs, not an error. What to do:
> 1. Click **More info**.
> 2. Click the **Run anyway** button that appears.
>
> The installation continues as usual. More details in [Installation Troubleshooting](#installation-troubleshooting).

---

# Step 3. Open the App

If the app did not open by itself, double-click the **FarmPanel** icon on your desktop or find it in the Start menu.

**What you will see.** On the very first launch, the app walks you through a short initial setup and license activation — these are the next steps.

---

# Step 4. Initial Setup — Steam & Sandboxie Locations

On the first launch, the app asks you to point it to where **Steam** and **Sandboxie-Plus** are located on your computer. Without these paths, the app cannot launch and isolate accounts.

> **Important.** Sandboxie-Plus must already be installed by this point. If you haven't done so yet, see the separate [Installing Sandboxie-Plus](../install-sandboxie-plus/INSTALL-SANDBOXIE-PLUS.md) guide.

1. **Steam location.** Click the folder-picker button (**Browse…** / folder icon) next to the Steam field and select the folder where Steam is installed. This is usually `C:\Program Files (x86)\Steam`.
2. **Sandboxie location.** Click the folder-picker button next to the Sandboxie field and select the folder where Sandboxie-Plus is installed. This is usually `C:\Program Files\Sandboxie-Plus`.
3. Confirm the setup (the **Save** / **Continue** button).

**What happens next.** The app remembers these paths and uses them every time it launches accounts.

**Sign of success.** Both paths are set, and the app shows no warnings that Steam or Sandboxie could not be found.

> **Tip.** You can change these paths later at any time in **Settings**.

![initial setup — Steam and Sandboxie locations](../images/initial-setup-locations.png)

---

# Step 5. Activate Your License

Activation is only needed once — on the first launch.

1. Type or paste your license key into the input field.
   To paste it from the clipboard, click **Paste from clipboard**.
2. The app checks the key format as you type. When the format is correct, the activate button becomes available.
3. Click **Activate**.

**What happens next.** The app contacts the server and verifies the key. This takes a few seconds — you will see the **Activating** state.

**Sign of success.** The activation window closes and the app's main screen — **Dashboard** — opens. Your license is active. You will not need to enter the key again on later launches.

> **If the key is not accepted** — make sure you entered it without typos (it is easier to paste it with **Paste from clipboard**), and that you have internet. Common messages are covered in [Installation Troubleshooting](#installation-troubleshooting).

![the license activation window](../images/license-activation.png)

---

# Step 6. Check That Everything Works

After activation you land on the main screen. Confirm that the installation succeeded:

1. At the top of the window you can see the **sidebar** with sections (**Dashboard**, **Accounts**, **Workflows**, and others).
2. At the bottom of the window is the **status bar** — a thin strip with a summary and the app version (for example, `v1.0.1`).
3. The app opens and switches between sections without errors.

If all of this is in place — **installation is complete and you can start using the app**.

**What's next.** Add your Steam accounts and launch your first farm. For step-by-step instructions, see the [User Guide](../user-guide/USER-GUIDE.md) (the “Core Workflows” section).

![the main screen after installation](../images/dashboard-overview.png)

---

# Updates

FarmPanel updates **automatically** — you do not need to download anything by hand.

- The app checks for new versions at startup and from time to time while running.
- A new version is downloaded quietly, in the background, without interrupting your work.
- The update is applied the next time the app restarts.

**What you do.** Nothing special. Just close and reopen the app now and then, and the latest version will be installed. The current version is always visible in the status bar at the bottom and in **Settings → About**.

---

# How to Uninstall

If you need to remove FarmPanel:

1. Open **Windows Settings** → **Apps** → **Installed apps**
   (or “Control Panel” → “Programs and Features”).
2. Find **FarmPanel** in the list.
3. Click **Uninstall** and confirm.

**What happens next.** The app is removed from your computer. Administrator rights are not required to uninstall.

---

# Installation Troubleshooting

Below are common situations and what to do about them.

## A “Windows protected your PC” (SmartScreen) window appeared

**Cause.** Windows shows this warning for programs that were downloaded recently and are not yet widely known to the system. It does not mean anything is wrong with the file.

**Solution.**
1. Click **More info**.
2. Click **Run anyway**.

The installation continues. If there is no **More info** button, make sure you downloaded the file from the official page and try again.

## An antivirus blocked or deleted the file

**Cause.** Some antivirus programs treat new installers cautiously and can trigger a false alarm.

**Solution.**
1. Make sure you downloaded `Setup.exe` from the official page (the link is in [Step 1](#step-1-download-the-installer)).
2. If needed, add the file to your antivirus exclusions and download it again.
3. If in doubt, contact support (see [Frequently Asked Questions](#frequently-asked-questions)).

## The browser won't let you download the file

**Cause.** The browser can also be cautious when downloading an `.exe`.

**Solution.** In the browser's download panel, choose **Keep** next to the file. It will then finish downloading.

## The installer won't start on double-click

**Solution.**
- Make sure the file downloaded completely (about 50–80 MB).
- Right-click the file and choose **Open**.
- Download the installer again if the file is damaged.

## The license key is not accepted

| Message | What it means | What to do |
|---|---|---|
| “License key invalid” | The key was entered with a typo | Check the spelling. It is easier to paste the key with **Paste from clipboard** |
| “Used on max devices” | The license is already used on the maximum number of devices | Free the license on another device, then try again. The **Manage devices** button leads to device management |
| “Cannot reach license server” | No connection to the server | Check your internet connection and click **Retry** |

## The app won't open after installation

**Solution.**
- Open it manually: the **FarmPanel** icon on the desktop or in the Start menu.
- Restart the computer and try again.
- If that doesn't help, reinstall the app: uninstall it (see [How to Uninstall](#how-to-uninstall)) and install it again.

---

# Frequently Asked Questions

**Do I need administrator rights to install?**
No. FarmPanel installs for your user account only and does not require administrator rights.

**Do I need to install .NET or other components separately?**
No. Everything required is already included in the installer — just run `Setup.exe`.

**Where does the app install to?**
Into your personal user folder. You do not need to choose a folder manually — the installer handles it.

**Is it safe to click “Run anyway” in the SmartScreen window?**
Yes, if you downloaded `Setup.exe` from the official page listed in this guide. The warning appears simply because the program is new to the system.

**Where are my passwords stored after installation?**
Only on your computer. They are encrypted with the built-in Windows protection, are never saved in plain text, and are never sent anywhere.

**Do I have to enter the license key every time?**
No. The key is entered once, during the first activation. After that the app opens straight to the main screen.

**How do I update the app to a new version?**
There's nothing to do — FarmPanel updates automatically. Just restart the app now and then so the latest version is installed (see [Updates](#updates)).

**Where do I go if something didn't work?**
Contact support on Telegram: [t.me/farmpanel_en](https://t.me/farmpanel_en). Describe the problem and, if you have one, include the text of the error message.

---

After installation, move on to the [User Guide](../user-guide/USER-GUIDE.md) — it explains in detail how to add accounts, launch them, and work with the app.

*End of the FarmPanel installation guide.*
