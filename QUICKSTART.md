# Quick Start Guide

Get up and running with your development settings in minutes!

## 🚀 First Time Setup

### 1. Clone the Repository

```bash
git clone https://github.com/arnabkaycee/development-settings.git
cd development-settings
```

### 2. Review the Structure

```bash
# See all available directories
ls -la

# Read the main README
cat README.md
```

### 3. Choose What to Use

The repository is organized into sections:

- **`ide-settings/`** - IDE configurations (VSCode, IntelliJ, etc.)
- **`cli-tools/`** - Shell and CLI tool configs (git, bash, zsh, etc.)
- **`prompts/`** - AI prompts and code templates
- **`notes/`** - Development notes and documentation
- **`scripts/`** - Useful automation scripts
- **`startup-configs/`** - Startup and environment configurations

### 4. Copy Example Files

All template files have `.example` suffix. Copy and customize them:

```bash
# Example: Set up Git configuration
cp cli-tools/git/.gitconfig.example ~/.gitconfig
cp cli-tools/git/.gitignore_global.example ~/.gitignore_global

# Edit with your information
vim ~/.gitconfig  # Change name and email

# Example: Set up Bash configuration
cp cli-tools/bash/.bashrc.example ~/.bashrc
source ~/.bashrc
```

### 5. Use the Scripts

Scripts are in the `scripts/` directory:

```bash
# Make scripts executable (if needed)
chmod +x scripts/setup/*.sh.example

# Review a script before running
cat scripts/setup/setup-dev-env.sh.example

# Run setup scripts (after reviewing)
./scripts/setup/setup-dev-env.sh.example
```

## 📋 Common Tasks

### Setting Up VSCode

```bash
# macOS
cp ide-settings/vscode/settings.json.example ~/Library/Application\ Support/Code/User/settings.json

# Linux
cp ide-settings/vscode/settings.json.example ~/.config/Code/User/settings.json

# Review recommended extensions
cat ide-settings/vscode/extensions.md
```

### Setting Up Git

```bash
# Copy config files
cp cli-tools/git/.gitconfig.example ~/.gitconfig
cp cli-tools/git/.gitignore_global.example ~/.gitignore_global

# Edit with your details
vim ~/.gitconfig
# Change user.name and user.email

# Test it
git config --list
```

### Starting Development Services

```bash
# Start Docker services for development
docker-compose -f startup-configs/docker-compose.dev.yml.example up -d

# Check running services
docker-compose -f startup-configs/docker-compose.dev.yml.example ps

# Stop services when done
docker-compose -f startup-configs/docker-compose.dev.yml.example down
```

### Using AI Prompts

```bash
# Browse available prompts
ls prompts/ai-prompts/

# View a prompt
cat prompts/ai-prompts/code-review-request.md

# Copy to clipboard (macOS)
cat prompts/ai-prompts/debug-assistance.md | pbcopy

# Copy to clipboard (Linux with xclip)
cat prompts/ai-prompts/debug-assistance.md | xclip -selection clipboard
```

### Creating Notes

```bash
# Create a new note based on template
cp notes/example-note.md notes/my-new-topic.md

# Edit your note
vim notes/my-new-topic.md
```

## 🔄 Keeping Settings Updated

### On Your Main Machine

1. Make changes to your configurations
2. Copy updated configs to this repository
3. Commit and push:
```bash
git add .
git commit -m "Update: VSCode settings with new extensions"
git push
```

### On Other Machines

1. Pull latest changes:
```bash
git pull
```

2. Copy updated configs to their locations:
```bash
cp cli-tools/git/.gitconfig ~/.gitconfig
# ... and so on
```

## 💡 Pro Tips

- **Backup First**: Always backup your existing configs before replacing them
- **Review Before Use**: Read example files before copying them
- **Customize**: These are templates - modify them for your needs
- **Stay Organized**: Keep your personal settings in this repository
- **Document Changes**: Add notes about why you made changes
- **Use Branches**: Create branches for experimental configs

## 🆘 Troubleshooting

### Config Not Working?

1. Check file permissions: `ls -la ~/.gitconfig`
2. Verify file location is correct
3. Check syntax in config files
4. Review error messages

### Script Won't Run?

1. Make it executable: `chmod +x script.sh`
2. Check for required dependencies
3. Read the script header for usage instructions

### Need Help?

1. Check the README in each directory
2. Review example files
3. Open an issue on GitHub
4. Check CONTRIBUTING.md for guidelines

## 📚 Next Steps

1. Explore each directory's README
2. Customize example files for your use
3. Add your own configs and scripts
4. Share useful additions via pull requests

Happy coding! 🎉
