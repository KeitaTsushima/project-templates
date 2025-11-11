# Project Template for Claude Code

This is a standardized project template optimized for development with Claude Code and CodeRabbit.

## How to Use This Template

### Starting a New Project

1. Copy this template to your new project directory:
   ```bash
   cp -r ~/dev/project-templates/* ~/dev/your-new-project/
   cd ~/dev/your-new-project
   ```

2. Initialize git repository:
   ```bash
   git init
   git branch -m main
   git commit --allow-empty -m "Project start"
   ```

3. Customize project-specific files:
   - Update `CLAUDE.md` (project name, specific rules)
   - Update `docs/project-overview.md` (purpose, tech stack)
   - Remove this README.md and create project-specific one

4. Set up GitHub repository (if using GitHub):
   ```bash
   gh repo create your-repo-name --public --source=. --remote=origin
   git push -u origin main
   ```

5. Install CodeRabbit GitHub App (if using GitHub):
   - Visit https://github.com/apps/coderabbitai
   - Install for your repository

## What's Included

### Core Files
- `CLAUDE.md` - Claude Code project context and workflow
- `.coderabbit.yaml` - CodeRabbit configuration
- `.gitignore` - Standard ignore patterns

### Documentation Structure
- `docs/README.md` - Documentation index
- `docs/project-overview.md` - Project summary template
- `docs/daily-logs/template.md` - Daily log format
- `docs/plans/PLAN-template.md` - Planning document template

### Claude Code Guides
- `.claude/coderabbit-workflow.md` - CodeRabbit workflow guide

## Development Workflow

1. **Start of each feature**: Create PLAN.md in `docs/plans/`
2. **During development** (repeat for each function):
   - Implement 20-30 lines
   - Q&A with developer (questions, explanations, adjustments)
   - Run CodeRabbit CLI review
   - Fix issues found by CodeRabbit
   - Get confirmation before moving to next chunk
3. **Before commit**: Final CodeRabbit CLI review
4. **End of each session**: Update daily log in `docs/daily-logs/`

## Key Principles

- Incremental development (20-30 lines at a time)
- Frequent CodeRabbit reviews
- Mandatory Q&A pauses
- Comprehensive daily logs

## Requirements

- Git installed
- CodeRabbit CLI installed (`curl -fsSL https://cli.coderabbit.ai/install.sh | sh`)
- Claude Code access
- GitHub account (optional, for PR reviews)

## Support

See individual documentation files for detailed guides:
- Development workflow: `CLAUDE.md`
- CodeRabbit usage: `.claude/coderabbit-workflow.md`
- Documentation structure: `docs/README.md`
