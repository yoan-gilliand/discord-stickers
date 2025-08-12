# GitHub Stickers Panel

A **Vencord plugin** that adds a **GitHub** tab inside Discord’s native sticker picker, allowing you to **manage, send, and delete** stickers hosted in a public GitHub repository.

## ✨ Features

- 📂 **List** stickers stored in the `stickers` folder of a GitHub repository.
- ⬆️ **Upload** new stickers directly to the repository from within Discord.
- 🗑 **Delete** stickers from the repository via a right-click context menu.
- 💬 **Send** stickers to a Discord channel (temporarily uploaded and automatically deleted after sending).
- 🔄 **Automatically refresh** the sticker list after changes.

## 📦 Installation

### 1. Prerequisites
- **Vencord with custom plugin support** (meaning you must "Install from Source").
  - [Vencord Installation](https://docs.vencord.dev/installing/)
  - [Custom Plugins](https://docs.vencord.dev/installing/custom-plugins/)
- A **public GitHub repository** with a `stickers` folder.
- A **GitHub Personal Access Token** with the `repo` scope.

### 2. Adding the plugin
1. Download `GitHubStickersPanel.tsx`.
2. Place it in your **Vencord custom plugins folder**.
3. Reload or rebuild Vencord so the plugin is recognized.

### 3. Configuration
In Vencord’s settings, configure:
- **GitHub token** → Your GitHub personal token (`ghp_...`)
- **GitHub repo** → Format: `owner/repo`
- **GitHub branch** → Defaults to `main`
- **Target Guild ID** (optional) → The Discord server ID for hosting stickers.

## 🖱 Usage

1. Open the **sticker picker** in Discord.
2. Click the **GitHub** tab.
3. From here, you can:
   - **Upload** a sticker with the `+` button.
   - **Send** a sticker by clicking it.
   - **Delete** a sticker with **right-click → Delete**.

## ⚙️ Technical Constraints

- Accepted formats: PNG, APNG, GIF.
- Maximum file size: **512 KiB**.
- Name length: 2–30 characters (filename without extension).

## 📜 License

Provided as-is, without warranty.  
