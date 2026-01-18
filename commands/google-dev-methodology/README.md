# Google Development Methodology Commands

Slash commands for the Google Development Methodology skill.

## Available Commands

### google-dev.md

Main command for invoking the Google Development Methodology skill.

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

# Database task
/google-dev 优化订单查询性能，解决 N+1 问题

# Testing task
/google-dev 为 OrderService 编写单元测试

# DevOps task
/google-dev 配置 GitHub Actions CI/CD 流水线

# Full-stack task
/google-dev 开发用户积分系统（后端 + 前端 + 数据库）
```

## Related

- [Google Development Methodology Skill](../../skills/google-dev-methodology/) - Main skill documentation
- [Commands Directory](../) - All available commands
