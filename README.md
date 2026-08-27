# Bookstack — Sistema de documentación de Cristi

Este es el repositorio donde se documenta todo el proceso de diseño y construcción del proyecto: decisiones, prompts, procesos y referencias. La idea es que cualquier agente de IA (Claude Code, Codex, Cursor, etc.) que entre a trabajar en el proyecto pueda orientarse leyendo estos archivos, sin depender de que alguien le explique el contexto desde cero.

Cada carpeta numerada es un **"libro"**: un tema con su propio índice (`README.md`) y sus propios documentos. Se alimenta de forma incremental — no todo está lleno desde el día uno, y eso está bien.

## Índice de libros

| Libro | Contenido |
|---|---|
| [`00-Inicio/`](./00-Inicio/README.md) | Resumen del proyecto, estado actual, mapa rápido de todo lo demás. |
| [`01-Diseño/`](./01-Diseño/README.md) | `Design.md`, sistema de diseño, inventario de pantallas — la fuente de verdad visual. |
| [`02-Prompts/`](./02-Prompts/README.md) | Prompts usados en Google AI Studio, Claude Code, Codex y plantillas reutilizables. |
| [`03-Procesos/`](./03-Procesos/README.md) | Flujo de trabajo, bitácora cronológica, checklist de entrega. |
| [`04-Decisiones/`](./04-Decisiones/README.md) | Decisiones de diseño/arquitectura importantes, una por archivo (ADRs). |
| [`05-Investigación/`](./05-Investigacion/README.md) | Research con usuarios, benchmarking, métricas. |
| [`06-Referencias/`](./06-Referencias/README.md) | Inspiración, enlaces, referentes externos. |
| [`07-Arquitectura/`](./07-Arquitectura/README.md) | Arquitectura técnica y plan de migración desde Google AI Studio a Android. |
| [`08-Agentes/`](./08-Agentes/README.md) | Contrato de cómo debe comportarse cualquier agente de IA que trabaje aquí. |

## Convenciones

- **Nombres de archivo:** minúsculas y guiones (`nombre-del-archivo.md`), salvo los `README.md` de índice.
- **Fechas:** formato ISO `AAAA-MM-DD`, siempre al inicio de una entrada nueva en bitácoras o decisiones.
- **Decisiones (ADR):** se numeran `0001-titulo.md`, `0002-titulo.md`... nunca se borran, si una decisión cambia se documenta una nueva que reemplaza a la anterior y se enlazan entre sí.
- **Carpetas nuevas:** si hace falta un libro que no está en el índice, se agrega aquí arriba con un número siguiente y se crea con su propio `README.md`.

## Estado

- [x] Estructura de Bookstack creada — 2026-08-27
- [ ] Carpeta del proyecto Android conectada
- [ ] `Design.md` real migrado a `01-Diseño/`
- [ ] Primer prompt documentado
- [ ] Primera decisión (ADR) documentada
