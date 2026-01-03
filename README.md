# ai-human-dev-template

A lightweight, reusable template for **AI/Human hybrid development** that emphasizes intentional planning, clear context, and maintainable outcomes - not vibe coding.

This repo provides a simple operating system for working with AI agents (Codex or otherwise) while keeping humans firmly in control of goals, constraints, and decisions.

## Core idea

AI should **assist thinking**, not replace it.

This template externalizes project thinking into a small set of shared Markdown files so that:
- humans stay oriented and intentional
- agents receive clear, durable context
- work remains reviewable, auditable, and maintainable over time

## How collaboration works

Humans and agents coordinate through the `.agent/` directory:

- `CONTEXT.md`
  What this project is, who it's for, and why it exists.

- `CONSTRAINTS.md`
  Hard rules, non-goals, and boundaries that must not be violated.

- `TASKS.md`
  A rolling list of current, next, and recently completed work.

- `PLANS.md`
  One active plan at a time: approach, tradeoffs, and validation steps.

- `DECISIONS.md`
  Append-only record of meaningful decisions and rationale.

- `REVIEW_CHECKLIST.md`
  A safety net to prevent scope creep and accidental breakage.

These files are intentionally:
- minimal
- human-readable
- append-friendly
- easy for AI agents to load and respect

## Skills

The `skills/` directory provides short, tool-agnostic checklists for common workflows such as planning, tasking, and reviewing.

## Typical workflow

1. Update **context and constraints**
2. Define or refine the **active plan**
3. Execute work on a branch
4. Validate changes (tests, lint, smoke checks, or manual verification)
5. Record decisions and mark tasks complete
6. Merge intentionally

## Forks are encouraged

This repository is meant to be **forked and adapted** to your domain, team size, and tooling.

You are free to:
- modify the structure
- add skills or automation
- use it with any AI system or none at all

The goal is not rigid process - it's **clear thinking made visible**.
