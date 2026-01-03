# Skill: Reviewing

## Purpose
Perform a structured review using `.agent/REVIEW_CHECKLIST.md` before changes are accepted.

## When to use
- A change set is ready for review.
- You need to confirm scope and constraints were respected.
- You are preparing a final report or handoff.

## Inputs required
- `AGENTS.md`
- `.agent/CONTEXT.md`
- `.agent/CONSTRAINTS.md`
- `.agent/REVIEW_CHECKLIST.md`
- The list of changed files

## Procedure
1. Read context and constraints to set review scope.
2. Walk the review checklist and check each item against the changes.
3. Record findings with specific file paths and brief evidence.
4. State remaining risks or gaps if full verification was not possible.

## Quality gates
- Checklist items are all addressed.
- Findings are specific, reproducible, and scoped.
- No speculative or unrelated issues are raised.

## Stop conditions
- The change set is incomplete or cannot be accessed.
- Required checklist inputs are missing.

## Output format
A review note with findings, risks, and a clear pass or request for fixes.
