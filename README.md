
# Developer's Theme + iPhonePlay's Crystal Files

**Original project:** [Developer's Theme by Rajeshwaran](https://github.com/Rajeshwaran2001/developer-theme-dark)

This fork preserves Developer's Theme and extends its file icon theme with custom icons for **iPhonePlay's Crystal programming language**.

## 💎 iPhonePlay's Crystal Language Icons

Three custom icons have been added to the original file icon theme.

| Icon | File association | Description |
|---|---|---|
| ![Crystal source icon](icons/crystal.png) | `.crst` | Source files for iPhonePlay's Crystal language |
| ![Crystal project icon](icons/crystalize.png) | `.crstproj` | Project files for iPhonePlay's Crystal language |
| ![MakeCrystal utility icon](icons/makecrystal.png) | `MakeCrystal` | The MakeCrystal utility |

### Icon files

**`icons/crystal.png`** — Used for `.crst` source files.

**`icons/crystalize.png`** — Used for `.crstproj` project files.

**`icons/makecrystal.png`** — Used for files named exactly `MakeCrystal`.

> **Important:** Crystal in this repository refers to iPhonePlay's own programming language. It does not refer to the unrelated Crystal programming language project.

## Installation

### Install the packaged extension

1. Download or clone this repository.
2. Open a terminal in the repository directory.
3. Install Microsoft's VS Code extension packaging tool if it is not already installed:

   ```powershell
   npm install --global @vscode/vsce
   ```

4. Package the extension:

   ```powershell
   vsce package --allow-missing-repository
   ```

5. Install the generated VSIX file in VS Code. The expected filename for version `6.0.0` is:

   ```powershell
   code --install-extension .\developer-theme-crystal-files-6.0.0.vsix
   ```

6. Open the Command Palette with `Ctrl+Shift+P`.
7. Select **Preferences: File Icon Theme**.
8. Choose **Rajeshwaran Developer's Theme + iPhonePlay's Crystal Files**.

The theme combines the original Developer's file icons with the three additional Crystal mappings.

## Original project

### Developer's theme

VS Code theme for developers.

> A dark theme for [Visual Studio Code](https://code.visualstudio.com/).
>
> For GitHub Actions, refer to [publish-vscode-extension](https://github.com/HaaLeo/publish-vscode-extension).

<p align="center">
  <a href="https://marketplace.visualstudio.com/items?itemName=Rajeshwaran.developer-theme-dark"><img src="https://img.shields.io/visual-studio-marketplace/v/Rajeshwaran.developer-theme-dark?style=for-the-badge&colorA=252526&colorB=43A047&label=VERSION" alt="Version"></a>&nbsp;
  <a href="https://marketplace.visualstudio.com/items?itemName=Rajeshwaran.developer-theme-dark"><img src="https://img.shields.io/visual-studio-marketplace/stars/Rajeshwaran.developer-theme-dark?style=for-the-badge&colorA=252526&colorB=43A047&label=RATING" alt="Rating"></a>&nbsp;
  <a href="https://marketplace.visualstudio.com/items?itemName=Rajeshwaran.developer-theme-dark"><img src="https://img.shields.io/visual-studio-marketplace/i/Rajeshwaran.developer-theme-dark?style=for-the-badge&colorA=252526&colorB=43A047&label=INSTALLS" alt="Installs"></a>&nbsp;
  <a href="https://marketplace.visualstudio.com/items?itemName=Rajeshwaran.developer-theme-dark"><img src="https://img.shields.io/visual-studio-marketplace/d/Rajeshwaran.developer-theme-dark?style=for-the-badge&colorA=252526&colorB=43A047&label=DOWNLOADS" alt="Downloads"></a>&nbsp;
  <a href="https://github.com/Rajeshwaran2001/developer-theme-dark/issues"><img src="https://img.shields.io/github/issues/Rajeshwaran2001/developer-theme-dark?style=for-the-badge&colorA=252526&colorB=43A047&label=GitHub%20issues" alt="GitHub issues"></a>&nbsp;
  <a href="https://github.com/Rajeshwaran2001/developer-theme-dark/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Rajeshwaran2001/developer-theme-dark?style=for-the-badge&colorA=252526&colorB=43A047&label=LICENSE" alt="License"></a>&nbsp;
  <a href="https://vscode.dev/theme/Rajeshwaran.developer-theme-dark"><img src="https://img.shields.io/badge/preview%20in-vscode.dev-blue?style=for-the-badge&colorA=252526&colorB=43A047&label=PREVIEW" alt="Preview"></a>&nbsp;
  <a href="https://discord.gg/N9WdqHdmC"><img src="https://img.shields.io/badge/Discord-Join%20Community?style=for-the-badge&colorA=252526&colorB=5865F2&logo=discord&logoColor=white" alt="Discord"></a>
</p>

## Preview of themes and colors

> Not too bright and not too subtle.

### Developer's Theme

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/theme.webp" alt="Developer's Theme preview">

### Firefox Dark

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/FirefoxDark.webp" alt="Firefox Dark">

### Ocean Dark

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/OceanDark.webp" alt="Ocean Dark">

### Slack Dark

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/SlackDark.webp" alt="Slack Dark">

### Green Coffee

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/GreenCoffee.webp" alt="Green Coffee">

### Aubergine Dark

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/AubergineDark.webp" alt="Aubergine Dark">

### Product icons

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/preview.png" alt="Product icons">

### File icons

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/fileIcons.png" alt="Original file icons">

### Folder icons

<img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/folderIcons.png" alt="Folder icons">

## Development

The original project specifies **Node.js 22 or newer** in `.nvmrc`; npm 10 or newer is included with Node.js 22.

Install dependencies and run the original project's development scripts when needed:

```bash
npm ci
npm run build
npm test
```

Useful individual scripts from the original project:

| Script | Description |
|---|---|
| `npm run lint` / `npm run lint:fix` | Run ESLint or automatically fix supported issues |
| `npm run typecheck` | Run TypeScript checks without emitting files |
| `npm run format` / `npm run format:check` | Format or check formatting with Prettier |
| `npm run svgo-p` | Optimize product icons in `Pro-icons/` |
| `npm run svgo-mf` | Optimize file and folder icons in `icons/` |
| `npm run fonts` | Rebuild the icon font using Fantasticon |
| `npm run preview` | Regenerate file and folder icon preview images |
| `npm run package` | Build a VSIX package |

The icon font's codepoints live in `src/scripts/template/mapping.json` and must stay synchronized with the `fontCharacter` values in `product_icons/developer's-icons.json`. Changing a codepoint can change glyphs for existing theme users.

> **Running `npm test` from the VS Code integrated terminal?** VS Code exports `ELECTRON_RUN_AS_NODE=1`, which can prevent the downloaded test instance from launching with its required flags. On compatible Unix environments, try `env -u ELECTRON_RUN_AS_NODE npm test`.

The three Crystal icon additions are PNG assets referenced by `file_icons/developer-icons.json`.

## Icon sources

The original project credits the following icon sources:

- [Fluent Design Icons](https://fluenticons.co/)
- [Material Design Icons](https://materialdesignicons.com/)
- Official icons

The Crystal icons in this fork were created for iPhonePlay's Crystal language.

## Contributors

Original project contributors:

<a href="https://github.com/Rajeshwaran2001/developer-theme-dark/graphs/contributors">
  <img src="https://raw.githubusercontent.com/Rajeshwaran2001/developer-theme-dark/main/assest/contributors.png" alt="Original project contributors">
</a>

## Credits

- **Original Developer's Theme:** [Rajeshwaran](https://github.com/Rajeshwaran2001/developer-theme-dark).
- **Crystal icons and integration:** iPhonePlay.
- **Original project license:** GPL-3.0.

This repository is a modified version of Developer's Theme. The original project's license and applicable copyright notices must be retained when redistributing the fork. See the included `LICENSE` file for the complete terms.
