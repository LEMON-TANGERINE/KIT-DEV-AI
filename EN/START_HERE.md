# Universal AI Development Framework

## What to copy ALWAYS when starting a project
- `.gitignore`
- `README.md`
- `ROADMAP.md`
- `AGENTS.md`

## What to use ONLY when needed

- `SPEC.md` → important, ambiguous feature, or one with multiple requirements/edge cases.
- `PLAN.md` → technical implementation of a spec or complex change.
- `TASKS.md` → split a large plan into small verifiable steps.
- `SECURITY_REVIEW.md` → sensitive changes or security review.
- `PRE_MERGE_REVIEW.md` → final review before merging into `main`.
- `PROMPTING_TEMPLATES.md` → reusable prompts.
- `DEVLOG_TEMPLATE.md` → use for projects where you want a persistent record of meaningful development work and decisions.

## Quick SPEC rule
NO spec for: typo, text change, rename, small obvious bug, trivial change.

USE a spec for: login, persistence, permissions, payments, sensitive data, multi-module changes,
features with edge cases, or behavior Codex could interpret in multiple ways.

SPEC = WHAT it must do.
PLAN = HOW it will be implemented.

## Flow
New project:
README → ROADMAP → AGENTS → first commit

Feature:
pick feature → SPEC if needed → PLAN if needed → implement → test → git diff
→ security/pre-merge review when relevant → commit → push → merge
