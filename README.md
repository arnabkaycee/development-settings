# Development Settings

A comprehensive repository for managing personal development environment settings, configurations, scripts, and resources.

## 📁 Repository Structure

```
development-settings/
├── ide-settings/          # IDE and editor configurations
│   ├── vscode/           # Visual Studio Code settings
│   ├── intellij/         # IntelliJ IDEA settings
│   ├── sublime/          # Sublime Text settings
│   └── vim/              # Vim configurations
├── cli-tools/            # Command-line tool configurations
│   ├── git/              # Git configurations (.gitconfig, etc.)
│   ├── bash/             # Bash configurations (.bashrc, etc.)
│   ├── zsh/              # Zsh configurations (.zshrc, etc.)
│   ├── tmux/             # Tmux configurations
│   └── vim/              # Vim/Neovim configurations
├── prompts/              # Development prompts and templates
│   ├── ai-prompts/       # AI assistant prompts for development
│   └── code-templates/   # Code snippets and templates
├── notes/                # Development notes and documentation
├── scripts/              # Useful utility scripts
│   ├── setup/            # Setup and installation scripts
│   ├── productivity/     # Productivity and workflow scripts
│   └── maintenance/      # System maintenance scripts
└── startup-configs/      # Startup configuration files
```

## 🚀 Quick Start

### Installation

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/development-settings.git
cd development-settings
```

> **Note**: Replace `YOUR_USERNAME` with your GitHub username

2. Run the setup script (if available):
```bash
./scripts/setup/install.sh
```

### Manual Setup

You can manually symlink specific configurations:

```bash
# Example: Link git configuration
ln -s $(pwd)/cli-tools/git/.gitconfig ~/.gitconfig

# Example: Link VSCode settings
ln -s $(pwd)/ide-settings/vscode/settings.json ~/Library/Application\ Support/Code/User/settings.json
```

## 📖 Usage

### IDE Settings

Navigate to the `ide-settings/` directory for IDE-specific configurations:
- **VSCode**: User settings, keybindings, extensions list
- **IntelliJ**: IDE settings, plugins, code styles
- **Sublime**: Preferences, key bindings, packages
- **Vim**: `.vimrc` and plugin configurations

### CLI Tools

The `cli-tools/` directory contains configurations for various command-line tools:
- **Git**: Global git configuration, aliases, and ignore patterns
- **Bash/Zsh**: Shell configurations, aliases, and functions
- **Tmux**: Terminal multiplexer settings
- **Vim**: Editor configurations and plugins

### Prompts

The `prompts/` directory includes:
- **AI Prompts**: Pre-written prompts for AI coding assistants
- **Code Templates**: Reusable code snippets and boilerplate

### Scripts

Utility scripts in the `scripts/` directory:
- **Setup**: Automated installation and configuration scripts
- **Productivity**: Workflow automation and shortcuts
- **Maintenance**: System cleanup and maintenance tasks

### Notes

The `notes/` directory contains development-related documentation, learning resources, and personal notes.

## 🔄 Keeping Settings in Sync

### Exporting Settings

When you make changes to your local development environment:

1. Copy updated configurations to this repository
2. Commit and push changes
3. Document any new dependencies or prerequisites

### Importing Settings

On a new machine:

1. Clone this repository
2. Run setup scripts or manually symlink configurations
3. Install required tools and dependencies

## 🤝 Contributing

This is a personal repository, but feel free to:
- Fork it for your own use
- Suggest improvements via issues
- Share your own configurations

## 📝 License

MIT License - See [LICENSE](LICENSE) file for details

## ⚠️ Important Notes

- Review all scripts before executing them
- Backup your existing configurations before applying these settings
- Some configurations may be specific to macOS/Linux/Windows
- Sensitive information (tokens, passwords) should never be committed
- Use `.env.example` files for environment variable templates
