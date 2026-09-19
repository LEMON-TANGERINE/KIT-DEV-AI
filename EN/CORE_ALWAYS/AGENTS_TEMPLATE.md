# AGENTS.md

## Project
**Name:** [NAME]

**Goal:**  
[What product is being built and what it must achieve.]

## Sources of truth
- `README.md` → what the project is.
- `ROADMAP.md` → scope and feature order.
- `specs/` → requirements for important features, when they exist.

## Stack
- Language:
- Framework:
- Persistence:
- Tests:
- Platform:

## Rules
- Keep the solution as simple as possible.
- Do not add dependencies without explaining and justifying them.
- Do not change the stack or architecture without proposing it first.
- Do not implement functionality outside the requested scope.
- Follow existing patterns.
- Avoid duplicated logic.
- Keep changes small and reviewable.

## Security
- Never add secrets, API keys, tokens, passwords or credentials to the repo.
- Never commit real `.env` files.
- Treat external input as untrusted.
- Do not run destructive commands without explicit approval.
- Do not use `force push` without explicit approval.
- Do not disable security controls just to “make it work”.
- For sensitive changes, perform a security review before finishing.

## Agent workflow

### Small change
1. Implement.
2. Verify.
3. Summarize changes.

### Medium change
1. Analyze.
2. Propose a short plan.
3. Implement after confirming the approach.
4. Verify.

### Important feature / delicate refactor
1. Read the spec if one exists.
2. Analyze the current state.
3. Propose a plan.
4. Split into small tasks if needed.
5. Implement step by step.
6. Run tests.
7. Review `git diff`.
8. Perform a security review when relevant.

## Definition of Done
A task is done when:
- requirements are met;
- relevant checks pass;
- there are no known regressions;
- there are no out-of-scope changes;
- there are no secrets or sensitive files;
- the diff is clear and reviewable.
