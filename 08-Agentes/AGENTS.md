# AGENTS.md — contrato para cualquier agente de IA

Si eres un agente entrando a este repositorio por primera vez, lee esto antes de tocar cualquier archivo.

## 1. Orienta antes de actuar

Lee, en este orden: `README.md` (raíz) → `00-Inicio/README.md` (incluye qué proyectos están documentados hoy) → `03-Procesos/Bitacora.md` (las últimas 2-3 entradas). Eso te da el mapa general y lo último que se hizo, antes de proponer nada.

## 2. Dónde documentar lo que hagas

Este repositorio documenta **todos los proyectos de Cristi**, no uno solo. Si el libro correspondiente ya tiene contenido de más de un proyecto, usa una subcarpeta con el nombre del proyecto (`01-Diseño/<proyecto>/`, `07-Arquitectura/<proyecto>/`); si son entradas sueltas en un mismo archivo (bitácora, un ADR), menciona a qué proyecto pertenece al inicio de la entrada.

- Cambio de diseño o de flujo → `01-Diseño/`
- Prompt nuevo que valga la pena guardar → `02-Prompts/<herramienta>/`
- Cualquier sesión de trabajo relevante → una línea nueva en `03-Procesos/Bitacora.md`, fecha ISO arriba de todo.
- Decisión importante (con alternativas descartadas) → un ADR nuevo en `04-Decisiones/`, usando la plantilla `0000-plantilla-adr.md`.
- Hallazgo de research o benchmarking → `05-Investigación/`.
- Referente o inspiración sin validar → `06-Referencias/`.
- Cambio de arquitectura técnica o de plan de migración de algún proyecto → `07-Arquitectura/`.

## 3. Reglas generales

- No se borra el historial: las bitácoras y decisiones se acumulan, no se editan retroactivamente.
- El diseño documentado en `01-Diseño/` (por proyecto) es la fuente de verdad visual — si el código y el diseño documentado no coinciden, se pregunta antes de asumir cuál tiene razón.
- Cada proyecto puede estar en una etapa distinta (uno migrando desde Google AI Studio a Android nativo, otro recién empezando, etc.) — no asumas el contexto de un proyecto por lo que se sabe de otro; revisa `00-Inicio/` para saber cuáles hay documentados.
- Ante ambigüedad sobre una decisión de producto o diseño, se pregunta a Cristi en vez de asumir.
