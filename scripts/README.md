# Utility Scripts

A collection of useful scripts for development, productivity, and system maintenance.

## 📂 Structure

- **setup/** - Installation and configuration scripts
- **productivity/** - Workflow automation scripts
- **maintenance/** - System cleanup and maintenance scripts

## 🚀 Setup Scripts

Scripts for setting up new development environments:
- Environment installation
- Dependency management
- Configuration deployment
- Tool installation

### Example Usage

```bash
# Run full setup
./setup/install-all.sh

# Install specific tool
./setup/install-node.sh
```

## ⚡ Productivity Scripts

Scripts to enhance development workflow:
- Git workflow helpers
- Project scaffolding
- Quick navigation
- Common task automation

### Example Usage

```bash
# Create new project from template
./productivity/new-project.sh my-app

# Quick git workflow
./productivity/quick-commit.sh "feat: add new feature"
```

## 🧹 Maintenance Scripts

System and environment maintenance:
- Cleanup old files
- Update dependencies
- Backup configurations
- System health checks

### Example Usage

```bash
# Clean up old logs
./maintenance/cleanup-logs.sh

# Update all tools
./maintenance/update-all.sh
```

## 📝 Script Guidelines

When adding new scripts:

1. **Use clear naming**: Descriptive names that explain what the script does
2. **Add help text**: Include usage instructions with `-h` or `--help`
3. **Make executable**: `chmod +x script-name.sh`
4. **Add error handling**: Check for errors and provide meaningful messages
5. **Document dependencies**: Note required tools in comments
6. **Test thoroughly**: Verify on a clean environment

## 🔒 Safety

- Always review scripts before running
- Test on non-production environments first
- Backup before running destructive operations
- Use dry-run modes when available

## 📖 Template Script

```bash
#!/bin/bash
# Script Name: example.sh
# Description: What this script does
# Dependencies: bash, git, curl
# Usage: ./example.sh [options]

set -e  # Exit on error

# Help text
if [[ "$1" == "-h" ]] || [[ "$1" == "--help" ]]; then
    echo "Usage: $0 [options]"
    echo "Description of what this script does"
    exit 0
fi

# Script logic here
echo "Running example script..."
```
