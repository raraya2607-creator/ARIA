# ARIA

Agente de control de la Gobernanza de la Auditoría Interna del
Ministerio de Vivienda y Asentamientos Humanos (MIVAH).

> El significado exacto de la sigla "ARIA" no está documentado. El rol
> operativo sí: ver `prompts/prompt-sistema.md`.

## Qué controla

ARIA mantiene bajo supervisión seis frentes de la gestión de la
Auditoría Interna, documentados en `prompts/prompt-sistema.md`:

1. **Seguimiento de Recomendaciones** — estado y vencimiento de cada
   recomendación de auditoría (Art. 22 inciso g) y Art. 12, Ley 8292).
2. **Planes Anuales de Trabajo (PAT)** — presupuesto de días-persona,
   universo auditable y estudios planificados por año.
3. **Cubo de Riesgos** — riesgos institucionales y de la Auditoría
   Interna, insumo del PAT basado en riesgos.
4. **Control de Auditorías a Desarrollar en el Año** — avance de cada
   estudio del PAT frente a los informes ya emitidos.
5. **Códigos de Buena Gobernanza** — cumplimiento del Código de Ética,
   el Código de Buena Gobernanza y la Política de Gobernanza de IA en
   toda recomendación o automatización.
6. **Plan Estratégico e Indicadores Anuales de Objetivos Estratégicos**
   — cumplimiento anual de los 12 objetivos estratégicos de la
   Auditoría Interna, mapeo de estudios/informes por objetivo, estado
   de sus recomendaciones y % de Universo Auditable atendido.

## Fuente de conocimiento

ARIA no almacena aquí los documentos fuente. Los seis módulos se
alimentan del repositorio `raraya2607-creator/Gobernanza-de-la-IA`, que
contiene la documentación real cargada y las skills que la mantienen.
Ver el detalle de correspondencia en `knowledge/README.md`.

## Estructura

| Carpeta | Contenido |
| :--- | :--- |
| `prompts/` | Prompt de sistema de ARIA, versionado con bitácora de cambios |
| `knowledge/` | Mapa de las fuentes reales, en el repositorio `Gobernanza-de-la-IA` |
| `tableros/` | Tableros de control generados por corte, por año |
| `skills/` | Skills o capacidades específicas del agente |
| `evaluaciones/` | Casos de prueba y criterios para validar las respuestas del agente |
| `docs/` | Documentación del proyecto: visión, alcance, decisiones |
| `.claude/skills/` | Skills de proyecto para Claude Code (viajan con el repositorio) |

Cada carpeta tiene un `README.md` que describe qué debe contener.
