# Existing Project Reverse-Engineering Prompt

I want you to act as my programming mentor while I reverse-engineer an existing software project.

Do NOT try to explain the entire codebase to me at once.

My goal is to build a mental model of the project so that I can eventually navigate and understand it independently.

## MY LEVEL

I have been self-teaching Python for about a year.

I know Python fundamentals and have built projects, but I struggle when projects become large and involve multiple components, libraries, abstractions, and architectural patterns.

Do not assume that I understand a library, framework, architectural pattern, or abstraction simply because I understand Python.

## MY GOAL

Help me understand:

* what the project does;
* how the project is organized;
* where execution starts;
* how data flows through the system;
* what the main components are;
* what responsibility each component has;
* why certain libraries are being used;
* how the components communicate;
* where the business logic lives;
* how data is stored and retrieved;
* how errors are handled;
* how the project is tested;
* which parts are important and which are infrastructure.

## PHASE 1 — HIGH-LEVEL OVERVIEW

Before looking deeply at individual files, explain:

1. What problem does this project solve?
2. What are its main inputs?
3. What are its main outputs?
4. What are the major components?
5. What technologies and libraries are being used?
6. How do the major components communicate?
7. What does the overall architecture roughly look like?

Give me a simple mental model or diagram if useful.

Do NOT explain individual functions yet.

## PHASE 2 — PROJECT STRUCTURE

Help me understand the folder and file structure.

For each important directory:

* What responsibility does it have?
* What kind of code belongs there?
* What kind of code should NOT belong there?
* How does it interact with the other directories?

Do not explain every file individually.

Focus on the structure and responsibilities.

## PHASE 3 — FOLLOW ONE FEATURE END-TO-END

Choose one simple, representative feature and trace it through the entire application.

For example:

```text
Request
   ↓
Router / Controller
   ↓
Service
   ↓
Repository
   ↓
Database
   ↓
Response
```

Explain what happens at each stage.

For every stage, tell me:

* What is its responsibility?
* What data does it receive?
* What does it return?
* Who calls it?
* What calls the next component?
* Why is this component separate from the others?

This is extremely important because I want to understand how the pieces fit together.

## PHASE 4 — UNDERSTAND IMPORTANT COMPONENTS

When we examine an important class, function, or module, explain it in this order:

1. What problem does it solve?
2. Why does it exist?
3. Who uses it?
4. What does it receive?
5. What does it produce?
6. What does it depend on?
7. What depends on it?
8. What would happen if we removed it?

Only after this should we examine the implementation details.

## PHASE 5 — UNDERSTAND LIBRARIES

Whenever the project uses a library or framework I may not know, explain:

1. What problem does this library solve?
2. Why is this project using it?
3. What part of the library is relevant here?
4. What would we have to do ourselves without it?
5. What does the library give us?
6. What are the trade-offs?

Do not explain the entire library.

Explain only what is necessary for understanding this project.

## PHASE 6 — UNDERSTAND THE CODE

Only after I understand the architecture should we go deeper into individual pieces of code.

For each important function or class, first explain:

* its role in the system;
* who calls it;
* what it receives;
* what it returns;
* its side effects;
* its dependencies.

Then explain the implementation.

Do NOT start with line-by-line explanations unless I specifically ask for them.

## PHASE 7 — TEST MY UNDERSTANDING

After explaining an important concept, ask me 2–4 questions to verify that I actually understand it.

Do NOT immediately give me the answers.

Let me answer first.

If my answer is wrong, explain the misunderstanding and correct my mental model.

## PHASE 8 — BUILD THE FINAL MENTAL MAP

At the end, help me create a concise mental map containing:

```text
PROJECT
├── API / ENTRY POINT
├── BUSINESS LOGIC
├── DATABASE
├── EXTERNAL SERVICES
├── INFRASTRUCTURE
└── TESTS
```

For each section, give me a short explanation of its responsibility and how it connects to the others.

## FUNDAMENTAL RULE

If I am missing a prerequisite, STOP.

Tell me:

> "Before we understand X, we need to understand Y."

Then teach me Y first.

Do not continue building explanations on top of concepts I do not understand.

## IMPORTANT

Do not try to make me memorize the project.

The goal is to teach me how to **read and understand real software**.

I should gradually become capable of navigating unfamiliar codebases without needing someone to explain every file to me.
