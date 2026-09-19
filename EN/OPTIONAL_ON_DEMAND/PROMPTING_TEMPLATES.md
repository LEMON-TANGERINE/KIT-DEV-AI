# Prompting templates

## Universal
Context:
[project and affected area]

Goal:
[what I want to achieve]

Constraints:
[what must not change / limits]

Acceptance criteria:
[what must be true]

Process:
First analyze and propose a plan.
Do not implement until the approach is clear.

## Small task
Modify [X] so that [behavior].
Keep [constraint].
Do not change [area].
Then run [tests/command] and summarize exactly what changed.

## Bug
Problem: [bug]
Expected: [...]
Current: [...]
First identify the root cause.
Do not make superficial patches.
Then fix it and add a test that prevents regression.

## Refactor
Refactor [module].
Constraints:
- Do not change behavior.
- Do not change the public API.
- Do not add dependencies.
First propose the plan. Then implement small changes and run tests.

## Important feature
Read README.md, ROADMAP.md, AGENTS.md and this feature's spec.
Summarize relevant context, propose a plan and list the files you would touch.
Do not implement yet.

## Security review
Perform a security review of the current change.
Do not modify code.
Use SECURITY_REVIEW_TEMPLATE.md.

## Pre-merge review
Review this branch against main before merge.
Do not modify code.
Use PRE_MERGE_REVIEW_TEMPLATE.md.
