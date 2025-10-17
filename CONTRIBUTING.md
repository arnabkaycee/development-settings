# Contributing to Development Settings

Thank you for your interest in contributing! This is a personal repository, but contributions and suggestions are welcome.

## How to Contribute

### Reporting Issues

If you find any issues or have suggestions:
1. Open an issue on GitHub
2. Describe the problem or suggestion clearly
3. Include examples if applicable

### Suggesting Improvements

- Share useful configurations you use
- Suggest better organizational structures
- Recommend helpful scripts or tools
- Propose documentation improvements

### Submitting Changes

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Test your changes thoroughly
5. Commit with clear messages (`git commit -m 'Add: useful git alias'`)
6. Push to your fork (`git push origin feature/improvement`)
7. Open a Pull Request

## Guidelines

### File Naming
- Use lowercase with hyphens: `my-script.sh`
- Add `.example` suffix for template files
- Use descriptive names

### Documentation
- Add README.md files to new directories
- Include usage examples in scripts
- Document dependencies and prerequisites
- Keep documentation up-to-date

### Scripts
- Use bash for shell scripts
- Include shebang (`#!/bin/bash`)
- Add help text with `-h` or `--help` flag
- Use `set -e` for error handling
- Add comments explaining complex logic
- Make scripts executable (`chmod +x script.sh`)

### Configuration Files
- Use `.example` suffix for templates
- Remove sensitive information
- Document all configuration options
- Provide sensible defaults

### Commit Messages

Use conventional commit format:
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation changes
- `style:` - Formatting, missing semicolons, etc.
- `refactor:` - Code restructuring
- `chore:` - Maintenance tasks

Examples:
```
feat: add docker-compose for dev services
docs: update README with installation steps
chore: reorganize script directory
```

## Code of Conduct

- Be respectful and constructive
- Focus on improving the repository
- Help others learn and grow
- Share knowledge generously

## Questions?

Feel free to open an issue for any questions or discussions.

Thank you for contributing! 🎉
