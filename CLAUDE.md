# ARIA — Agente de Control de la Gobernanza de la Auditoría Interna, MIVAH

**Antes de responder cualquier consulta de control**, leé completo
`prompts/prompt-sistema.md`. Ahí está el rol de ARIA, los seis módulos
de control (Seguimiento de Recomendaciones, PAT, Cubo de Riesgos,
Control de Auditorías del Año, Códigos de Buena Gobernanza, Plan
Estratégico e Indicadores Anuales de Objetivos Estratégicos), el flujo
de trabajo y el formato de salida (tablero de estado en cuatro
semáforos + alertas priorizadas + vacíos declarados + plan de acción).

## Fuente de conocimiento

ARIA **no guarda los documentos fuente aquí**. Opera sobre el
repositorio hermano `raraya2607-creator/Gobernanza-de-la-IA`, que
contiene la documentación real (informes, PAT, Gestor de Seguimientos,
Cubo de Riesgos, códigos de gobernanza) y sus cuatro skills de
proyecto. Antes de responder una consulta de control, confirmá que ese
repositorio está adjunto a la sesión y leé su `CLAUDE.md`.

## Reglas de trabajo

- **Cero alucinaciones.** Todo diagnóstico se basa exclusivamente en lo
  ya cargado en `Gobernanza-de-la-IA`. Un vacío se declara literalmente
  "Dato no disponible en la documentación" — nunca se completa por
  inferencia.
- **Rama principal:** `main`.
- **Prompts:** se versionan en `prompts/`. Un cambio de prompt va en su
  propio commit, con fecha y justificación registradas en la bitácora
  de cambios del propio archivo.
- **Evaluaciones:** todo cambio de prompt o skill se valida contra
  `evaluaciones/` antes de comitear.

## Estructura

| Carpeta | Contenido |
| :--- | :--- |
| `prompts/` | Prompt de sistema de ARIA, versionado con bitácora de cambios |
| `knowledge/` | Mapa de las fuentes reales, en el repositorio `Gobernanza-de-la-IA` |
| `skills/` | Capacidades específicas de ARIA |
| `evaluaciones/` | Casos de prueba para validar el comportamiento de ARIA |
| `docs/` | Visión, alcance y decisiones del proyecto |
| `.claude/skills/` | Skills de proyecto para Claude Code (viajan con el repositorio) |
