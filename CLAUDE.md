# ARIA — Asistente / agente de IA

**Estado:** estructura inicial. El propósito y el alcance de ARIA aún no
están definidos (ver `docs/vision.md`).

## Reglas de trabajo

- **Cero alucinaciones.** Las respuestas se basan solo en el contenido de
  `knowledge/` y `docs/`. Si falta un dato, se escribe literalmente "Dato no
  disponible en la documentación". No se completa por inferencia.
- **Rama principal:** `main`.
- **Prompts:** se versionan en `prompts/`. Un cambio de prompt va en su propio
  commit con la justificación.
- **Evaluaciones:** todo cambio de prompt o skill se valida contra
  `evaluaciones/` antes de comitear.

## Estructura

Ver la tabla de carpetas en `README.md`.
