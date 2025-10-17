# CLI Tools Configuration

Configuration files for command-line tools and terminal utilities.

## 📂 Structure

- **git/** - Git configuration and aliases
- **bash/** - Bash shell configuration
- **zsh/** - Zsh shell configuration
- **tmux/** - Tmux terminal multiplexer
- **vim/** - Vim editor configuration

## 🔧 Setup Instructions

### Git

```bash
# Link global git config
ln -s $(pwd)/git/.gitconfig ~/.gitconfig

# Link global gitignore
ln -s $(pwd)/git/.gitignore_global ~/.gitignore_global
```

### Bash

```bash
# Link bashrc
ln -s $(pwd)/bash/.bashrc ~/.bashrc

# Link bash_profile (macOS)
ln -s $(pwd)/bash/.bash_profile ~/.bash_profile
```

### Zsh

```bash
# Link zshrc
ln -s $(pwd)/zsh/.zshrc ~/.zshrc

# For oh-my-zsh custom configurations
ln -s $(pwd)/zsh/custom ~/.oh-my-zsh/custom
```

### Tmux

```bash
# Link tmux config
ln -s $(pwd)/tmux/.tmux.conf ~/.tmux.conf
```

### Vim

```bash
# Link vimrc
ln -s $(pwd)/vim/.vimrc ~/.vimrc

# Link vim directory (for plugins)
ln -s $(pwd)/vim/.vim ~/.vim
```

## 📝 What to Include

- Configuration files (`.bashrc`, `.zshrc`, `.gitconfig`, etc.)
- Aliases and functions
- Environment variables (use `.env.example` for sensitive data)
- Custom scripts sourced by shell
- Plugin configurations
- Color schemes and themes

## ⚠️ Important

- Never commit sensitive data (API keys, tokens, passwords)
- Use `.env.example` files to document required environment variables
- Test configurations on a new shell session before committing
