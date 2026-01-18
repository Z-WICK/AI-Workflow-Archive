# Slash Commands

This directory contains slash commands for quick invocation of skills, organized by category.

## Directory Structure

```
commands/
├── README.md                           # This file
├── google-dev-methodology/             # Commands for Google Dev Methodology
│   └── google-dev.md
└── [other-skill-name]/                 # Commands for other skills
    └── command.md
```

## Available Commands

### google-dev-methodology/

Commands for the Google Development Methodology skill.

**Installation:**
```bash
cp google-dev-methodology/google-dev.md ~/.factory/commands/
```

**Available commands:**
- `google-dev.md` - Main command for invoking the skill

See [google-dev-methodology/](./google-dev-methodology/) for details.

## What is a Slash Command?

Slash commands are shortcuts that make it easier to invoke skills in Factory/Droid:

- **Quick invocation** - Type `/command` instead of "Use the skill: skill-name"
- **Argument passing** - Pass task descriptions directly: `/command [task]`
- **Binding** - Automatically loads the associated skill
- **Documentation** - Includes usage examples and descriptions

## Creating Your Own Slash Commands

Slash commands are markdown files with YAML frontmatter:

```markdown
---
name: command-name
description: Command description
argument-hint: <argument description>
binding: skill:skill-name
---

# Command Title

**任务**: $ARGUMENTS

Command content and examples...
```

**Key fields:**
- `name` - Command name (used as `/name`)
- `description` - Brief description
- `argument-hint` - Hint for arguments
- `binding` - Skill to invoke (format: `skill:skill-name`)
- `$ARGUMENTS` - Placeholder for user-provided arguments

## Adding New Commands

To add commands for a new skill:

1. Create a subdirectory: `commands/your-skill-name/`
2. Add your command files: `your-skill-name/command.md`
3. Update this README with installation instructions
4. Commit and push

## Related

- [Skills Directory](../skills/) - Available skills
- [Google Development Methodology](../skills/google-dev-methodology/) - Main skill documentation
