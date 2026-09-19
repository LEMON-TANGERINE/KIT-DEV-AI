# AGENTS.md

## Project overview

**Project:** [NAME]

**Objective:**  
[What product is being built and what outcome it should deliver.]

**Product source of truth:**  
- `README.md` → project vision and usage.
- `ROADMAP.md` → scope and feature order.
- `specs/` → detailed requirements for important features, if they exist.

## Stack and constraints

- Language: [Python / ...]
- Framework: [if applicable]
- Persistence: [if applicable]
- Tests: [pytest / ...]
- Target platforms: [Windows / web / ...]

### Constraints
- Keep the solution as simple as possible.
- Do not add dependencies without warning and justification.
- Do not change the stack or architecture without proposing it first.
- Do not implement functionality outside the requested scope.

## Main commands

```bash
# Run
[command]

# Tests
[command]

# Lint / type check (if it exists)
[command]
```

If a command does not exist yet, do not invent it: say so.

## Project structure

```text
[current or expected structure]
```

Respect existing patterns. Do not create folders or abstractions just to “make it more professional”.

## Conventions

- Naming: [snake_case / PascalCase / ...]
- Functions and modules should have a clear responsibility.
- Avoid duplicating logic.
- Handle errors where there is enough context to do so properly.
- Add comments only when they provide information the code does not express clearly.

## Agent workflow

### Small change
1. Implement.
2. Run the relevant verification.
3. Summarize the changes.

### Medium change
1. Analyze the affected code.
2. Propose a short plan.
3. Implement after confirming the approach.
4. Verify.

### Important feature / delicate refactor
1. Read the corresponding spec if it exists.
2. Analyze the current state.
3. Propose a plan.
4. Break the work into small tasks.
5. Implement one task at a time.
6. Run tests after relevant changes.
7. Review the diff before finishing.

## Security

- Never add secrets, tokens, passwords, or credentials to the repository.
- Never include real `.env` files in commits.
- Do not run destructive operations without warning.
- Use the minimum privileges necessary.

## Before finishing a task

Check:
- [ ] The requested behavior works.
- [ ] The scope has not expanded.
- [ ] Relevant tests pass.
- [ ] No unnecessary dependencies were added.
- [ ] There are no secrets or sensitive files.
- [ ] The change is understandable and consistent with the project.

## Definition of Done

A task is finished when:
- it meets the agreed requirements;
- the relevant verification passes;
- it introduces no known regressions;
- it includes no out-of-scope changes;
- the result can be clearly reviewed with `git diff`.
