# IDE Settings

This directory contains configuration files for various Integrated Development Environments (IDEs) and code editors.

## 📂 Structure

- **vscode/** - Visual Studio Code settings and extensions
- **intellij/** - IntelliJ IDEA settings and plugins
- **sublime/** - Sublime Text preferences and packages
- **vim/** - Vim/Neovim configurations

## 🔧 Setup Instructions

### Visual Studio Code

1. Settings location:
   - **macOS**: `~/Library/Application Support/Code/User/`
   - **Linux**: `~/.config/Code/User/`
   - **Windows**: `%APPDATA%\Code\User\`

2. Symlink settings:
   ```bash
   ln -s $(pwd)/vscode/settings.json ~/Library/Application\ Support/Code/User/settings.json
   ln -s $(pwd)/vscode/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
   ```

### IntelliJ IDEA

1. Export settings: File → Manage IDE Settings → Export Settings
2. Import settings: File → Manage IDE Settings → Import Settings
3. Or copy to the appropriate config directory

### Sublime Text

1. Settings location:
   - **macOS**: `~/Library/Application Support/Sublime Text/Packages/User/`
   - **Linux**: `~/.config/sublime-text/Packages/User/`
   - **Windows**: `%APPDATA%\Sublime Text\Packages\User\`

### Vim

1. Copy `.vimrc` to home directory:
   ```bash
   ln -s $(pwd)/vim/.vimrc ~/.vimrc
   ```

## 📝 What to Include

- User settings/preferences
- Keyboard shortcuts
- Extensions/plugins list
- Code snippets
- Color themes (if custom)
- Workspace settings templates
