# Absolutely Theme

A clean, calm, and readable color theme family for Visual Studio Code, inspired by warm paper tones and modern coding tools.

Absolutely Theme balances comfort with clarity: soft backgrounds, readable contrast, restrained UI color, and carefully separated Vue / HTML syntax highlighting for long coding sessions.

[![Marketplace Version](https://vsmarketplacebadges.dev/version/yulin96.vscode-absolutely-theme.svg?color=B8674C)](https://marketplace.visualstudio.com/items?itemName=yulin96.vscode-absolutely-theme)
[![Installs](https://vsmarketplacebadges.dev/installs/yulin96.vscode-absolutely-theme.svg?color=B8674C)](https://marketplace.visualstudio.com/items?itemName=yulin96.vscode-absolutely-theme)
[![Rating](https://vsmarketplacebadges.dev/rating/yulin96.vscode-absolutely-theme.svg?color=B8674C)](https://marketplace.visualstudio.com/items?itemName=yulin96.vscode-absolutely-theme)
[![License](https://img.shields.io/github/license/yulin96/vscode-absolutely-theme?color=B8674C)](https://github.com/yulin96/vscode-absolutely-theme/blob/main/LICENSE)

---

## 🎨 Theme Variants

Absolutely Theme includes three balanced variants for different lighting conditions:

| Variant                   | Type  | Description                                                           | Background |  Accent   |
| :------------------------ | :---- | :-------------------------------------------------------------------- | :--------: | :-------: |
| **Absolutely Light**      | Light | The primary light theme with neutral warm-white surfaces.             | `#FAF8F3`  | `#A85438` |
| **Absolutely Light Warm** | Light | The same readable color system on warmer paper-like surfaces.         | `#FAF6ED`  | `#A85438` |
| **Absolutely Dark**       | Dark  | A calm dark theme with warm neutrals and clearer code/Git colors.     | `#252522`  | `#D98666` |

---

## ✨ Highlights

- Clearer Vue syntax highlighting: components, HTML tags, attributes, class values, variables, functions, and strings are easier to tell apart.
- More readable Git colors for modified, added, deleted, untracked, and history graph states.
- Cleaner terminal output and readable low-priority editor text, including line numbers, CodeLens, and inline Git blame.
- Restrained selection and border treatment so secondary UI stays calm and does not compete with code.
- Accent colors are reserved for meaningful states like links, cursor, active items, search, and warnings.
- Explicit Modern UI and Agents surfaces with clearer floating-panel separation and visible keyboard focus states.
- Consistent light, warm light, and dark variants.

---

## 🚀 Installation

1. Open **Visual Studio Code**.
2. Open the **Extensions** panel (`Ctrl+Shift+X` or `Cmd+Shift+X`).
3. Search for **`Absolutely Theme`**.
4. Click **Install**.
5. Press `Ctrl+K Ctrl+T` (or `Cmd+K Cmd+T` on macOS) and select your preferred variant from the dropdown menu.

---

## 🛠 Customization & Tips

### Enable Semantic Highlighting

For the best visual experience, make sure semantic highlighting is enabled in your settings:

```json
"editor.semanticHighlighting.enabled": true
```

### Font Recommendations

This theme pairs beautifully with clean monospaced fonts that support ligatures. We recommend:

- [Fira Code](https://github.com/tonsky/FiraCode)
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/)
- [Operator Mono](https://www.typography.com/fonts/operator/styles)

Add this to your `settings.json` for a modern, distraction-free aesthetic:

```json
{
  "editor.lineHeight": 1.6,
  "editor.fontSize": 14,
  "editor.minimap.enabled": false,
  "editor.scrollbar.horizontal": "hidden",
  "workbench.startupEditor": "none"
}
```

### Modern UI Recommendations

VS Code 1.129 introduced an experimental modern workbench with floating, rounded panels. Absolutely Theme includes dedicated surface, border, input, badge, and status colors for this layout.

This version of Absolutely Theme requires VS Code 1.129 or later so all Modern UI color tokens are validated and applied consistently.

For a compact horizontal layout:

```json
{
  "workbench.experimental.modernUI": true,
  "workbench.activityBar.location": "top",
  "workbench.activityBar.autoHide": false,
  "workbench.shadows": false,
  "window.customTitleBarVisibility": "auto",
  "window.commandCenter": true,
  "workbench.layoutControl.enabled": true,
  "workbench.layoutControl.type": "toggles"
}
```

If you prefer the traditional vertical Activity Bar, use its compact size instead:

```json
{
  "workbench.activityBar.location": "default",
  "workbench.activityBar.compact": true
}
```

`workbench.activityBar.compact` only affects the vertical Activity Bar. Modern UI is still experimental, so its layout may change in future VS Code releases.

### Override Colors

Want to tweak the background or another specific color? You can override any theme color in your user settings:

```json
"workbench.colorCustomizations": {
  "[Absolutely Dark]": {
    "editor.background": "#1E1E1C"
  }
}
```

---

## 📄 License & Credits

This project is licensed under the [MIT License](LICENSE).

Developed and designed with ❤️ by [yulin96](https://github.com/yulin96).
