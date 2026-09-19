# AGENTS.md

## Proyecto
**Nombre:** [NOMBRE]

**Objetivo:**  
[Qué producto se construye y qué debe conseguir.]

## Fuentes de verdad
- `README.md` → qué es el proyecto.
- `ROADMAP.md` → alcance y orden de features.
- `specs/` → requisitos de features importantes, si existen.

## Stack
- Lenguaje:
- Framework:
- Persistencia:
- Tests:
- Plataforma:

## Reglas
- Mantén la solución lo más simple posible.
- No añadas dependencias sin avisar y justificarlo.
- No cambies stack o arquitectura sin proponerlo primero.
- No implementes funcionalidades fuera de alcance.
- Sigue los patrones existentes.
- Evita duplicar lógica.
- Haz cambios pequeños y revisables.

## Seguridad
- Nunca añadas secretos, API keys, tokens, contraseñas o credenciales al repo.
- Nunca incluyas `.env` reales en commits.
- Trata inputs externos como no confiables.
- No ejecutes comandos destructivos sin aprobación explícita.
- No uses `force push` sin aprobación explícita.
- No desactives controles de seguridad solo para “hacer que funcione”.
- Para cambios sensibles, realiza una revisión de seguridad antes de terminar.

## Workflow del agente

### Cambio pequeño
1. Implementa.
2. Verifica.
3. Resume cambios.

### Cambio mediano
1. Analiza.
2. Propón un plan corto.
3. Implementa tras confirmar enfoque.
4. Verifica.

### Feature importante / refactor delicado
1. Lee la spec si existe.
2. Analiza el estado actual.
3. Propón un plan.
4. Divide en tareas pequeñas si hace falta.
5. Implementa por pasos.
6. Ejecuta tests.
7. Revisa `git diff`.
8. Haz security review si aplica.

## Definition of Done
Una tarea termina cuando:
- cumple requisitos;
- las verificaciones relevantes pasan;
- no hay regresiones conocidas;
- no hay cambios fuera de alcance;
- no hay secretos ni archivos sensibles;
- el diff es claro y revisable.

## Registro de desarrollo

Si existe `DEVLOG.md`:

- Mantén `DEVLOG.md` actualizado después de completar tareas relevantes.
- Añade una entrada breve por cada tarea completada, no por cada edición individual.
- Registra:
  - qué cambió;
  - archivos principales afectados;
  - verificación realizada;
  - decisiones técnicas relevantes o limitaciones.
- No registres cambios triviales de formato, correcciones tipográficas o ediciones insignificantes.
- Mantén las entradas breves, claras y objetivas.