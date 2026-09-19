# AGENTS.md

## Project overview

**Proyecto:** [NOMBRE]

**Objetivo:**  
[Qué producto se está construyendo y qué resultado debe entregar.]

**Fuente de verdad del producto:**  
- `README.md` → visión y uso del proyecto.
- `ROADMAP.md` → alcance y orden de features.
- `specs/` → requisitos detallados de features importantes, si existen.

## Stack y restricciones

- Lenguaje: [Python / ...]
- Framework: [si aplica]
- Persistencia: [si aplica]
- Tests: [pytest / ...]
- Plataformas objetivo: [Windows / web / ...]

### Restricciones
- Mantén la solución lo más simple posible.
- No añadas dependencias sin avisar y justificarlo.
- No cambies el stack o la arquitectura sin proponerlo primero.
- No implementes funcionalidades fuera del alcance solicitado.

## Comandos principales

```bash
# Ejecutar
[comando]

# Tests
[comando]

# Lint / type check (si existe)
[comando]
```

Si un comando todavía no existe, no lo inventes: indícalo.

## Estructura del proyecto

```text
[estructura actual o esperada]
```

Respeta los patrones existentes. No crees carpetas o abstracciones solo para “hacerlo más profesional”.

## Convenciones

- Nombres: [snake_case / PascalCase / ...]
- Funciones y módulos con una responsabilidad clara.
- Evita duplicar lógica.
- Maneja errores donde tengan contexto suficiente.
- Comentarios solo cuando aporten información que el código no expresa bien.

## Workflow del agente

### Cambio pequeño
1. Implementa.
2. Ejecuta la verificación relevante.
3. Resume los cambios.

### Cambio mediano
1. Analiza el código afectado.
2. Propón un plan corto.
3. Implementa tras confirmar el enfoque.
4. Verifica.

### Feature importante / refactor delicado
1. Lee la spec correspondiente si existe.
2. Analiza el estado actual.
3. Propón un plan.
4. Divide el trabajo en tareas pequeñas.
5. Implementa una tarea cada vez.
6. Ejecuta tests después de cambios relevantes.
7. Revisa el diff antes de terminar.

## Seguridad

- Nunca añadas secretos, tokens, contraseñas o credenciales al repositorio.
- Nunca incluyas `.env` reales en commits.
- No ejecutes operaciones destructivas sin avisar.
- Usa el mínimo privilegio necesario.

## Antes de terminar una tarea

Comprueba:
- [ ] El comportamiento pedido funciona.
- [ ] No se ha ampliado el alcance.
- [ ] Los tests relevantes pasan.
- [ ] No se han añadido dependencias innecesarias.
- [ ] No hay secretos ni archivos sensibles.
- [ ] El cambio es entendible y coherente con el proyecto.

## Definition of Done

Una tarea está terminada cuando:
- cumple los requisitos acordados;
- la verificación relevante pasa;
- no introduce regresiones conocidas;
- no incluye cambios fuera de alcance;
- el resultado puede ser revisado claramente con `git diff`.
