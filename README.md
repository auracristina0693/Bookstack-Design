# Bookstack — Documentación de Cristi

Esta es la librería de documentación de Cristi: un solo lugar donde queda registrado el proceso, las decisiones, los prompts y las referencias de **todos sus proyectos**, no de uno en particular. La idea es que cualquier agente de IA (Claude Code, Codex, Cursor, Claude en Cowork, etc.) que entre a trabajar en cualquiera de sus proyectos pueda orientarse leyendo estos archivos, sin depender de que alguien le explique el contexto desde cero.

Cada carpeta numerada es un **"libro"**: un tema con su propio índice (`README.md`) y sus propios documentos. Se alimenta de forma incremental — no todo está lleno desde el día uno, y eso está bien.

## Cómo conviven varios proyectos aquí

Los libros están organizados por **tipo de información**, no por proyecto. Cuando algo aplica a un proyecto específico (un diseño, una arquitectura, un plan de migración), se distingue así:

- Si un libro va a tener contenido voluminoso de varios proyectos, se organiza en subcarpetas por proyecto — por ejemplo `01-Diseño/nombre-del-proyecto/`.
- Si son entradas sueltas dentro de un mismo archivo (como la bitácora o un ADR), el nombre del proyecto se menciona al inicio de la entrada.

## Índice de libros

| Libro | Contenido |
|---|---|
| [`00-Inicio/`](./00-Inicio/README.md) | Qué es esta librería, qué proyectos documenta hoy, mapa rápido de todo lo demás. |
| [`01-Diseño/`](./01-Diseño/README.md) | Diseño y UX de cada proyecto — sistemas de diseño, inventarios de pantallas, la fuente de verdad visual. |
| [`02-Prompts/`](./02-Prompts/README.md) | Prompts usados en Google AI Studio, Claude Code, Codex y plantillas reutilizables. |
| [`03-Procesos/`](./03-Procesos/README.md) | Flujo de trabajo, bitácora cronológica, checklist de entrega. |
| [`04-Decisiones/`](./04-Decisiones/README.md) | Decisiones de diseño/arquitectura importantes, una por archivo (ADRs). |
| [`05-Investigación/`](./05-Investigacion/README.md) | Research con usuarios, benchmarking, métricas. |
| [`06-Referencias/`](./06-Referencias/README.md) | Inspiración, enlaces, referentes externos. |
| [`07-Arquitectura/`](./07-Arquitectura/README.md) | Arquitectura técnica de cada proyecto que lo amerite. |
| [`08-Agentes/`](./08-Agentes/README.md) | Contrato de cómo debe comportarse cualquier agente de IA que trabaje aquí. |

## Convenciones

- **Nombres de archivo:** minúsculas y guiones (`nombre-del-archivo.md`), salvo los `README.md` de índice.
- **Fechas:** formato ISO `AAAA-MM-DD`, siempre al inicio de una entrada nueva en bitácoras o decisiones.
- **Decisiones (ADR):** se numeran `0001-titulo.md`, `0002-titulo.md`... nunca se borran, si una decisión cambia se documenta una nueva que reemplaza a la anterior y se enlazan entre sí.
- **Carpetas nuevas:** si hace falta un libro que no está en el índice, se agrega aquí arriba con un número siguiente y se crea con su propio `README.md`.

## Estado

- [x] Estructura de Bookstack creada — 2026-08-27
- [x] Repositorio conectado a GitHub y primer push hecho — 2026-08-27
- [x] Reencuadrado como librería de documentación general, no de un solo proyecto — 2026-08-27
- [ ] Primer proyecto real documentado de punta a punta
- [ ] Primer prompt documentado
- [ ] Primera decisión (ADR) documentada
