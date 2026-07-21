# Changelog

All notable changes to the **Absolutely Theme** extension will be documented in this file.

## [Unreleased]

### Added

- Added dedicated colors for the VS Code Modern UI floating surfaces and the Agents window, including panels, chat inputs, badges, progress states, and charts.
- Added explicit colors for staged Git resources, unfocused tabs, Peek views, activity badges, comments, and newer quick input states.

### Changed

- Prioritized Absolutely Light as the primary light palette, while keeping Absolutely Light Warm aligned to the same syntax and foreground system with warmer surfaces.
- Improved button contrast, variable and property hierarchy, inlay hints, ghost text, selection states, and bright terminal ANSI colors across both light variants.
- Aligned dark-theme variables with the light themes' neutral variable hierarchy.
- Added a brighter editor canvas to both light variants so the sidebar, title bar, and panel retain a clear but comfortable surface contrast in Modern UI, while borders, scrollbars, and indentation guides remain visually restrained.
- Raised the minimum supported VS Code version to 1.129 so Modern UI theme colors use the matching public color schema.
- Restored restrained accent focus rings so keyboard navigation remains visible without changing the theme's calm visual direction.
- Separated editor, floating-panel, and elevated surfaces for clearer hierarchy in Modern UI.
- Unified syntax roles across variants: functions remain distinct from HTML tags, and Vue component colors now agree between semantic and TextMate highlighting.
- Added recommended Modern UI settings to the README.

### Removed

- Removed the Absolutely Dark Warm variant to keep the theme family focused on Absolutely Light, Absolutely Light Warm, and Absolutely Dark.

## [0.1.0] - 2026-06-20

### Changed

- Improved terminal readability across light and dark variants, especially low-contrast ANSI output and selection states.
- Increased readability for low-priority editor text such as line numbers, CodeLens, placeholders, inactive tabs, and inline Git blame.
- Switched inline Git blame decoration to a quieter gray treatment.
- Kept borders and secondary UI elements restrained so non-essential areas remain calm and do not draw too much attention.

## [0.0.8] - 2026-06-17

### Added

- Added **Absolutely Dark Warm**, a warmer yellow-leaning dark theme variant.

### Changed

- Removed strong focus/selection borders from menus, quick pick lists, and related popup surfaces.
- Switched selected rows in menus and pickers to a deeper quiet gray while keeping panel surfaces unchanged.

## [0.0.7] - 2026-06-17

### Changed

- Refined light, warm light, and dark theme colors for better readability and a cleaner editor experience.
- Improved Vue syntax highlighting to better distinguish components, HTML tags, attributes, class values, variables, functions, and strings.
- Increased Git decoration and SCM graph color contrast for clearer changed-file and history states.
- Softened UI border colors to reduce visual noise while keeping editor structure readable.
- Updated `README.md` to reflect the current theme direction, palette, and highlighting improvements.

## [0.0.6] - 2026-06-14

### Changed

- Updated the extension icon (`icon.png`) to have a transparent background for a cleaner appearance on the VS Code Marketplace and in extension settings.

## [0.0.5] - 2026-06-14

### Added

- Added repository, homepage, and issues URLs to `package.json` for better marketplace integration.
- Added comprehensive search keywords/tags to improve discoverability on the marketplace.

### Changed

- Refined the extension description for clarity and professionalism.

## [0.0.4] - 2026-06-14

### Fixed

- Adjusted editor overview ruler and editor margin colors across all theme variants to improve readability.
- Fixed focus border and background color configurations for better UI consistency.
- Updated marketplace badge URLs in `README.md` to show correct metrics.

## [0.0.3] - 2026-06-14

### Added

- Initial release of the theme family, introducing three variants:
  - **Absolutely Light**: Soft, clean light theme to reduce glare.
  - **Absolutely Light Warm**: Warm-toned light theme resembling physical book paper.
  - **Absolutely Dark**: Muted, low-contrast dark theme designed to soothe the eyes.
