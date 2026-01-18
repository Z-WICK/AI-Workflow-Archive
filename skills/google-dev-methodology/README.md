# Google Development Methodology

A comprehensive skill for acting as a Google full-stack engineer who adapts roles based on task type while maintaining Google's core development principles.

## Overview

This skill enables you to work like a Google engineer across all layers of the stack:
- **Backend Engineer** - Java/Spring Boot, API development, microservices
- **Frontend Engineer** - Vue/React, UI components, state management
- **Database Engineer** - SQL optimization, schema design, performance tuning
- **QA Engineer** - Testing strategy, automation, quality assurance
- **DevOps Engineer** - CI/CD, deployment, infrastructure automation
- **Full-Stack Engineer** - Coordinating across all layers

## Core Principles (Non-Negotiable)

1. **Documentation First** - Create detailed docs before coding
2. **Small Steps** - Frequent commits, one feature per commit
3. **Always Green** - Every commit must compile and pass tests
4. **Test First** - Write tests before implementation (TDD)
5. **Never Compromise** - Complete implementation, no shortcuts
6. **Code Review Standards** - Follow style guides, clear naming, proper error handling

## Installation

### Install the Skill

```bash
# Copy skill to Factory skills directory
cp -r google-dev-methodology ~/.factory/skills/
```

### Install the Slash Command (Optional)

For easier invocation, install the slash command:

```bash
# Copy slash command to Factory commands directory
cp ../../commands/google-dev-methodology/google-dev.md ~/.factory/commands/
```

The slash command (`google-dev.md`) provides:
- Quick invocation: `/google-dev [task]`
- Automatic skill binding
- Chinese language support
- Comprehensive usage examples for all 6 roles

## Usage

### Method 1: Using Slash Command (Recommended)

```bash
/google-dev [task description]
```

### Method 2: Direct Skill Invocation

```
Use the skill: google-dev-methodology
[task description]
```

### Examples

**Backend Tasks:**
```bash
/google-dev Refactor MartialScheduleService, split into multiple services
/google-dev Implement user authentication API with JWT
/google-dev Optimize order query performance, fix N+1 problem
```

**Frontend Tasks:**
```bash
/google-dev Build user dashboard component with responsive layout
/google-dev Implement shopping cart with state management
/google-dev Optimize bundle size, reduce first load time
```

**Database Tasks:**
```bash
/google-dev Design user points system database schema
/google-dev Optimize slow query, order list takes 5 seconds
/google-dev Add composite index for user table
```

**Testing Tasks:**
```bash
/google-dev Write unit tests for OrderService
/google-dev Add integration tests for payment flow
/google-dev Improve test coverage to 80%+
```

**DevOps Tasks:**
```bash
/google-dev Set up GitHub Actions CI/CD pipeline
/google-dev Deploy backend service with Docker
/google-dev Configure Nginx reverse proxy
```

**Full-Stack Tasks:**
```bash
/google-dev Build user points system (backend + frontend + database)
/google-dev Implement complete order management module
/google-dev Build user authentication system with login page
```

## How It Works

1. **Task Analysis** - Analyzes your task and selects appropriate engineer role
2. **Documentation** - Creates detailed implementation document
3. **User Approval** - Waits for your approval before coding
4. **Test First** - Writes tests before implementation (TDD)
5. **Small Steps** - Implements in small, frequent commits
6. **Verification** - Compiles and tests before each commit
7. **Code Review** - Self-reviews before completion
8. **Deployment** - Deploys and monitors
9. **Documentation** - Documents lessons learned

## Subagent Strategy

The skill intelligently uses subagents for parallel execution:

| Scenario | Strategy | Expected Speedup |
|----------|----------|------------------|
| Creating independent files | Parallel subagents | 2-4x |
| Modifying same file | Single agent sequential | None |
| Independent test writing | Parallel subagents | 2-3x |
| Multi-module projects | Parallel subagents | 3-5x |
| Strong dependencies | Serial subagents | 1.5-2x |

## Decision Matrix

Use this matrix to understand when to use this methodology:

| Task Type | Complexity | Urgent? | Use This Skill? |
|-----------|-----------|---------|-----------------|
| Simple bug | Low | Yes | ❌ No - direct fix |
| Complex bug | High | No | ✅ Yes |
| Small feature | Low | - | ❌ No - direct implementation |
| Medium feature | Medium | No | ✅ Yes |
| Large feature | High | No | ✅ Yes |
| God Class refactoring | High | No | ✅ Yes |
| Database optimization | Medium | No | ✅ Yes |
| Test suite creation | Medium | No | ✅ Yes |
| CI/CD setup | Medium | No | ✅ Yes |
| Urgent hotfix | Low | Yes | ❌ No - direct fix |

## Quality Standards

All work must meet these standards:
- ✅ All tests passing (100%)
- ✅ Code coverage ≥ 80%
- ✅ Code review passed
- ✅ Documentation updated
- ✅ Deployed successfully
- ✅ Monitoring in place

## Real-World Results

### Backend - God Class Refactoring
- **Before**: 996 lines
- **After**: 290 lines (70.9% reduction)
- **Commits**: 48
- **Tests**: 482 (100% passing)
- **Time**: 2 days

### Frontend - User Dashboard
- **Result**: 5 reusable components, 12 tests
- **Bundle**: Optimized
- **Time**: 1 day

### Database - Query Optimization
- **Before**: 850ms
- **After**: 45ms (95% improvement)
- **Time**: 4 hours

### Full-Stack - User Points System
- **Components**: Backend + Frontend + Database
- **Coverage**: 80%+
- **Time**: 5 hours (vs 11 hours single agent, 55% speedup)

## Files in This Skill

```
google-dev-methodology/
├── SKILL.md                          # Main skill definition
├── README.md                         # This file
├── prompts/                          # Subagent prompt templates
│   ├── backend-engineer-prompt.md
│   ├── frontend-engineer-prompt.md
│   ├── database-engineer-prompt.md
│   ├── qa-engineer-prompt.md
│   └── devops-engineer-prompt.md
└── case-studies/                     # Continuous learning
    ├── README.md                     # Case study guidelines
    ├── template.md                   # Case study template
    └── index.md                      # Statistics and index
```

## Continuous Learning & Evolution

This skill **learns and evolves** from every completed task!

After successfully completing a task, you'll be prompted:

```
✅ Task completed successfully!

📊 Would you like to save this as a case study for continuous learning?
   [Y/n]
```

**Benefits:**
- **For You:** Search similar cases, learn from experiences, get accurate estimates
- **For Skill:** Refine Decision Matrix, optimize strategies, improve documentation
- **For Community:** Share knowledge, build collective intelligence, improve success rates

**What's Saved:**
- Task description and approach
- Execution details and metrics
- Lessons learned and recommendations
- Impact on skill improvement

See `case-studies/README.md` for details.

## Related

- **Slash Command**: `~/.factory/commands/google-dev.md`
- **Skill Store**: This is a custom skill, not from Skillstore

## Philosophy

> "The only way to go fast is to go well." - Robert C. Martin

This skill embodies Google's engineering culture:
- **Your identity is flexible** - Adapt role based on task
- **Your standards are not** - Always follow core principles
- **Quality over speed** - But quality enables speed
- **No compromises** - Complete implementation, zero technical debt

---

*"Sir, as a Google engineer, I adapt my role but never my standards." - J.A.R.V.I.S.*
