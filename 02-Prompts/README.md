# 02 · Prompts

Biblioteca de prompts usados a lo largo del proyecto, organizada por herramienta.

## Subcarpetas

- **`AI-Studio/`** — prompts usados en Google AI Studio durante la etapa inicial del proyecto.
- **`Claude-Code/`** — prompts usados con Claude Code para desarrollo, análisis o refactor.
- **`Codex/`** — prompts usados con Codex (o herramientas equivalentes).
- **`Plantillas/`** — prompts reutilizables, ya probados, listos para adaptar a una tarea nueva.

## Convención de archivo

Un prompt por archivo: `AAAA-MM-DD-proposito-corto.md`, con esta forma mínima:

```md
# Propósito
(qué se buscaba lograr)

# Prompt
(el prompt tal cual se usó)

# Resultado
(qué tan bien funcionó, qué se ajustaría la próxima vez)
```

Los prompts que funcionan bien y se repiten pasan a `Plantillas/`.
