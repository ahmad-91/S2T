# Cursor Project Rules

This directory contains project-specific rules that Cursor AI will automatically follow when working in this codebase.

## How It Works

Cursor automatically reads all `.md` files in the `.cursor/rules/` directory and applies them as context for AI-generated code and suggestions.

## Rule Files

- **authoritative-sources.md** - Defines `/truth/TC.vX.md` as the authoritative source
- **requirements-handling.md** - Guidelines for handling ambiguous requirements
- **metadata-tags.md** - Rules for using `origin:` and `derived-from:` tags
- **custom-commands.md** - Documentation of available custom commands/macros
- **workflow-guidelines.md** - Overall workflow and process guidelines

## Adding New Rules

To add new rules:
1. Create a new `.md` file in this directory
2. Use clear, actionable language
3. Be specific about what should or shouldn't be done
4. Commit the file to version control

Cursor will automatically pick up new rule files without requiring any additional configuration.

## Verification

To verify Cursor is reading these rules:
1. Ask Cursor to generate code
2. Check if it references `/truth/TC.vX.md` when making decisions
3. Verify it logs ambiguities to `/requirements/SRS.ambiguities.md` when needed

