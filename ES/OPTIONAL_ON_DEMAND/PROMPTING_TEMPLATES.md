# Prompting templates

## Universal
Contexto:
[proyecto y parte afectada]

Objetivo:
[qué quiero conseguir]

Restricciones:
[qué no debe cambiar / límites]

Criterios de aceptación:
[qué debe cumplirse]

Proceso:
Primero analiza y propón un plan.
No implementes hasta tener claro el enfoque.

## Tarea pequeña
Modifica [X] para que [comportamiento].
Mantén [restricción].
No cambies [parte].
Después ejecuta [tests/comando] y resume exactamente qué cambiaste.

## Bug
Problema: [bug]
Esperado: [...]
Actual: [...]
Primero identifica la causa raíz.
No hagas parches superficiales.
Después corrígelo y añade una prueba que evite regresiones.

## Refactor
Refactoriza [módulo].
Restricciones:
- No cambiar comportamiento.
- No cambiar API pública.
- No añadir dependencias.
Primero propón el plan. Después implementa cambios pequeños y ejecuta tests.

## Feature importante
Lee README.md, ROADMAP.md, AGENTS.md y la spec de esta feature.
Resume contexto relevante, propón un plan y lista archivos que tocarías.
No implementes todavía.

## Security review
Haz una revisión de seguridad del cambio actual.
No modifiques código.
Usa SECURITY_REVIEW_TEMPLATE.md.

## Pre-merge review
Revisa esta rama contra main antes del merge.
No modifiques código.
Usa PRE_MERGE_REVIEW_TEMPLATE.md.
