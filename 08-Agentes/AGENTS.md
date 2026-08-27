# AGENTS.md — contrato para cualquier agente de IA

Si eres un agente entrando a este proyecto por primera vez, lee esto antes de tocar cualquier archivo.

## 1. Orienta antes de actuar

Lee, en este orden: `README.md` (raíz) → `00-Inicio/README.md` → `03-Procesos/Bitacora.md` (las últimas 2-3 entradas). Eso te da el mapa del proyecto y lo último que se hizo, antes de proponer nada.

## 2. Dónde documentar lo que hagas

- Cambio de diseño o de flujo → `01-Diseño/`
- Prompt nuevo que valga la pena guardar → `02-Prompts/<herramienta>/`
- Cualquier sesión de trabajo relevante → una línea nueva en `03-Procesos/Bitacora.md`, fecha ISO arriba de todo.
- Decisión importante (con alternativas descartadas) → un ADR nuevo en `04-Decisiones/`, usando la plantilla `0000-plantilla-adr.md`.
- Hallazgo de research o benchmarking → `05-Investigación/`.
- Referente o inspiración sin validar → `06-Referencias/`.
- Cambio de arquitectura técnica o de plan de migración → `07-Arquitectura/`.

## 3. Reglas generales

- No se borra el historial: las bitácoras y decisiones se acumulan, no se editan retroactivamente.
- El diseño (`01-Diseño/Design.md` y el sistema de diseño) es la fuente de verdad visual — si el código y el diseño documentado no coinciden, se pregunta antes de asumir cuál tiene razón.
- El proyecto es una app Android que se originó en Google AI Studio y está en proceso de conversión a Android nativo — cualquier propuesta de arquitectura debe tener en cuenta esa migración, documentada en `07-Arquitectura/`.
- Ante ambigüedad sobre una decisión de producto o diseño, se pregunta a Cristi en vez de asumir.
