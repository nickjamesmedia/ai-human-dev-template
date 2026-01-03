# Skill: Planning

## Purpose
Create or update a deliberate plan in `.agent/PLANS.md` for non-trivial work.

## When to use
- New work is non-trivial or touches multiple files.
- The current plan is missing, stale, or unclear.
- Requirements or constraints are ambiguous.

## Inputs required
- `AGENTS.md`
- `.agent/CONTEXT.md`
- `.agent/CONSTRAINTS.md`
- `.agent/PLANS.md`
- `.agent/TASKS.md` (if present)

## Procedure
1. Read context and constraints; restate the goal in your own words.
2. Draft or update the active plan with goal, non-goals, approach, steps, and validation.
3. Keep one active plan; archive older plans if needed.
4. Stop and ask if required information is missing.

## Quality gates
- Plan aligns with constraints and avoids scope creep.
- Steps are minimal and ordered for small, safe changes.
- Validation criteria are concrete and checkable.

## Stop conditions
- Requirements are ambiguous or conflicting.
- The plan's acceptance criteria are met.

## Output format
Updated `.agent/PLANS.md` with a single active plan.
