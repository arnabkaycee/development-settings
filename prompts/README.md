# Development Prompts

A collection of prompts and templates for development workflows.

## 📂 Structure

- **ai-prompts/** - Prompts for AI coding assistants (GitHub Copilot, ChatGPT, etc.)
- **code-templates/** - Reusable code snippets and boilerplate

## 🤖 AI Prompts

The `ai-prompts/` directory contains pre-written prompts for:
- Code review requests
- Documentation generation
- Test case creation
- Refactoring guidance
- Debugging assistance
- Architecture planning

### Usage Example

```bash
# Copy a prompt template
cat ai-prompts/code-review-prompt.md | pbcopy

# Or use with a script
./scripts/productivity/use-prompt.sh code-review
```

## 📝 Code Templates

The `code-templates/` directory includes:
- Project scaffolding templates
- Common code patterns
- Configuration file templates
- Documentation templates
- CI/CD pipeline templates

### Template Format

Templates should use placeholders for easy find-and-replace:
- `{{PROJECT_NAME}}` - Project name
- `{{AUTHOR}}` - Author name
- `{{DATE}}` - Current date
- `{{DESCRIPTION}}` - Project description

## 🔧 Adding New Prompts

1. Create a new `.md` file in the appropriate directory
2. Use clear, descriptive filenames (e.g., `debug-performance-issue.md`)
3. Include context about when to use the prompt
4. Add examples if applicable

## 💡 Tips

- Keep prompts focused on specific tasks
- Include necessary context in the prompt
- Update prompts based on what works well
- Share successful prompts with the team
