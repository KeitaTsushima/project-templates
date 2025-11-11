# Claude Code - [Project Name]

## Important Rules

1. **Check current status before working**
   - Check progress in `docs/daily-logs/` (most recent file)
   - Reference current PLAN in `docs/plans/` for implementation steps

2. **Never work directly on main branch**
   - Create feature branches for all work

3. **Always confirm before deletion**

4. **Record session log regularly**
   - Update `docs/daily-logs/YYYY-MM-DD.md` throughout the session
   - Good timing: after completing a feature, solving a problem, or making a key decision

## Code Implementation Procedure (MOST IMPORTANT)

**This workflow ensures effective collaboration, even for beginners.**

### Complete Development Workflow

#### Phase 1: Planning (Create PLAN.md)

Use `docs/plans/PLAN-template.md` as starting point. See `docs/plans/PLAN-guide.md` for detailed guidance.

#### Phase 2: Skeleton Implementation

**Step 1: Structure Only** (20-30 lines max)
- Empty functions/classes
- Type definitions
- Interface declarations
- NO implementation yet

**Step 2: Q&A Pause**
- Wait for questions and clarifications
- Explain architecture decisions
- Make adjustments based on feedback

**Step 3: Review & Confirm**
```bash
git add .
coderabbit review --prompt-only --type uncommitted
```
Fix any issues, then get confirmation to proceed.

#### Phase 3: Incremental Implementation

**For each function/component:**

1. **Implement ONE function** (20-30 lines max)
2. **Mandatory Q&A pause** - Explain what you wrote, answer questions
3. **Run CodeRabbit review** (same command as Phase 2)
4. **Fix issues** found by CodeRabbit
5. **Get confirmation** before next function

#### Phase 4: Integration & Testing

After all functions implemented:
- Integration testing
- Update PLAN.md with "Issues Encountered and Resolved"
- Document learnings for future reference
- Final CodeRabbit review before commit
- Commit with descriptive message

### Key Principles

- **Never rush**: Small iterations prevent misunderstandings
- **Document discoveries**: Real issues > theoretical assumptions
- **Always pause**: Frequent Q&A keeps understanding aligned
- **CodeRabbit as gatekeeper**: Review before every progression

### ❌ DON'T DO THIS
- Implementing multiple functions at once
- Skipping CodeRabbit reviews
- Moving forward without confirmation
- Writing implementation in planning phase

## Documentation Structure

This project follows a standardized documentation structure:

### Required Documentation

**docs/project-overview.md** - High-level project summary (start here)

**docs/plans/** - Create PLAN.md before major features (see `docs/plans/PLAN-template.md` and `PLAN-guide.md`)

**docs/daily-logs/** - Record every development session (see `docs/daily-logs/template.md` for format)

See `docs/README.md` for complete documentation structure.

## Code Quality Standards

- **No trailing whitespace**: Files must not contain trailing spaces or tabs on empty lines
- **Clean empty lines**: Empty lines should contain no characters (not even spaces)
- **Consistent indentation**: Use spaces consistently, no mixed tabs/spaces
