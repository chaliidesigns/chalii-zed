<h1 align="center">⚡ Chalii Themes - Zed</h1>

<p align="center">
  Premium light and dark themes for <a href="https://zed.dev">Zed</a> with warm orange accents and excellent readability.<br>
  The Zed extension port of the <a href="https://github.com/chaliidesigns/chalii-themes">Chalii Themes</a> family, generated from one shared palette.
</p>

<p align="center">
  <a href="#-features">✨ Features</a> •
  <a href="#-quick-start">🚀 Quick Start</a> •
  <a href="#-structure">🏗️ Structure</a> •
  <a href="#-how-it-is-built">🔧 How It Is Built</a> •
  <a href="https://github.com/chaliidesigns/chalii-themes">🧩 Source Repo</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Zed-extension-084CCF?logo=zedindustries&logoColor=white" alt="Zed extension">
  <img src="https://img.shields.io/badge/schema-v1-0e0e0f" alt="schema_version 1">
  <img src="https://img.shields.io/badge/variants-Light%20%2B%20Dark-ff711a" alt="Light + Dark">
  <img src="https://img.shields.io/badge/style%20keys-130%2B-5C2D91" alt="130+ style keys">
  <img src="https://img.shields.io/badge/License-MIT-green" alt="MIT">
</p>

---

## 🌟 Highlights

- ☀️🌙 **Two variants in one extension** - **Chalii Light** and **Chalii Dark**, selectable per appearance with `"theme": { "mode": "system" }`
- 🟠 **Chalii palette** - warm orange accents, purple types, teal strings, deep `#0e0e0f` dark background
- 🧩 **Full Zed theme schema** - 130+ UI style keys (editor, panels, tabs, terminal ANSI colours, git/diagnostic colours), 40+ syntax scopes and a collaboration `players` palette
- 🔁 **Generated from the source palette** - stays in sync with the VS Code, JetBrains, Sublime, Neovim and terminal ports

## ✨ Features

- `extension.toml` manifest (`id = "chalii-themes"`, `schema_version = 1`) ready for the Zed extension registry
- Single `themes/chalii.json` family file containing both variants
- Editor, gutter, scrollbar, search-match, status-bar, title-bar, tab and panel colours
- Terminal ANSI 16-colour set tuned to the brand
- Syntax highlighting for keywords, functions, types, strings, comments, attributes, punctuation and more

## 🚀 Quick Start

### Install as a dev extension (local)

1. Clone this repository.
2. In Zed, open the command palette and run **zed: install dev extension**.
3. Select the cloned `chalii-zed/` directory (the one containing `extension.toml`).
4. Open **zed: open settings** and set:

   ```json
   {
     "theme": {
       "mode": "system",
       "light": "Chalii Light",
       "dark": "Chalii Dark"
     }
   }
   ```

### Install from the registry

Once published to the Zed extension registry:

1. Open the command palette → **zed: extensions**.
2. Search for **Chalii Themes** and click **Install**.
3. Activate via **zed: theme selector**, or use the settings snippet above.

## 🏗️ Structure

```
chalii-zed/
├── extension.toml      # Zed extension manifest (id, name, version, authors, repository)
├── themes/
│   └── chalii.json     # Theme family: Chalii Light + Chalii Dark
├── LICENSE             # MIT
└── README.md
```

## 🔧 How It Is Built

`themes/chalii.json` and `extension.toml` are emitted by `build/zed.mjs` in [chalii-themes](https://github.com/chaliidesigns/chalii-themes) from `source/palette.json`:

```bash
# in chaliidesigns/chalii-themes
npm run build:zed   # writes ports/zed/
```

**Do not edit the generated files here directly** - open issues and pull requests against [chalii-themes](https://github.com/chaliidesigns/chalii-themes/issues), then sync the regenerated output into this repo and tag a release.

## 📄 License

[MIT](LICENSE) © Chalii Designs

## 👤 Author

**Chalii Designs** - design & engineering studio by Chalii wa UX/UI - [@chaliiwaui](https://github.com/chaliiwaui)

- 📧 Email: me@makindajackson.com
- 💼 LinkedIn: [Jackson Makinda](https://linkedin.com/in/makindajack)
- 🎨 Dribbble: [@makindajack](https://dribbble.com/makindajack)
- 🐦 Twitter: [@makindajack](https://twitter.com/makindajack)

Part of the **Chalii** design ecosystem - [Themes](https://github.com/chaliidesigns/chalii-themes) • [Icons](https://github.com/chaliidesigns/chalii-icons) • [Sublime](https://github.com/chaliidesigns/chalii-sublime) • [Obsidian](https://github.com/chaliidesigns/chalii-obsidian) • [Spicetify](https://github.com/chaliidesigns/chalii-spicetify)

---

Built with ❤️ in Dar es Salaam, Tanzania 🇹🇿
