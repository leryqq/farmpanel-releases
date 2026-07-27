# 安装 Sandboxie-Plus

**Windows 分步安装指南**

文档版本：1.0 · Sandboxie-Plus 版本：**1.17.5**

🌐 [English](INSTALL-SANDBOXIE-PLUS.md) · [Русский](INSTALL-SANDBOXIE-PLUS.ru.md) · [Español](INSTALL-SANDBOXIE-PLUS.es.md) · [Português](INSTALL-SANDBOXIE-PLUS.pt.md) · [Français](INSTALL-SANDBOXIE-PLUS.fr.md) · [Türkçe](INSTALL-SANDBOXIE-PLUS.tr.md) · [Bahasa Indonesia](INSTALL-SANDBOXIE-PLUS.id.md) · [Tiếng Việt](INSTALL-SANDBOXIE-PLUS.vi.md) · [हिन्दी](INSTALL-SANDBOXIE-PLUS.hi.md) · **中文** · [العربية](INSTALL-SANDBOXIE-PLUS.ar.md)

---

FarmPanel 将每个账号保存在各自的 **sandbox**（沙盒）中——一个隔离的环境，让 Steam 和 CS2 不会与其他账号相互串扰。这种隔离由一款名为 **Sandboxie-Plus** 的免费程序负责。你只需在开始于 FarmPanel 中启动账号之前安装它一次。

本指南带你分步完成安装。并不复杂——只需几分钟。

> **简而言之。**下载 **Sandboxie-Plus 1.17.5** 安装程序 → 运行 → 接受默认设置 → 允许安装（需要管理员权限）→ 完成。

> **重要。**与 FarmPanel 本身不同，Sandboxie-Plus 安装时**需要管理员权限**——这是正常的，因为该程序会深入集成到 Windows 中，以可靠地隔离应用程序。

## 目录

1. [你需要准备什么](#你需要准备什么)
2. [步骤 1. 下载安装程序](#步骤-1-下载安装程序)
3. [步骤 2. 运行安装](#步骤-2-运行安装)
4. [步骤 3. 完成安装向导](#步骤-3-完成安装向导)
5. [步骤 4. 首次启动 Sandboxie-Plus](#步骤-4-首次启动-sandboxie-plus)
6. [步骤 5. 确认一切正常](#步骤-5-确认一切正常)
7. [步骤 6. 将它连接到 FarmPanel](#步骤-6-将它连接到-farmpanel)
8. [如何卸载 Sandboxie-Plus](#如何卸载-sandboxie-plus)
9. [疑难解答](#疑难解答)
10. [常见问题](#常见问题)

---

# 你需要准备什么

- **一台运行 Windows 10 或 11 的电脑**（64 位）。
- **这台电脑的管理员权限**（安装时会出现一个提示——你需要点击**是**）。
- **网络连接**——用于下载程序。
- **大约 5 分钟的时间。**

> Sandboxie-Plus 是免费的。一些额外功能面向支持该项目的人，但使用 FarmPanel **并不需要**它们——普通的免费版本就够了。

---

# 步骤 1. 下载安装程序

1. 打开你所需版本的官方页面：
   **[GitHub 上的 Sandboxie-Plus 1.17.5](https://github.com/sandboxie-plus/Sandboxie/releases/tag/v1.17.5)**
2. 向下滚动到 **Assets** 部分。
3. 找到并下载名称类似 **`Sandboxie-Plus-x64-v1.17.5.exe`** 的文件——这是面向普通 64 位 Windows 的安装程序。

**如何选择正确的文件：**

| 文件 | 适合谁 |
|---|---|
| **`Sandboxie-Plus-x64-v1.17.5.exe`** | **大多数用户**——使用 Intel 或 AMD 处理器的普通 Windows。下载这个。 |
| `Sandboxie-Plus-arm64-v1.17.5.exe` | 仅适用于 ARM 处理器的电脑（少见）。 |
| `Sandboxie-Classic-…` | 旧界面版本。FarmPanel **不需要**——请选择 **Plus**。 |
| `.7z` 文件 | 面向高级用户的便携版。安装**不需要**。 |

**接下来会发生什么。**文件出现在你的**下载**（Downloads）文件夹中。

> **提示。**只从上面链接的官方 GitHub 页面下载安装程序。这样你得到的是真实、经过验证的版本。

![带有 Assets 部分的 1.17.5 发布页面](../images/sandboxie/github-release-assets.png)

---

# 步骤 2. 运行安装

1. 打开**下载**文件夹，双击已下载的 **`Sandboxie-Plus-x64-v1.17.5.exe`** 文件。
2. Windows 会显示提示 **“你要允许此应用对你的设备进行更改吗？”**——点击**是**。这就是管理员权限提示；没有它，Sandboxie-Plus 无法安装。

> **如果出现蓝色的 SmartScreen 窗口**（“Windows 已保护你的电脑”）——点击**更多信息**，然后点击**仍要运行**。这是已下载程序的常见警告，并非错误。

**接下来会发生什么。**安装向导窗口打开。

---

# 步骤 3. 完成安装向导

安装向导会带你完成几个简单的界面。大多数情况下，你只需把所有内容保持默认并点击 **Next**。

1. **语言选择。**如果出现语言选择窗口，选择中文（或你的语言）并点击 **OK**。
2. **许可协议。**阅读后点击 **I Agree** 或 **Next**。
3. **安装文件夹。**保留默认文件夹（`C:\Program Files\Sandboxie-Plus`）并点击 **Next**。无需更改。
4. **安装选项。**无需更改任何内容——直接点击 **Next** / **Install**。
5. 等待完成。安装不到一分钟。
6. 在最后一个界面点击 **Finish**。如果有“启动 Sandboxie-Plus”的复选框，请保持勾选。

**接下来会发生什么。**Sandboxie-Plus 完成安装，其图标出现在桌面和开始菜单中。程序通常在安装后立即打开。

> **需要重启吗？**通常不需要。但如果向导要求重启电脑，请照做，以便隔离正常工作。

![带有默认文件夹的安装向导界面](../images/sandboxie/installer-wizard.png)

---

# 步骤 4. 首次启动 Sandboxie-Plus

首次打开 Sandboxie-Plus 时，它会显示一个 **Setup Wizard**（设置向导）。请逐步完成——只需照下面所述操作即可。

如果在向导之前出现**界面语言选择**窗口，请选择你的语言并点击 **OK**。

随后向导会带你完成几个界面。

### 界面 1 — Introduction

选择 **“Personally, for private non-commercial use”**（个人非商业用途）并点击 **Next**。

![Setup Wizard — 已选择 “Personally, for private non-commercial use” 的 Introduction 界面](../images/sandboxie/wizard-1-introduction.png)

### 界面 2 — Support certificate

将该字段**留空**并点击 **Next**。使用 FarmPanel 不需要证书。

![Setup Wizard — 字段留空的 Support certificate 界面](../images/sandboxie/wizard-2-support-certificate.png)

### 界面 3 — Configure UI

将各项值保持**默认**（**Advanced UI for experts** 已被选中）并点击 **Next**。

![Setup Wizard — 采用默认值的界面配置界面](../images/sandboxie/wizard-3-ui-configuration.png)

### 界面 4 — Shell integration

**取消勾选所有复选框**并点击 **Next**。

![Setup Wizard — 所有复选框已取消勾选的 Shell integration 界面](../images/sandboxie/wizard-4-shell-integration.png)

### 界面 5 — Updater

**取消勾选所有复选框**并点击 **Next**。

![Setup Wizard — 所有复选框已取消勾选的 Updater 界面](../images/sandboxie/wizard-5-updater.png)

### 界面 6 — Complete

点击 **Finish** 以应用设置并关闭向导。

![Setup Wizard — 带有 Finish 按钮的最终界面](../images/sandboxie/wizard-6-complete.png)

> **提示。**如果在任何界面拿不定主意，就取消勾选复选框并点击 **Next**。FarmPanel 不需要额外的集成或更新提醒。

**接下来会发生什么。**Sandboxie-Plus 主窗口打开——沙盒列表和控制面板。

![首次启动后的 Sandboxie-Plus 主窗口](../images/sandboxie/main-window.png)

---

# 步骤 5. 确认一切正常

确认 Sandboxie-Plus 已正确安装：

1. 打开 Sandboxie-Plus（桌面或开始菜单中的图标）。
2. 主窗口显示一个沙盒列表——通常有一个名称类似 **DefaultBox** 的默认沙盒。
3. 程序能够打开，且不显示任何错误消息。

如果这些都具备——**Sandboxie-Plus 已安装并可以使用**。

---

# 步骤 6. 将它连接到 FarmPanel

Sandboxie-Plus 安装好后，FarmPanel 就能用它来隔离账号。

1. 打开 **FarmPanel**。
2. 前往 **Settings → Sandboxes**。
3. 确认沙盒文件夹路径已设置。如果该字段为空，请为沙盒选择一个文件夹；如果已填写，则无需更改。
4. 返回 **Accounts** 界面。现在添加账号时，你可以选择沙盒的分配方式（**Auto-assign** 等），并且可以启动账号。

> **它们如何关联。**在 FarmPanel 中，每个账号都必须绑定到一个沙盒，否则无法启动。正是 Sandboxie-Plus 在“幕后”创建并维护这些隔离环境。关于沙盒和启动账号的更多内容，请参见[FarmPanel 用户指南](../user-guide/USER-GUIDE.zh.md)。

**成功的标志。**FarmPanel 中的账号启动并进入 **Running** 状态——这意味着通过 Sandboxie-Plus 的隔离正在生效。

---

# 如何卸载 Sandboxie-Plus

如果你需要移除该程序：

1. 首先，关闭所有在沙盒中运行的程序（在 FarmPanel 中用 **Stop** 停止账号）。
2. 打开 **Windows 设置** → **应用** → **已安装的应用**
   （或“控制面板” → “程序和功能”）。
3. 在列表中找到 **Sandboxie-Plus**。
4. 点击**卸载**并确认。卸载同样需要管理员权限。

> **注意。**移除 Sandboxie-Plus 后，在重新安装该程序之前，FarmPanel 无法启动账号。

---

# 疑难解答

## Windows 不让安装——没有管理员权限

**原因。**Sandboxie-Plus 严格需要管理员权限。

**解决办法。**使用具有管理员权限的账户登录，或请电脑的管理员安装该程序。当出现 **“是否允许更改？”** 提示时，点击**是**。

## 出现 SmartScreen 窗口

**原因。**Windows 会对最近下载的程序发出警告。这并非错误。

**解决办法。**点击**更多信息**，然后点击**仍要运行**。

## 杀毒软件拦截了安装程序

**原因。**部分杀毒软件对集成到系统中的软件较为谨慎。

**解决办法。**
1. 确认你是从官方 GitHub 页面下载的文件（链接见[步骤 1](#步骤-1-下载安装程序)）。
2. 如有需要，临时把文件加入杀毒软件的排除项，然后重新下载。

## 下载了错误的文件

**原因。**发布页面上有多个文件。

**解决办法。**对于普通 Windows，你需要名为 **`Sandboxie-Plus-x64-v1.17.5.exe`** 的文件。不要选择 **arm64**、**Classic** 或 **.7z** 变体。返回[步骤 1](#步骤-1-下载安装程序)并下载正确的文件。

## 安装后 FarmPanel 不启动账号

**解决办法。**
1. 确认 Sandboxie-Plus 已安装且能打开（见[步骤 5](#步骤-5-确认一切正常)）。
2. 在 FarmPanel 中打开 **Settings → Sandboxes**，检查沙盒文件夹路径是否已设置。
3. 重启 FarmPanel。
4. 如果问题仍在，请联系支持（见[常见问题](#常见问题)）。

## 安装后电脑要求重启

**解决办法。**重启电脑——这会完成安装并启用隔离。重启后，再次打开 FarmPanel。

---

# 常见问题

**安装 Sandboxie-Plus 是必需的吗？**
是的，如果你想在 FarmPanel 中启动账号。正是 Sandboxie-Plus 在各自独立的环境中为每个账号提供隔离。

**Sandboxie-Plus 收费吗？**
不收费，基础版本是免费的，足以配合 FarmPanel 使用。额外功能面向支持该项目的人，但并非必需。

**为什么安装需要管理员权限而 FarmPanel 不需要？**
Sandboxie-Plus 会深入集成到 Windows 中以可靠地隔离程序，所以需要管理员权限。而 FarmPanel 仅为你的用户账户安装，因此不需要。

**我需要自己配置沙盒吗？**
不需要。只需安装 Sandboxie-Plus。FarmPanel 会自动为账号创建并配置沙盒。

**我需要支持者证书（supporter certificate）吗？**
不需要。首次启动时你可以跳过那个界面。FarmPanel 不需要它。

**我应该安装哪个确切版本？**
版本 **1.17.5**——链接见[步骤 1](#步骤-1-下载安装程序)。请正是安装这个版本，以获得与 FarmPanel 可预期的兼容性。

**如果出问题，我该去哪里求助？**
在 Telegram 上联系 FarmPanel 支持：[t.me/farmpanel_cn](https://t.me/farmpanel_cn)。描述问题，如果有，请附上错误消息的文字。

---

安装好 Sandboxie-Plus 后，返回[FarmPanel 安装指南](../install-guide/INSTALL-GUIDE.zh.md)，或直接前往[用户指南](../user-guide/USER-GUIDE.zh.md)，添加账号并启动你的第一个农场。

*Sandboxie-Plus 安装指南到此结束。*
