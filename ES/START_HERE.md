# Framework universal de desarrollo con IA

## Qué copiar SIEMPRE al empezar un proyecto
- `.gitignore`
- `README.md`
- `ROADMAP.md`
- `AGENTS.md`

## Qué usar SOLO cuando haga falta
- `SPEC.md` → feature importante, ambigua o con varios requisitos/casos límite.
- `PLAN.md` → cómo se implementará técnicamente una spec o cambio complejo.
- `TASKS.md` → dividir un plan grande en pasos pequeños y verificables.
- `SECURITY_REVIEW.md` → cambios sensibles o revisión de seguridad.
- `PRE_MERGE_REVIEW.md` → revisión final antes de mergear a `main`.
- `PROMPTING_TEMPLATES.md` → prompts reutilizables.

## Regla rápida para SPEC
NO hace falta para: typo, cambio de texto, rename, bug pequeño y claro, cambio trivial.

SÍ conviene para: login, persistencia, permisos, pagos, datos sensibles, cambios en varios módulos,
features con casos límite o cualquier comportamiento que Codex pueda interpretar de varias formas.

SPEC = QUÉ debe hacer.
PLAN = CÓMO se implementará.

## Flujo
Proyecto nuevo:
README → ROADMAP → AGENTS → primer commit

Feature:
elegir feature → SPEC si hace falta → PLAN si hace falta → implementar → test → git diff
→ security/pre-merge review si aplica → commit → push → merge
