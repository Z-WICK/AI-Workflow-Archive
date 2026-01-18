# Slash Commands

This directory contains slash commands for quick invocation of skills.

## Available Commands

### google-dev.md

Slash command for the Google Development Methodology skill.

**Installation:**
```bash
cp google-dev.md ~/.factory/commands/
```

**Usage:**
```bash
/google-dev [task description]
```

**Features:**
- Automatic skill binding to `google-dev-methodology`
- Chinese language support
- Comprehensive usage examples
- All 6 role examples (Backend, Frontend, Database, QA, DevOps, Full-Stack)

**Examples:**
```bash
# Backend task
/google-dev 重构 OrderService，拆分成多个服务

# Frontend task
/google-dev 构建用户仪表盘组件，支持响应式布局

# Full-stack task
/google-dev 开发用户积分系统（后端 + 前端 + 数据库）
```

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

## Related

- [Skills Directory](../skills/) - Available skills
- [Google Development Methodology](../skills/google-dev-methodology/) - Main skill documentation
