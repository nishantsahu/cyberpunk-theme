# Cyberpunk Theme

A cyberpunk-inspired VS Code theme featuring a vibrant color palette with red, cyan, dark grey, and green accents.

## Color Palette

- **Red** (#ff0000): Used for errors, warnings, and accent elements
- **Bright Cyan** (#00ffff): Used for keywords, functions, and highlights
- **Dark Grey** (#1a1a1a): Used for backgrounds
- **Dark Green** (#00aa00): Used for strings and comments
- **Red** (#ff0000): Used for warnings and destructive actions

## Features

- Dark theme optimized for long coding sessions
- High contrast syntax highlighting
- Cyberpunk aesthetic with neon-like colors
- Full support for all VS Code UI elements
- Terminal color scheme included

## Installation

1. Copy this folder to your VS Code extensions directory:

   - Windows: `%USERPROFILE%\.vscode\extensions\`
   - macOS: `~/.vscode/extensions/`
   - Linux: `~/.vscode/extensions/`

2. Restart VS Code

3. Select the theme: `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS) → "Preferences: Color Theme" → "Cyberpunk"

## Development

To modify the theme, edit `themes/cyberpunk-theme.json` and reload VS Code.

## License

MIT

## Publishing

This repository is prepared to be packaged and published as a Visual Studio Code theme extension.

Before publishing, update the `publisher` field in `package.json` to your Marketplace publisher id (often your GitHub username).

Recommended steps to package and publish:

1. Install vsce (packager) locally or use npx:

   ```bash
   npm install -g vsce    # optional, or use npx in the commands below
   ```

2. Ensure you have a 128x128 PNG icon at `images/icon.png`. A placeholder file is referenced in `package.json` — add your artwork there.

3. Package the extension:

   ```bash
   npm run package
   # or
   npx vsce package
   ```

4. Publish the extension (you need a Personal Access Token and to have created a publisher):

   ```bash
   npm run publish
   # or
   npx vsce publish
   ```

Notes:

- If you prefer not to install `vsce` globally, the `package` and `publish` scripts use `npx` so you can run them without a global install.
- Update `repository.url` and `publisher` in `package.json` to reflect your settings before publishing.
