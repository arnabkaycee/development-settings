# VSCode Extensions

This file lists recommended VSCode extensions for development.

## How to Use

Install all extensions at once:
```bash
cat extensions.txt | xargs -L 1 code --install-extension
```

Or install individually:
```bash
code --install-extension <extension-id>
```

## Export Your Extensions

```bash
code --list-extensions > extensions.txt
```

## Recommended Extensions

### General Development
- esbenp.prettier-vscode
- dbaeumer.vscode-eslint
- eamodio.gitlens
- streetsidesoftware.code-spell-checker

### Languages
- ms-python.python
- golang.go
- ms-vscode.cpptools
- rust-lang.rust-analyzer

### Tools
- ms-azuretools.vscode-docker
- ms-kubernetes-tools.vscode-kubernetes-tools
- redhat.vscode-yaml
- yzhang.markdown-all-in-one

### Productivity
- formulahendry.auto-rename-tag
- christian-kohler.path-intellisense
- wayou.vscode-todo-highlight
- oderwat.indent-rainbow
