<div align="center">
<table>
  <tr>
    <td>
      <p align="center">
        <img src="./icon-512x512.svg" alt="Vesper Icon" width="100">
      </p>
      <h1 align="center">Welcome to the Vesper Project</h1>
      <p align="center">
        Your persistent, predictable, terminal workspace.
        <br />
        <a href="https://www.vesper.sh"><strong>Visit the Website »</strong></a>
      </p>
      <p align="center">
        <!--a href="https://github.com/vesper-app/vesper/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/vesper-app/vesper/ci.yml?branch=main&style=for-the-badge" alt="Build Status"></a>
        <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/github/license/vesper-app/vesper?style=for-the-badge" alt="License: MIT"></a>
        <a href="https://github.com/vesper-app/vesper/releases"><img src="https://img.shields.io/github/v/release/vesper-app/vesper?style=for-the-badge" alt="Latest Release"></a-->
        <a href="https://discord.gg/DFEgkv3MkU"><img src="https://img.shields.io/badge/Community-Join_the_Conversation-C792EA?style=for-the-badge&logo=discord" alt="Discord Community"></a>
      </p>
    </td>
  </tr>
</table>
</div>

---

## 🚀 Installation

The recommended way to install Vesper is via a package manager. For detailed, OS-specific instructions and a fallback guide for building from source, please see the **[Official Installation Guide](https://www.vesper.sh/docs/install.html)** on our website.

### macOS & Linux (Homebrew)
```bash
brew tap vesper-app/vesper
brew install vesper
```

### Arch Linux (AUR)
```bash
yay -S vesper-git
```

## ✨ Why Vesper?

*   **True Remote Integration:** Stop the "double prefix dance." Vesper's native remote tabs integrate remote connections directly into your local workspace for a seamless experience.
*   **A Scriptable Environment with Lua:** Use the powerful Lua API to dynamically set environment variables for every new pane. Securely load API tokens, automate your shell setup, and more.
*   **Flexible Configuration:** Use a simple `.ini` file for easy setup and a powerful `init.lua` file for deep, programmatic control—a skill that transfers across the developer ecosystem.
*   **A Clipboard That Just Works:** Direct, out-of-the-box access to your system clipboard. No configuration, no buffer juggling.
*   **Flexible Layouts with Floating Panes:** Toggle any tiled pane into a floating overlay for quick tasks without disrupting your main layout.

➡️ **[See a detailed comparison with Tmux on our website.](https://www.vesper.sh/vs-tmux.html)**

## ⚡ Quickstart

Vesper uses a **<kbd>Ctrl</kbd>+<kbd>a</kbd>** prefix for all commands. Press the prefix, release, then press the desired key.

| Action | Keybinding Sequence |
| :--- | :--- |
| **Split Vertically** | <kbd>Ctrl</kbd>+<kbd>a</kbd> then <kbd>v</kbd> |
| **Split Horizontally**| <kbd>Ctrl</kbd>+<kbd>a</kbd> then <kbd>h</kbd> |
| **Navigate Panes** | <kbd>Ctrl</kbd>+<kbd>a</kbd> then <kbd>h</kbd>/<kbd>j</kbd>/<kbd>k</kbd>/<kbd>l</kbd> |
| **New Tab** | <kbd>Ctrl</kbd>+<kbd>a</kbd> then <kbd>c</kbd> |
| **Detach Session** | <kbd>Ctrl</kbd>+<kbd>a</kbd> then <kbd>d</kbd> |

➡️ **[For a full list of commands, see the Cheatsheet on our website.](https://www.vesper.sh/docs/cheatsheet.html)**

---

## 🤝 Contributing

We welcome contributions of all kinds! The best place to start is by checking out our issues tracker or joining the conversation on our Discord server.

*   **[Read our full Contributing Guide](./CONTRIBUTING.md)** to get your development environment set up.
*   **[Propose a new feature](https://github.com/vesper-app/vesper/issues/new?template=feature_proposal.yml)** or **[report a bug](https://github.com/vesper-app/vesper/issues/new?template=bug_report.yml)**.
*   **[Join the community on Discord](https://discord.gg/DFEgkv3MkU)** to ask questions and get involved.

## 📄 License

Vesper is open-source software licensed under the [MIT License](./LICENSE).
