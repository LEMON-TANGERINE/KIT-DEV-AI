# Code Understanding Prompt

I am going to give you a piece of code that I do not fully understand.

I want you to help me understand it as a developer, not simply translate it line by line.

## IMPORTANT RULE

Do NOT start with a line-by-line explanation.

First help me understand the role of the code within the larger system.

## STEP 1 — BUILD THE MENTAL MODEL

Before explaining the implementation, answer:

1. What is the overall purpose of this code?
2. Where does this code belong in the application?
3. Who calls or uses it?
4. What inputs does it receive?
5. What outputs does it produce?
6. What side effects does it have?
7. What external dependencies or libraries does it use?
8. Which parts are normal Python concepts I probably already know?
9. Which parts introduce new concepts?
10. What 2–3 concepts do I need to understand before this code will make sense?

Keep this explanation at the architectural/functional level.

## STEP 2 — DIVIDE IT INTO LOGICAL BLOCKS

Break the code into meaningful sections.

For example:

```text
1. Configuration
2. Validation
3. Data retrieval
4. Business logic
5. Persistence
6. Response
```

Explain what each block is responsible for.

Do NOT explain every line yet.

## STEP 3 — EXPLAIN THE IMPORTANT PARTS

For each important block, explain:

* what problem it solves;
* why it exists;
* what it receives;
* what it produces;
* what it depends on;
* what depends on it.

Connect unfamiliar concepts to Python concepts I already know whenever possible.

## STEP 4 — STOP WHEN THERE IS A PREREQUISITE

If the code uses something I probably do not understand, such as:

* a framework;
* a library;
* dependency injection;
* decorators;
* middleware;
* async programming;
* ORM;
* repository pattern;
* context manager;
* dependency;
* API concept;
* architectural pattern;

STOP and explain that concept before continuing.

Do not assume I understand it just because I can read the syntax.

## STEP 5 — GO DEEPER ONLY WHERE NECESSARY

After the high-level explanation, let me identify what I still don't understand.

If I ask about a specific section, then explain it in more detail.

Only use line-by-line explanation when it is actually useful.

## MY LEVEL

I have been self-teaching Python for about a year.

I understand Python fundamentals such as:

* variables;
* functions;
* classes;
* exceptions;
* modules;
* loops;
* conditionals;
* basic object-oriented programming.

I can solve programming problems and build projects.

However, I struggle to understand unfamiliar professional code, especially when multiple libraries, abstractions, and components interact.

## GOAL

The goal is not for me to understand this single piece of code.

The goal is for me to become better at reading unfamiliar code independently.

Teach me the mental models and reasoning that will help me understand similar code in the future.
