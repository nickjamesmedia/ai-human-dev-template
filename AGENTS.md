# Agent Contract

This repository is a reusable **AI/Human Hybrid Development Template**.  
All agents (Codex or non-Codex) must follow this contract when working here.

## Workflow (deliberate, repeatable)

1) **Read**  
   Open `AGENTS.md`, then `.agent/CONTEXT.md` and `.agent/CONSTRAINTS.md` before acting.

2) **Plan**  
   If the task is non-trivial, ambiguous, or could affect multiple files, write or update a plan in `.agent/PLANS.md`.  
   - Maintain **one active plan at a time**.
   - Clearly state assumptions and non-goals.

3) **Execute**  
   Make the **smallest safe change set** that advances the active plan.  
   Avoid speculative edits, rewrites, or pre-optimization.

4) **Verify**  
   Run, describe, or reason through **minimal validation checks** appropriate to the change.  
   Record results or limitations if full verification is not possible.

5) **Report**  
   Summarize what changed and update:
   - `.agent/TASKS.md` (status)
   - `.agent/DECISIONS.md` (if tradeoffs or irreversible choices were made)

## Guardrails (anti-drift, anti-overgeneration)

- Do not invent architecture, features, or files beyond the request and constraints.
- Avoid “vibe coding”: no speculative rewrites, mass refactors, or placeholder content.
- Prefer clarity over completeness; **pause and ask** when requirements are ambiguous.
- Keep outputs minimal and scoped; only touch files necessary for the task.

## Uncertainty & stop conditions

- If required information is missing, **stop and ask** rather than guessing.
- If the plan no longer fits the constraints, **revise the plan before executing**.
- When the plan’s acceptance criteria are met, **stop** and report—do not continue expanding scope.

## Directory-level overrides

- Instructions apply in this order:  
  nearest `AGENTS.md` → `.agent/CONSTRAINTS.md` → `.agent/CONTEXT.md` → root `AGENTS.md`.
- If a subdirectory contains its own `AGENTS.md`, follow it for work in that subtree.
- If no overrides exist, the root files are authoritative.

## Collaboration conventions

- Use `.agent/` files as the **shared source of truth** across humans and agents.
- Treat `.agent/` entries as append-only unless explicitly instructed otherwise.
- Keep “current” sections at the top of each file; older notes remain below.

## What not to do

- Do not generate application code unless explicitly requested.
- Do not assume a framework, language, or deployment target.
- Do not remove, rewrite, or reorganize unrelated content without approval.
