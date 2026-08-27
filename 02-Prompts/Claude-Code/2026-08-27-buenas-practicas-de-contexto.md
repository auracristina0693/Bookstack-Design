# Propósito

Prompt guía (1 de una serie de 3) para aplicar buenas prácticas de gestión de contexto y memoria en un proyecto trabajado con Claude Code: primero analiza qué información crítica se pierde entre sesiones, y luego crea una estructura de memoria persistente en disco para que las decisiones de diseño y el estado del proyecto sobrevivan entre sesiones.

# Prompt

```
Aplica las siguientes buenas prácticas de gestión de contexto y memoria:

### 1. Analiza el proyecto actual
- Revisa la estructura actual del repositorio.
- Identifica qué información crítica se pierde entre sesiones.
- Detecta archivos o contexto que se están cargando de forma ineficiente.

### 2. Crea la estructura de memoria persistente
Implementa la siguiente estructura de archivos (crea los que no existan) y añade al folder contexto, todas las decisiones importantes de diseño, como el design.md, decisiones.md:

├── AGENTS.md      # Archivo central de control (máximo 250-300 líneas)
├── decisions/     # Decisiones importantes con fecha y razonamiento
├── state/         # Estado actual del proyecto (hecho / pendiente / blockers)
├── skills/        # Procedimientos y habilidades reutilizables
├── gotchas/       # Problemas conocidos + soluciones
└── logs/          # Resúmenes comprimidos de sesiones importantes
```

# Resultado

Pendiente de registrar. Es el prompt 1/3 de una serie — anotar aquí qué tan bien funcionó y ajustar cuando se use, y documentar los prompts 2/3 y 3/3 de la serie cuando lleguen.
