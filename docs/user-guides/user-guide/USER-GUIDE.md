# FarmPanel User Guide

**Control panel for your Steam and CS2 account farm on Windows**

Document version: 1.0

🌐 **English** · [Русский](USER-GUIDE.ru.md) · [Español](USER-GUIDE.es.md) · [Português](USER-GUIDE.pt.md) · [Français](USER-GUIDE.fr.md) · [Türkçe](USER-GUIDE.tr.md) · [Bahasa Indonesia](USER-GUIDE.id.md) · [Tiếng Việt](USER-GUIDE.vi.md) · [हिन्दी](USER-GUIDE.hi.md) · [中文](USER-GUIDE.zh.md) · [العربية](USER-GUIDE.ar.md)

---

> **How to read this guide.** Buttons, tabs, and statuses appear in the app exactly as written in **bold** (for example, **Add Account**, **Start**, **Running**), so you always click the right thing. Every procedure tells you what to click, what happens next, and how to confirm success.

## Contents

1. [Introduction](#1-introduction)
2. [Before You Start](#2-before-you-start)
3. [First Launch](#3-first-launch)
4. [Interface Overview](#4-interface-overview)
5. [Core Workflows](#5-core-workflows)
6. [Common Tasks (“I want to…”)](#6-common-tasks-i-want-to)
7. [Feature Reference](#7-feature-reference)
8. [Statuses and Indicators](#8-statuses-and-indicators)
9. [Notifications](#9-notifications)
10. [Errors and Troubleshooting](#10-errors-and-troubleshooting)
11. [Best Practices](#11-best-practices)
12. [Frequently Asked Questions](#12-frequently-asked-questions)

---

# 1. Introduction

## What FarmPanel Is

**FarmPanel** is a Windows desktop application that helps you manage many Steam accounts and Counter-Strike 2 clients from a single window. Instead of opening dozens of Steam windows by hand, watching each one, and restarting the ones that freeze, you manage your entire account farm centrally — from one clear panel.

FarmPanel launches clients, isolates accounts from one another, watches their state in real time, and automatically recovers them after failures.

> **Important.** FarmPanel is **not a bot and not an auto-farmer**. It does not play for you and does not imitate in-game actions. It manages everything that happens *around* the game: launching clients, lobby invites, recovery after failures, and live visibility for each account. All in-game actions are performed by a real person.

## What Problems It Solves

If you have more than one account, this routine is familiar:

- you have to launch dozens of Steam and CS2 clients;
- each account must run separately, without interfering with the others;
- building lobbies and sending invites by hand is slow and tiring;
- a crashed CS2 has to be noticed and restarted in time;
- it is hard to tell who is already in a match and who is stuck loading.

FarmPanel removes this routine and brings every operation into one application.

## Who It Is For

The app is built for anyone who needs to centrally manage many Steam and CS2 accounts — from a handful to several hundred — with automated launch, live monitoring, and reliable recovery after failures.

## What You Can Do

- Keep all accounts in one place and quickly find the one you need.
- Start and stop accounts one at a time or all at once.
- Isolate each account in its own protected environment (a sandbox).
- Build parties of accounts and queue them for matchmaking together.
- Watch computer load, process health, and crashes in real time.
- Automatically recover accounts after a crash or after the app is closed.
- Arrange CS2 windows across your monitors using a preset layout.

![FarmPanel main screen (Dashboard)](../images/dashboard-overview.png)

---

# 2. Before You Start

## System Requirements

| Item | Minimum | Recommended |
|---|---|---|
| Operating system | Windows 10 or 11 (64-bit) | Windows 10 / 11 (64-bit) |
| Memory | 8 GB | 32 GB |
| Disk | Any | SSD |
| Simultaneous accounts | 2 | 4–10 CS2 accounts |
| Screen resolution | Working area at least 1280 pixels wide | Full HD (1920×1080) or higher |

## What to Prepare in Advance

- **The FarmPanel installer** — a file named `Setup.exe` that you download from the official download page.
- **A license key** — you receive it with your purchase. It looks like this: `XXXX-XXXX-XXXX-XXXX-XXXX` (five groups of four characters).
- **Your Steam account details** — logins and passwords, and Steam Guard codes if you use them. You can enter them one at a time or import a list from a file.
- **An internet connection** — required on first launch to activate the license, and afterwards for Steam and CS2 to work.

## Permissions

- Installation **does not require administrator rights** — the app installs for your user account only.
- The first time you run the installer, Windows may show a blue **SmartScreen** window (“Windows protected your PC”) — this is a routine warning for new programs. Click **More info**, then **Run anyway**.
- The app may need network access (for Steam) and access to Windows Firewall rules. If a firewall prompt appears, allow access.

## Where Your Data Is Stored

Logins and passwords are encrypted with the built-in Windows protection and are stored **only on your computer**. They are never saved in plain text and are never sent anywhere.

---

# 3. First Launch

Below is the path from installation to a ready-to-use panel. Follow the steps in order.

## Step 1. Install the App

1. Download the `Setup.exe` installer from the download page.
2. Double-click the `Setup.exe` file.
3. If a blue **SmartScreen** window appears (“Windows protected your PC”), click **More info**, then **Run anyway**. This is a routine warning for new programs, not an error.
4. Wait for the installation to finish. No administrator rights are needed — the installer checks your system and prepares everything.

**What happens next.** A FarmPanel icon appears on your desktop and in the Start menu.

![the Setup.exe installer window](../images/setup-installer.png)

## Step 2. Open the App

Double-click the **FarmPanel** icon on your desktop.

**What you will see.** On the very first launch, while the license is not yet activated, the **Activation Wizard** opens. The main screen appears only after successful activation.

## Step 3. Activate Your License

The activation window guides you step by step.

1. Type or paste your license key into the input field. To paste it from the clipboard, click **Paste from clipboard**.
2. The app checks the key format as you type. When the format is correct, the activate button becomes available.
3. Click **Activate**.

**What happens next.** The app contacts the license server and verifies the key. This takes a few seconds — you will see the **Activating** state.

**Sign of success.** The activation window closes and the app's main screen (**Dashboard**) opens. Your license is active — you will not need to enter the key again on later launches.

> **If activation fails**, the app shows a clear message and tells you what to do. Common cases are covered in [10. Errors and Troubleshooting](#10-errors-and-troubleshooting).

![the license activation window](../images/license-activation.png)

## Step 4. Check the Basic Settings

Before launching accounts for the first time, it is worth checking your settings.

1. Click **Settings** in the left panel, or press `Ctrl+,`.
2. Open the **Sandboxes** section and, if needed, choose a folder for sandboxes.
3. Optionally open **Appearance** and choose a theme (**System / Dark / Light**) and interface density.

Settings save automatically: after each change a short **Saved** notification appears.

## Step 5. Ready to Go

You can now add accounts and launch your first farm. See [5. Core Workflows](#5-core-workflows) for how.

**Sign that everything works.** The bottom bar of the window (the status bar) shows a summary: the number of accounts, active processes, and the current app version.

---

# 4. Interface Overview

The app runs in a single main window. It consists of fixed elements that are always in place and a screen area that changes depending on the section you choose.

```
┌────────────────────────────────────────────────────────────┐
│  Command Bar                                                │
├──────────┬─────────────────────────────────────────────────┤
│          │                                                 │
│ Sidebar  │   Working area of the selected screen           │
│          │                                                 │
│          │                                                 │
├──────────┴─────────────────────────────────────────────────┤
│  Status Bar                                                 │
└────────────────────────────────────────────────────────────┘
```

![overall window structure with labeled areas](../images/window-layout.png)

## 4.1. Command Bar (top bar)

**Purpose.** A fixed strip across the top of the window. It holds navigation, global search, and notifications.

**Location.** The very top row of the window.

**Main elements (left to right):**

- **Hamburger button (☰)** — collapses and expands the sidebar. Shortcut `Ctrl+B`.
- **Logo** — clicking it returns you to the main screen (**Dashboard**).
- **Breadcrumbs** — show where you are, for example `Accounts › alex_42 › Events`. Click any segment to jump to it.
- **Search / command palette** — in the center. Press `Ctrl+K` to open the command palette (see below).
- **Notification badge** — an icon with a counter (for example, `⚠ 3`). Clicking it opens the notification center.

**When to use it.** The command bar is always within reach: for quick jumps between screens, searching for an account by login, or running a command without the mouse.

### Command Palette

Press `Ctrl+K` at any time to open the command palette — a search box for every action and object in the app.

1. Start typing the name of a command, screen, account login, or workflow.
2. The list narrows to matching results. Move through them with `↑` `↓`.
3. Press `Enter` to run the selected item.

**Why it helps.** The command palette is the fastest way to find anything without memorizing where the buttons are.

![the command palette open](../images/command-palette.png)

## 4.2. Sidebar

**Purpose.** The main navigation for the app.

**Location.** On the left, full height of the window.

**Sections (top to bottom):**

| Icon | Section | What it shows |
|---|---|---|
| ▤ | **Dashboard** | Overview of the whole farm |
| 👥 | **Accounts** | List of all accounts (the main working screen) |
| ⚙ | **Workflows** | Automated launch scenarios and their progress |
| ⚔ | **Matchmaking** | Parties and match search |
| 📈 | **Monitoring** | Computer load and process health |
| 📜 | **Logs** | The event log |
| ▣ | **Layouts** | Arranging CS2 windows across monitors |
| ▦ | **Sandboxes** | Sandboxes (isolated environments) |
| ⚙ | **Settings** | App settings |
| ? | **Help** | Help |

Some sections show a counter (for example, the number of accounts) or a live dot when there is activity.

**Main actions:**

- Click a section to open it. You can also use `Ctrl+1`…`Ctrl+8`.
- The collapse button (or `Ctrl+B`) shrinks the panel to icons to free up space.

**Tip.** Switching between sections preserves your state — filters, selection, and scroll position. When you return to a screen, you find it exactly as you left it.

![the sidebar with all sections](../images/sidebar.png)

## 4.3. Status Bar

**Purpose.** A thin bar at the bottom of the window with a quick summary of the whole farm's state.

**Location.** The very bottom row of the window.

**What it shows (example):**

```
[env: PROD] | ● 412 accounts (238 running) | ▶ 18 workflows | ◎ 7 matches | CPU 42% RAM 71% | ⚠ 3 errors | 14:32:08 | v1.0.1
```

- how many accounts exist and how many are running now;
- how many workflows and active matches are in progress;
- processor and memory load;
- the number of errors (click to open the notification center);
- the time and app version.

**When to use it.** Glance at the status bar to tell in a second whether everything is fine.

## 4.4. Dashboard Screen

**Purpose.** A single overview screen. In a few seconds it answers: how many accounts are online, how many workflows are running or failed, is there matchmaking activity, are there any crashes, and how loaded is the computer.

**Location.** The first section in the sidebar. It opens right after launch.

**Main areas:**

- **KPI strip** — five cards at the top: **Accounts**, **Workflows**, **Matches**, **Errors**, **System**. Each shows a headline number and a mini chart. Clicking a card takes you to the matching screen.
- **Live Activity Feed** — a real-time stream of operational events. Use the pause button (or the `Space` key) to pause scrolling.
- **Account State Heatmap** — a grid where each account is a colored cell. The color reflects its status. Hover to see the login and status; click to jump to the account.
- **Active Workflows / Matchmaking Queue / Sandboxes** — three tiles summarizing workflows, the match queue, and sandboxes.
- **Failures & Crashes** — a table of recent errors and crashes from the last hour.

**Typical use.** In the morning, open the **Dashboard** to size up the farm at a glance, then go to wherever attention is needed.

**Tips.**
- The metrics refresh automatically. To force a full refresh, press `F5`.
- If anything is highlighted red in the **Errors** card or the failures table, start your investigation there.

![the Dashboard with the KPI strip and activity feed](../images/dashboard-screen.png)

## 4.5. Accounts Screen

**Purpose.** The main working screen. Here you store accounts, find the ones you need, and start and stop them.

**Location.** The second section in the sidebar (`Ctrl+2`).

**Main areas:**

- **Toolbar** — the **Add Account**, **Import**, **Export**, and **Refresh** buttons, the search field, filters, and view controls.
- **Accounts table** — a list of all accounts with columns: status, login, nickname, rank, workflow, sandbox, tags, last login time, and others.
- **Details Pane** — on the right. Shows details of the selected account. Show or hide it with `Ctrl+\`.

**What you can do:**

- Add accounts one at a time or import a list.
- Search and filter accounts.
- Start, stop, and restart a single account or many at once.
- Bind accounts to sandboxes and assign workflows.
- View a detailed account card: data, history, events, and logs.

**Typical use.** Select the accounts you need in the table, then perform an action on them — using the toolbar, the context menu (right-click), or keyboard shortcuts.

Detailed step-by-step instructions are in [5. Core Workflows](#5-core-workflows).

![the Accounts screen with the table and details pane](../images/accounts-screen.png)

### Account Details Pane

To the right of the table, a card for the selected account appears with these tabs:

| Tab | What it shows |
|---|---|
| **Overview** | Core data, sandbox binding, assigned workflow, tags, key dates, and action buttons |
| **Inventory** | The account's inventory: item count and value |
| **Workflow** | The current state of the assigned scenario and its current step |
| **Events** | Recent events for this account |
| **Logs** | The event log filtered to this account |
| **History** | Change history: creation, edits, renames, sandbox rebinds |

At the bottom of the **Overview** tab is a block of buttons: **Start**, **Stop**, **Restart**, **Pause**, plus **Edit account** and **Delete**. The most relevant action is highlighted: **Start** when the account is stopped, and **Stop** when it is running.

## 4.6. Workflows Screen

**Purpose.** Manage automated launch scenarios and watch them run.

**Location.** The third section in the sidebar (`Ctrl+3`).

**What a workflow is.** A workflow is a predefined sequence of steps that the app performs for an account: sign in to Steam, launch CS2, and so on. The same scenario always runs the same way, so the result is predictable.

- **Definition** — the scenario template: a set of steps.
- **Instance** — a single run of a definition for a specific account.

**Main areas:**

- **Left** — a list of definitions (templates) and their versions.
- **Center** — a table of running instances: which scenario, for which account, at which step, how many retries, when started.
- **Right** — details of the selected instance (**Overview**, **State Machine**, **Steps**, **Logs**, **Retries** tabs).
- **Bottom** — a collapsible event timeline for the visible instances (`Ctrl+T`).

**When to use it.** Come here to see which step each account's launch is on, pause or restart a scenario, or figure out why something did not finish.

![the Workflows screen with three panes](../images/workflows-screen.png)

## 4.7. Matchmaking Screen

**Purpose.** Build parties of accounts and queue them for matchmaking together.

**Location.** The fourth section in the sidebar (`Ctrl+4`).

**Key concepts:**

| Term | Meaning |
|---|---|
| **Party** | A group of accounts that search for a match together |
| **Quorum** | All party members are signed in, in the queue, and not in a match |
| **Queue** | Waiting for a match: position, region, mode |
| **Match Found** | Steam found a match. The app confirms readiness for all members automatically — you do not need to do anything |
| **Desync** | Members are in an inconsistent state (for example, someone dropped out of the queue) |

**Main areas:**

- **Left** — a list of parties with their state (quorum, desync, match found, idle).
- **Right** — details of the selected party: members, their state, queue position, network latency, sandbox.
- **Bottom** — a timeline of recent matchmaking events.

**When to use it.** Here you build parties of 2–5 accounts and put them in the queue. When a match is found, the app confirms readiness for all members automatically.

![the Matchmaking screen with parties and details](../images/matchmaking-screen.png)

## 4.8. Monitoring Screen

**Purpose.** Watch computer load, process health, and crashes in real time.

**Location.** The fifth section in the sidebar (`Ctrl+5`).

**Main areas:**

- **Resource gauges** — **CPU**, **RAM**, **Disk**, **Net**, and, where available, **GPU** cards with current values and mini charts.
- **Process Explorer** — a table of all running Steam and CS2 processes: which account each belongs to, how much it consumes, how long it has run.
- **Crashes & Warnings** — a feed of recent failures.
- **Logs panel** — a log at the bottom of the screen, which can be collapsed.

**Time controls.** At the top you can switch between **Live** (real time), **Last 1h / 24h**, and **Custom** (a custom period). The **Freeze** button (`Ctrl+Space`) freezes the picture so you can study it calmly.

**When to use it.** If the computer starts to slow down or crashes become frequent, open **Monitoring** to see which process is consuming resources and what exactly crashed.

> **Tip.** You can open the **Monitoring** screen in a separate window with the detach button and place it on a second monitor.

![the Monitoring screen with gauges and process list](../images/monitoring-screen.png)

## 4.9. Logs Screen

**Purpose.** A detailed log of all app events — like a live feed of what is happening.

**Location.** The sixth section in the sidebar (`Ctrl+6`).

**Main features:**

- **Level filter** — the **Error**, **Warn**, **Info**, **Debug** toggles. By default errors, warnings, and info messages are shown.
- **Source filter** — you can narrow the log to a single account, workflow, or sandbox.
- **Search** — `Ctrl+F`, with jumping between matches (`F3` / `Shift+F3`).
- **Follow** — the log scrolls automatically to new lines. The `Space` key turns following on and off. If you scroll up, following pauses and a jump-to-bottom button appears.
- **Export** — save the visible lines to a file.

**When to use it.** When you need the details: exactly what happened to a specific account and in what order.

![the Logs screen with an event log](../images/logs-screen.png)

## 4.10. Layouts Screen

**Purpose.** Arrange CS2 windows across one or more monitors using a preset layout.

**Location.** The seventh section in the sidebar (`Ctrl+7`).

**Key concepts:**

- **Preset** — a saved window arrangement.
- **Slot** — a rectangular area on a monitor where one window will go.
- **Snap** — the command that arranges running windows into slots.

**Main areas:**

- **Left** — a list of saved presets.
- **Right** — a canvas showing your monitors, on which you place slots.
- **Bottom** — a bindings table: which slot corresponds to which account or role.

**How to use it.**
1. Create a preset with the **New Preset** button.
2. Place the slots on the canvas.
3. Set which account goes in which slot.
4. Click **Apply** or **Snap windows** — the app arranges the running CS2 windows into the defined places.

> **Safety net.** Before arranging, the app remembers the current window positions. The **Revert layout** button restores the previous positions within one minute.

![the Layouts screen with the monitor canvas](../images/layouts-screen.png)

## 4.11. Sandboxes Screen

**Purpose.** Manage sandboxes — the isolated environments in which Steam clients run.

**Location.** The eighth section in the sidebar (`Ctrl+8`).

**What a sandbox is.** A sandbox is a separate, protected environment for one Steam client. Accounts in different sandboxes never overlap: they share no sessions, files, or traces. One account is bound to one sandbox.

**When to use it.** Here you create sandboxes and watch their state. In most cases sandboxes are assigned automatically when you add accounts, so you rarely need to come here on purpose.

## 4.12. Settings Screen

**Purpose.** Tailor the app to your preferences.

**Location.** The **Settings** section at the bottom of the sidebar (`Ctrl+,`).

**Layout.** On the left is a list of settings sections; on the right are the settings themselves. Changes save immediately: a short **Saved** notification appears after each one.

**Settings sections:**

| Section | What it configures |
|---|---|
| **General** | Launch with Windows, minimize to tray, update channel |
| **Appearance** | Theme (**System / Dark / Light**), density, font scale, reduced motion |
| **Accounts** | Behavior when creating accounts, retention of deleted ones |
| **Workflows** | Retry policy, limits on concurrent runs |
| **Sandboxes** | Sandbox folder, automatic recovery |
| **Monitoring** | Data refresh rate, warning thresholds |
| **Notifications** | Notifications and sounds per severity level |
| **Layouts** | Default layouts, multi-monitor behavior |
| **Hotkeys** | Keyboard shortcuts — can be reassigned |
| **Advanced** | Logging level, diagnostics, environment selection, reset to defaults |
| **About** | App version, buttons to open the data and log folders |

> **Note.** Some settings (for example, the sandbox folder or the environment) apply only after a restart. Such settings show a “Requires restart” badge next to them.

![the Settings screen](../images/settings-screen.png)

---

# 5. Core Workflows

This is the most important section. It contains complete step-by-step instructions for the main tasks. Each step describes what you will see and how to confirm success.

## 5.1. Adding a Single Account

**Goal.** Add one new Steam account to the app.

**What you need.** The account's login and password. A Steam Guard code if applicable.

### Step 1 — Open the add form

Go to the **Accounts** screen and click **Add Account** on the toolbar. You can also press `Ctrl+N`.

**Expected result.** A form with fields for the new account opens.

### Step 2 — Fill in the details

Fill in the fields:

- **Login** — required, must be unique.
- **Password** — required.
- **Steam Guard secret** — the Steam Guard code, if you have one (optional).
- **Nickname** — optional; may be fetched automatically on first login.
- **Tags** — optional tags for grouping.
- **Sandbox binding** — choose **Auto-assign**, a specific sandbox, or **None**.
- **Workflow** — the launch scenario, if you want to assign one right away.

**Expected result.** If the login is already taken, the field is highlighted red with an explanation. A weak password is highlighted amber — this is a warning and does not prevent saving.

### Step 3 — Save the account

Click the save button in the form.

**Expected result.** The form closes and the new account appears in the table with a **Draft** status or, if it is bound to a sandbox, ready to launch.

**Sign of success.** The account is visible in the table on the **Accounts** screen.

### Tips

- If you enable **Validate immediately** in the form, the app checks the login in the background and shows the result as a notification.
- For an account to be launchable, it must be bound to a sandbox. The simplest choice is **Auto-assign**.

### Common mistakes and how to fix them

- **“Login already in use.”** This login already exists in the app. Check your account list — you may have added it already.
- **Forgot the sandbox.** An account without a sandbox cannot be launched. Bind one later via the context menu → **Bind sandbox**.

![the add account form](../images/accounts-add-form.png)

## 5.2. Importing a List of Accounts from a File

**Goal.** Quickly add many accounts at once from a file.

**What you need.** A file with a list of accounts (TXT, CSV, or TSV). The simplest TXT line format is `login:password` (you can also use `login:password:steamguard:nickname`).

### Step 1 — Start the import wizard

On the **Accounts** screen, click the arrow next to the **Import** button and choose a source — for example, **From file…**. You can also press `Ctrl+I`.

**Expected result.** A step-by-step import wizard opens.

### Step 2 — Choose the source and how sandboxes are assigned

Point to the file with the **Browse…** button. At the bottom, choose how to assign sandboxes:

- **Auto-assign (round-robin)** — distribute in a cycle (recommended);
- **Bind to specific sandbox** — bind them all to one sandbox;
- **Leave unbound** — leave them without a sandbox.

Click Next.

### Step 3 — Check how the data was recognized

The wizard shows the first rows of the file as a table. Make sure the data was split into columns correctly. If the delimiter was detected wrong, set it manually.

**Expected result.** In the preview, logins and passwords are in their own columns.

### Step 4 — Map the fields

Drag the column headers onto the required cells: **Login**, **Password**, **SteamGuard**, **Nickname**.

### Step 5 — Check that the rows are valid

The wizard marks each row: ✓ valid, ⚠ warning, ✕ error. Rows with errors can be fixed right here or skipped.

**Expected result.** You see how many accounts will be added, how many are duplicates, and how many have errors.

### Step 6 — Confirm the import

Click **Import N accounts**.

**Expected result.** A progress bar with a per-row status appears. When it finishes, the accounts appear in the table.

**Sign of success.** The number of accounts in the table has grown by the number imported.

### How to cancel and recover

If you cancel the import while it is running, the app offers to roll back the batch already added. Confirm the rollback to return to the original state.

![the import wizard, row validation step](../images/import-wizard-validation.png)

## 5.3. Launching Multiple Accounts

**Goal.** Start several accounts at the same time.

**What you need.** Accounts that have been added and bound to sandboxes.

### Step 1 — Select the accounts

On the **Accounts** screen, check the accounts you want in the first column. To select all visible ones, press `Ctrl+A`.

**Expected result.** The toolbar switches to bulk mode and shows how many rows are selected, for example `12 selected`.

### Step 2 — Start the selected accounts

Click **Start** on the bulk toolbar. You can also press `Ctrl+R`.

**Expected result.** The selected accounts' status changes to **Starting**. The app prepares each account and begins launching. Launching happens in batches so the computer is not overloaded.

### Step 3 — Wait for launch

Watch the status column. Wait until the accounts move to the **Running** state.

**Expected result.** Launched accounts show **Running**, with an uptime counter next to them.

**Sign of success.** All selected accounts show **Running**. The active count in the status bar has increased.

### Tips

- You do not have to launch every account at once. Start with a small batch, make sure everything is stable, then add more.
- To launch a single account: select one row and click **Start**, or use the **Start** button in the details pane on the right.

### Common mistakes and recovery

- **An account stays in Starting for too long.** The login may be slow. Wait; if the status changes to **Error**, use the **Retry** button.
- **Some accounts did not start.** After a bulk launch, a summary shows how many succeeded and failed. Click **Filter to failed** to deal with just those.

![bulk launch of accounts, Starting/Running statuses](../images/accounts-bulk-start.png)

## 5.4. Stopping All Running Accounts

**Goal.** Cleanly shut down all active accounts.

### Step 1 — Select the accounts

Select the running accounts. To select all visible ones, press `Ctrl+A`.

### Step 2 — Stop them

Click **Stop** on the bulk toolbar, or press `Ctrl+.` (Ctrl and period).

**Expected result.** The app cleanly shuts down each account. The status changes to **Stopped**. If an account does not respond, after a while the app closes it forcibly.

**Sign of success.** All accounts show **Stopped**. The active count in the status bar has decreased.

### Tips

- **Stop** is a graceful shutdown. The app first tries to close the clients correctly.
- If an account is in a match, finish the in-game actions first, then stop it.

## 5.5. Creating a Party and Queueing It

**Goal.** Build a party of several accounts and queue them for matchmaking together.

**What you need.** Several running accounts (**Running**) that have signed in.

### Step 1 — Create a party

Go to the **Matchmaking** screen and click **Create Party**. You can also press `Ctrl+N`.

**Expected result.** A window opens where you can add accounts to the party and give it a name.

### Step 2 — Add members and save

Add 2 to 5 accounts to the party, set a name, and save.

**Expected result.** The new party appears in the list on the left.

### Step 3 — Check the quorum

Select the party and look at its members on the right. Make sure the party is in the **Quorum** state — that is, all members are signed in and ready.

**Expected result.** The party shows a **✓ Quorum** badge. If a member has a problem (for example, a slow login), it is shown as a separate line.

### Step 4 — Queue the party

Click **Queue** for the selected party (or `Ctrl+Q`). To queue all parties at once, use **Queue All** on the toolbar.

**Expected result.** Before queueing, the app runs its checks. Then all members enter the queue, with their positions and network latency shown.

**Sign of success.** Members are in the queue state, with a waiting-time counter running.

### Tips

- Choose the region and mode on the toolbar (for example, `EU` and `Premier`) before queueing.
- If the party enters the **Desync** state, use the **Re-sync** action to pause the queue and wait for a consistent state.

![a party in the queue with member positions](../images/matchmaking-party-queue.png)

## 5.6. What Happens When a Match Is Found

**Goal.** Understand what the app does at the moment a match is found.

**What you need.** A party that is in the queue.

### Match acceptance is automatic

When Steam finds a match, a prominent **MATCH FOUND** banner appears for the party. **You do not need to click anything** — the app confirms readiness for all party members within the given window. No action on your part is required.

**Expected result.** The party members accept the match automatically; their state changes to **✓ Accepted**.

**Sign of success.** All members show **Accepted**, and the match starts.

> **Tip.** Want to know a match was found without watching the screen? Enable a sound alert for **Match found** in **Settings → Notifications**. The acceptance still happens automatically — the sound is only there to keep you informed.

### What to do if the party desyncs

Sometimes a match cannot be confirmed for everyone — for example, if a member dropped out of the queue. The party then enters the **Desync** state. Use the **Re-sync** action, and if needed remove the problem member with **Drop member**, then queue the rest again.

![the Match Found banner](../images/matchmaking-match-found.png)

## 5.7. Recovering After a Crash or App Restart

**Goal.** Return the farm to a working state after a client crash, or after the app was closed and opened again.

**What you need.** Nothing extra — recovery largely happens automatically.

### What happens automatically

- **After a client crash.** If Steam or CS2 closes unexpectedly, the app notices, marks the account with the **Crashed** status, and shows a notification with a **Restart** button. Recovery often happens on its own within a few seconds.
- **After an app restart.** On startup, the app looks for Steam and CS2 processes left over from the previous session and takes them back under management. During this, a **Recovering** indicator appears in the status bar. Reattached accounts are marked “Reattached” briefly.

### What to do manually

1. Open the **Dashboard** and look at the **Failures & Crashes** table.
2. For a crashed account, click **Restart** in the notification, in the account row, or in the details pane.
3. If the app reports an **Orphan process** in the notification center, choose **Adopt** or **Kill**.

**Sign of success.** Accounts are in the **Running** status again, red crash markers are gone, and there is no active **Recovering** indicator in the status bar.

### Tips

- Do not relaunch everything by hand right after a crash — first give automatic recovery a few seconds.
- If crashes recur, open **Monitoring** to see the load: you may be running more accounts than this computer can handle.

![the Recovering indicator in the status bar](../images/status-recovering.png)

---

# 6. Common Tasks (“I want to…”)

Short answers to common goals. For full instructions, follow the links to section 5.

## “I want to add new accounts”

- **When you need it.** You have new Steam accounts.
- **What to do.** For one account, use the **Add Account** button on the **Accounts** screen. For many at once, use the **Import** button and the import wizard.
- **What happens.** The accounts appear in the table and are ready to launch (once they have a sandbox).
- More: [5.1](#51-adding-a-single-account), [5.2](#52-importing-a-list-of-accounts-from-a-file).

## “I want to launch Steam”

- **When you need it.** You need an account to sign in to Steam.
- **What to do.** Select the account on the **Accounts** screen and click **Start**.
- **What happens.** The app launches Steam in the account's sandbox and signs in. The status moves **Starting → Running**.

## “I want to launch CS2”

- **When you need it.** Steam is already running and you need to start the game.
- **What to do.** Launching the account with **Start** takes it through the whole scenario, including starting CS2 (if the assigned workflow includes it).
- **What happens.** After signing in to Steam, the app launches CS2. You can watch the steps on the **Workflows** screen.

## “I want to create a lobby”

- **When you need it.** You need to gather accounts into a game lobby.
- **What to do.** Build a party on the **Matchmaking** screen with **Create Party** and add members.
- **What happens.** The app combines the selected accounts into a party and helps bring them to a consistent state (quorum).
- More: [5.5](#55-creating-a-party-and-queueing-it).

## “I want to start matchmaking”

- **When you need it.** The party is built and ready.
- **What to do.** Select the party and click **Queue** (or **Queue All** for all of them).
- **What happens.** The members enter the queue; you see their positions and waiting time.

## “I want to stop all running sessions”

- **When you need it.** It is time to wrap up.
- **What to do.** Select the accounts (`Ctrl+A`) and click **Stop**.
- **What happens.** The app cleanly closes the clients, and statuses become **Stopped**.
- More: [5.4](#54-stopping-all-running-accounts).

## “I want to recover after a crash”

- **When you need it.** A client crashed or the app was restarted.
- **What to do.** Give automatic recovery a few seconds; if needed, click **Restart** for the crashed account.
- **What happens.** The app returns the accounts to work.
- More: [5.7](#57-recovering-after-a-crash-or-app-restart).

## “I want to arrange the windows on screen”

- **When you need it.** You want to lay out CS2 windows neatly across your monitor.
- **What to do.** On the **Layouts** screen, create a preset and click **Apply** / **Snap windows**.
- **What happens.** The running windows move into the defined places.

---

# 7. Feature Reference

This section covers individual features with their purpose, location, and specifics.

## 7.1. Account Search and Filters

**Purpose.** Quickly find the accounts you need in a large list.

**Location.** The **Accounts** screen toolbar: the search field and the **Filters** button.

**How to use it.**
- Type into the search field (`Ctrl+F`). You can search by parts: `login:alex`, `status:running`, `rank:>=gold`, `tag:prime`.
- Click **Filters** (`Ctrl+K` on this screen opens the filters window), set conditions by status, rank, sandbox, workflow, or tags, and save the set as a preset.

**Expected behavior.** The table immediately shows only matching accounts. Active filters appear as a row of chips below the toolbar.

**Tip.** Save frequently used condition sets as presets — they are available from the dropdown on the toolbar.

## 7.2. Grouping and Column Setup

**Purpose.** Organize the table to fit your task.

**Location.** The **Accounts** screen toolbar: the **Density**, **Columns**, and **Group** buttons.

**How to use it.**
- **Group** lets you group accounts by status, workflow, sandbox, tag, or rank. Groups show counters, for example `Running (24)`.
- **Columns** — the set of visible columns. Built-in sets are available: **Operational**, **Identity**, **Audit**, **Compact**. You can save your own.
- **Density** — the row height (more compact or more spacious).

## 7.3. Account Context Menu

**Purpose.** Quick access to every action for an account.

**Location.** Right-click an account row.

**What is available.** Edit, copy login or Steam ID, start/stop/restart, bind and unbind a sandbox, assign a workflow, re-authenticate (**Re-auth**), probe the login (**Probe login now**), work with tags, export, clone, and delete.

## 7.4. Bulk Operations

**Purpose.** Perform one action on many accounts at once.

**Location.** The **Accounts** screen toolbar in selection mode (when at least one row is checked).

**How to use it.** Check the accounts, then click the button you need: **Start**, **Stop**, **Restart**, **Bind sandbox**, **Workflow…**, **Tag…**, **Export**, or **Delete**.

**Expected behavior.** A window appears with a per-account progress view. You can cancel the operation while it runs.

**Limitation.** When deleting five or more accounts, the app asks you to confirm by typing the word `DELETE`.

## 7.5. Exporting Accounts

**Purpose.** Save account data to a file.

**Location.** The **Export** button on the toolbar or in the context menu.

**How to use it.** Choose a format: **TXT** (login:password), **CSV** (all fields), or **JSON** (the full record).

> **Warning.** Exporting passwords requires separate consent — the app asks you to tick a checkbox. Handle such files carefully.

## 7.6. Cloning an Account

**Purpose.** Quickly create a copy of an account as a starting point.

**Location.** Row context menu → **Clone…**.

**Expected behavior.** A form opens with the fields already filled in (the login becomes `original_copy`), except for the Steam Guard code and the sandbox binding — you set those again.

## 7.7. Workflows: Start, Pause, Stop

**Purpose.** Manage automated scenarios.

**Location.** The **Workflows** screen.

**How to use it.**

| Action | What it does | Asks for confirmation? |
|---|---|---|
| **Start** | Runs the scenario for the selected accounts | When launching more than 10 accounts |
| **Pause** | Gently pauses after the current step | No |
| **Resume** | Continues from the current point | No |
| **Stop** | Ends the scenario with cleanup | Yes |
| **Restart** | Stops and starts over | Yes (for a bulk operation) |
| **Skip step** | Marks the current step done and moves on | Yes |
| **Retry now** | Retries the current step immediately | No |

**Tip.** The **State Machine** tab in the details pane clearly shows which step a scenario is on.

## 7.8. Binding to a Sandbox

**Purpose.** Reserve an isolated environment for an account, without which it cannot be launched.

**Location.** Context menu → **Bind sandbox…**, or the **Bind sandbox** bulk operation.

**How to use it.** Choose a method: round-robin, fill empty ones first, or a specific sandbox.

**Limitation.** One account, one sandbox. If the chosen sandbox is already in use, the app offers to free it from the previous account.

## 7.9. Window Layouts

**Purpose.** Arrange CS2 windows using a preset layout.

**Location.** The **Layouts** screen.

**How to use it.** Create a preset, place slots on the monitor canvas, set the bindings, and click **Apply**.

**Tip.** The **Revert layout** button restores the previous window positions within one minute, in case a layout did not work out.

## 7.10. Notification Center

**Purpose.** A single place for all app notifications.

**Location.** The notification badge in the top bar, or `Ctrl+Shift+N`.

**How to use it.** The panel opens on the right. Switch between the **All**, **Errors**, **Warnings**, and **Info** tabs. For each entry you can go to the source, retry, or dismiss. The **Clear all** button empties the list.

**Limitation.** The last 200 entries are kept; older ones are removed.

---

# 8. Statuses and Indicators

Every status has a color, a glyph, and a label. Below is what each one means and whether you need to act.

| Status | Glyph | What it means | Action needed |
|---|---|---|---|
| **OK / Success** | ✓ (green) | Account online, login succeeded | No |
| **Running** | ▶ (blue) | Account or workflow is running | No |
| **Starting** | ◐ (violet) | Launch in progress, a transitional state | Wait for it to finish |
| **Queued** | ⏱ (grey) | Waiting in the queue | No |
| **Stopped** | ■ (grey) | Stopped, idle | Optional — you can start it |
| **Paused** | ⏸ (amber) | Scenario is paused | Click **Resume** to continue |
| **Warning** | △ (amber) | A non-critical anomaly | Check the details; often you can continue |
| **Error** | ✕ (red) | A recoverable failure | Click **Retry** or investigate the cause |
| **Crashed** | ☠ (dark red, pulsing) | The process exited unexpectedly | Click **Restart** |
| **Match Found** | ◎ (green, pulsing) | A CS2 match was found | Nothing — the app confirms readiness automatically |
| **Desync** | ⛓ (orange) | Party members are out of sync | Run **Re-sync** |
| **Info** | ⓘ (blue) | A neutral message | No |

**Additional indicators:**

- **Recovering** — a blue indicator in the status bar during app startup: processes from the previous session are being taken back under management. Wait for it to finish.
- **Reattached** — a temporary marker on an account row: the process was successfully taken over after a restart.
- **Frozen at HH:mm:ss** — on the **Monitoring** screen, means the data display is frozen (not in **Live** mode). To bring back live data, switch to **Live** or turn off **Freeze**.

**How to see details.** Hover over a status glyph to get a tooltip: since when the state has lasted, which step the account is on, and what the last event was.

![examples of statuses in the accounts table](../images/status-badges.png)

---

# 9. Notifications

The app reports events in three ways: **toasts** (pop up in the corner and disappear), the **status bar** (a persistent summary at the bottom), and **inline banners** (tied to a specific screen).

## Toasts

They appear in the bottom-right corner.

| Notification | Why it appears | What it means | What to do | Can it be ignored |
|---|---|---|---|---|
| **Saved** | You changed a setting | The change was saved | Nothing | Yes, it disappears on its own |
| Operation success (green) | An action completed successfully | Everything is fine | Nothing | Yes, disappears after ~5 seconds |
| Warning (amber) | A non-critical anomaly was noticed | Worth a look | Optionally view the details | Usually yes, disappears after ~10 seconds |
| Error (red) | An operation failed | Action is required | Click **View** or **Retry** | No, stays until dismissed |
| Crash | A client closed unexpectedly | An account crashed | Click **Restart** or open the dump | No, stays until acknowledged |

**Good to know.**
- Hovering over a notification stops the auto-dismiss timer — you can read it calmly.
- Identical notifications collapse into one with a counter, for example `… failed (×4)`.

## Status Bar

On the right side of the status bar, the most important unread notification is shown, for example `● 3 errors`. Clicking it opens the notification center.

## Inline Banners

They appear at the top of a screen and apply to it as a whole. Example: `⚠ Steam network degraded — 12 accounts retrying login`. A banner can be closed with the **Dismiss** button if it is non-blocking. Blocking banners (for example, when a service is unavailable) stay until the problem is resolved.

## Sound Alerts

Sound is off by default. You can enable it for specific events (for example, **Match found** or **Crash**) in **Settings → Notifications**. A sound for **Match found** is handy for knowing a match was found without watching the screen — the match acceptance itself happens automatically.

![an error toast with View and Retry buttons](../images/notification-error-toast.png)

---

# 10. Errors and Troubleshooting

Errors while running a farm are routine, and the app helps you resolve them. Below are common situations in the format “Problem → Possible cause → Solution → Expected result.”

## Cannot Activate the License

**Problem.** When entering the key, the app will not let you proceed.

| Message | Possible cause | Solution |
|---|---|---|
| “License key invalid” | The key was entered with a typo | Check the spelling. It is easier to paste the key with **Paste from clipboard** |
| “Used on max devices” | The license is already used on the maximum number of devices | Free the license on another device, then try again. The **Manage devices** button leads to device management |
| “Cannot reach license server” | No connection to the license server | Check your internet connection and click **Retry** |

**Expected result.** With a correct key and a connection to the server, the activation window closes and the **Dashboard** opens.

## An Account Will Not Launch

**Problem.** You clicked **Start**, but the account does not move to **Running**.

- **Possible cause.** The account is not bound to a sandbox.
  **Solution.** Open the account's context menu → **Bind sandbox…** and assign a sandbox.
- **Possible cause.** Re-authentication is required (stale login details); a “Reauth required” marker is next to the row.
  **Solution.** Context menu → **Re-auth (Steam Guard)**.
- **Possible cause.** Steam has temporarily rate-limited logins.
  **Solution.** Wait about a minute and click **Retry**.

**Expected result.** The status moves **Starting → Running**.

## Steam Stays in Waiting/Starting for a Long Time

**Problem.** The account is stuck at the login stage.

- **Possible cause.** A slow login or temporary Steam network issues.
  **Solution.** Give it a little time. If an **Error** status appears, click **Retry**. If the Steam network is unstable, a warning banner appears at the top — wait for it to recover.

**Expected result.** The account signs in and moves to **Running**.

## A Client Crashed

**Problem.** The account got the **Crashed** status.

- **Possible cause.** The CS2 or Steam client exited unexpectedly.
  **Solution.** In the notification that appears, click **Restart**. Recovery is often already underway automatically. Crash details are on the **Monitoring** screen in the **Crashes & Warnings** feed.

**Expected result.** The account restarts and returns to **Running**.

## A Party Entered Desync

**Problem.** The party is in the **Desync** state — members are in an inconsistent state.

- **Possible cause.** One member accepted a match and another did not in time, or someone dropped out of the queue.
  **Solution.** Click **Re-sync** to pause the queue and wait for consistency. If one account is causing trouble, remove it with **Drop member** and queue the rest again.

**Expected result.** The party returns to the **Quorum** state and is ready to queue again.

## A Bulk Launch Finished with Errors

**Problem.** After a bulk **Start**, some accounts did not launch.

- **Solution.** In the summary, click **Filter to failed** — the table shows only the problem accounts. Resolve each by the causes above and launch again.

**Expected result.** After the causes are resolved, a repeat **Start** moves the accounts to **Running**.

## A Screen's Data Will Not Load

**Problem.** Instead of the screen's content, there is a banner or a message that a service is unavailable.

- **Possible cause.** A background service is temporarily unavailable.
  **Solution.** Click **Retry**. If that does not help, click **Open logs** to see the details, or restart the app.

**Expected result.** The screen loads and shows current data.

## The App Reports an Orphan Process

**Problem.** In the notification center, a message like “Orphan process … — Adopt or Kill?”.

- **Possible cause.** A process from the previous session remained that could not be automatically bound to an account.
  **Solution.** Choose **Adopt** (take it under management) if the process is needed, or **Kill** (end it) if not.

**Expected result.** The process list is put in order.

## The Computer Is Slow and Crashes Are Increasing

**Problem.** General instability, frequent failures.

- **Possible cause.** More accounts are running than the computer can handle.
  **Solution.** Open **Monitoring** and look at **CPU** and **RAM**. If the values are near their limits, stop some accounts with **Stop**.

**Expected result.** The load drops and operation stabilizes.

> **Error codes.** Error details include a short code such as `[E-1042]`. You can copy it and use it when contacting support. A full reference of codes is available via **Help → Error reference**.

![an example error screen with Retry / Open logs buttons](../images/error-screen.png)

---

# 11. Best Practices

## Preparing Accounts

- Add accounts as a list via **Import** — it is faster and there are fewer typos.
- Leave the sandbox assignment on **Auto-assign** unless you need a specific binding.
- Use **Tags** to group accounts and filter them quickly.

## Launching Many Accounts

- Launch in batches: start with a small group, confirm stability, then add more.
- Keep the **Dashboard** or **Monitoring** open to watch the load in real time.
- Aim for the recommended 4–10 CS2 accounts at once; you can run more on a powerful PC and fewer on weaker machines.

## Working with Layouts

- Prepare several presets in advance for different situations (for example, “4-stack”, “single focused”).
- After a layout goes wrong, use **Revert layout** right away, while the one-minute revert window is active.

## Stopping Safely

- Stop accounts with the **Stop** button (a graceful shutdown) rather than closing windows by hand.
- Before exiting the app, stop the active accounts. If you try to close the app while scenarios are running, it warns you.

## Avoiding Interruptions

- Before queueing, make sure the party is in the **Quorum** state.
- Watch banners about the Steam network state — when it is unstable, it is better to wait.

## Maintaining Stable Operation

- Check the **Dashboard** regularly — it shows the overall state in seconds.
- Keep the number of simultaneously running accounts within your computer's capacity.
- Let automatic recovery work for a few seconds before stepping in by hand.

---

# 12. Frequently Asked Questions

**Why can't I launch an account?**
Most likely the account is not bound to a sandbox — without one it cannot launch. Bind one via the context menu → **Bind sandbox…**. A launch can also be blocked by the need to re-authenticate (a “Reauth required” marker) — in that case run **Re-auth**.

**Why does Steam stay in a waiting state for a long time?**
This is usually a slow login or temporary Steam network delays. Give it a little time. If an **Error** status appears, click **Retry**.

**How do I restart a workflow?**
Select the accounts or instances you need and click **Restart** (or `Ctrl+Shift+R`). For a bulk operation, the app asks for confirmation.

**What happens if the app closes?**
Your accounts and settings are saved. On the next launch, the app tries to take the previous session's processes back under management — a **Recovering** indicator appears in the status bar. If scenarios were active when it closed, the app warns you in advance.

**How do I know everything is working?**
Check the status bar at the bottom and the **Dashboard**. Signs of normal operation: accounts in the **Running** status, no red markers in the **Errors** card or the **Failures & Crashes** table, and **CPU** and **RAM** load within normal ranges.

**Where are my passwords stored?**
Only on your computer. They are encrypted with the built-in Windows protection, are never saved in plain text, and are never sent anywhere.

**Does FarmPanel play for me?**
No. It is not a bot or an auto-farmer. The app manages launching, monitoring, lobby building, and recovery, while all in-game actions are performed by you.

**Do I have to enter the license key every time?**
No. The key is entered once, during the first activation. After that the app opens straight to the **Dashboard**.

**How do I quickly find an action if I forgot where the button is?**
Press `Ctrl+K` to open the command palette. Start typing the name of an action, screen, or account login, and pick the one you need from the list.

**Can I move monitoring to a second monitor?**
Yes. On the **Monitoring** screen, click the detach button — the screen opens as a separate window that you can place on a second monitor. Its position is remembered.

**How do I reset the settings to their defaults?**
In **Settings → Advanced** there is **Reset to defaults**. To protect against accidental clicks, the app asks you to confirm by typing text.

---

*End of the FarmPanel User Guide.*
