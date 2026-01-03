# Skill: Tasking

## Purpose
Maintain a clear, rolling task list in `.agent/TASKS.md` that matches the active plan.

## When to use
- Starting or finishing a task.
- The active plan changes.
- Work is blocked or needs clarification.

## Inputs required
- `AGENTS.md`
- `.agent/CONTEXT.md`
- `.agent/CONSTRAINTS.md`
- `.agent/PLANS.md`
- `.agent/TASKS.md`

## Procedure
1. Read the active plan and confirm the next task to do.
2. Add or update the Active section with a concise task and acceptance criteria.
3. Move completed work to Completed (append-only).
4. Note blockers or questions in Active if work cannot proceed.

## Quality gates
- Active tasks map directly to the plan's steps.
- Each task has a clear acceptance check.
- Completed entries are appended, not rewritten.

## Stop conditions
- No active plan exists for the work.
- Tasks extend beyond agreed scope.

## Output format
Updated `.agent/TASKS.md` with current Active and updated Completed sections.
