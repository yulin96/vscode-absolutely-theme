# Absolutely Theme

A clean, calm, and readable color theme family for Visual Studio Code, inspired by warm paper tones and modern coding tools.

Absolutely Theme balances comfort with clarity: soft backgrounds, readable contrast, clearer Git colors, and carefully separated Vue / HTML syntax highlighting for long coding sessions.

[![Marketplace Version](https://vsmarketplacebadges.dev/version/yulin96.vscode-absolutely-theme.svg?color=B8674C)](https://marketplace.visualstudio.com/items?itemName=yulin96.vscode-absolutely-theme)
[![Installs](https://vsmarketplacebadges.dev/installs/yulin96.vscode-absolutely-theme.svg?color=B8674C)](https://marketplace.visualstudio.com/items?itemName=yulin96.vscode-absolutely-theme)
[![Rating](https://vsmarketplacebadges.dev/rating/yulin96.vscode-absolutely-theme.svg?color=B8674C)](https://marketplace.visualstudio.com/items?itemName=yulin96.vscode-absolutely-theme)
[![License](https://img.shields.io/github/license/yulin96/vscode-absolutely-theme?color=B8674C)](https://github.com/yulin96/vscode-absolutely-theme/blob/main/LICENSE)

---

## 🎨 Theme Variants

Absolutely Theme includes four balanced variants for different lighting conditions:

| Variant                   | Type  | Description                                                           | Background |  Accent   |
| :------------------------ | :---- | :-------------------------------------------------------------------- | :--------: | :-------: |
| **Absolutely Light**      | Light | A clean light theme with soft contrast and crisp editor UI.           | `#FAF8F3`  | `#B8674C` |
| **Absolutely Light Warm** | Light | A warmer paper-like light theme with the same readable syntax system. | `#FAF6ED`  | `#B8674C` |
| **Absolutely Dark**       | Dark  | A calm dark theme with warm neutrals and clearer code/Git colors.     | `#252522`  | `#D98666` |
| **Absolutely Dark Warm**  | Dark  | A warmer dark theme with a yellow-leaning editor surface.             | `#1F1D18`  | `#C79D45` |

---

## ✨ Highlights

- Clearer Vue syntax highlighting: components, HTML tags, attributes, class values, variables, functions, and strings are easier to tell apart.
- More readable Git colors for modified, added, deleted, untracked, and history graph states.
- Softer borders and cleaner editor surfaces to keep the interface calm without making it blurry.
- Quieter gray selection states to reduce distraction without changing panel surfaces.
- Consistent light, warm light, dark, and dark warm variants.

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
