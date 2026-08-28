# Propósito

Prompt guía completo (unifica las 3 partes de la serie) para aplicar buenas prácticas de gestión de contexto y memoria en un proyecto trabajado con Claude Code: analiza qué información crítica se pierde entre sesiones, crea una estructura de memoria persistente en disco, define el contenido de AGENTS.md y las reglas de comportamiento, y especifica el resultado esperado de la tarea.

# Prompt

```
Aplica las siguientes buenas prácticas de gestión de contexto y memoria:

### 1. Analiza el proyecto actual
- Revisa la estructura actual del repositorio.
- Identifica qué información crítica se pierde entre sesiones.
- Detecta archivos o contexto que se están cargando de forma ineficiente.

### 2. Crea la estructura de memoria persistente
Implementa la siguiente estructura de archivos (crea los que no existan) y añade al folder contexto, todas las decisiones importantes de diseño, como el design.md, decisiones.md:

/
├── AGENTS.md      # Archivo central de control (máximo 250-300 líneas)
├── decisions/     # Decisiones importantes con fecha y razonamiento
├── state/         # Estado actual del proyecto (hecho / pendiente / blockers)
├── skills/        # Procedimientos y habilidades reutilizables
├── gotchas/       # Problemas conocidos + soluciones
└── logs/          # Resúmenes comprimidos de sesiones importantes

### 3. Contenido que debes generar

AGENTS.md debe contener:
- Identidad y propósito del proyecto
- Reglas duras e invariantes
- Orden de lectura preferido de archivos
- Routing de skills (qué skill usar según el tipo de tarea)
- Definition of Done
- Instrucciones claras de cómo el agente debe comportarse con el contexto
- Punteros a las demás carpetas de memoria

En las carpetas:
- Crea archivos iniciales útiles basados en el estado real del proyecto.
- Extrae y organiza decisiones, estado actual, patrones y gotchas que ya existan en el código o en conversaciones previas (si las hay).
- Escribe de forma densa, clara y orientada a bajo consumo de tokens.

### 4. Reglas de comportamiento que debes instalar

Incluye en AGENTS.md las siguientes reglas de oro:

- El context window es caro y volátil. La memoria real debe vivir en archivos.
- Nunca cargar todo el historial ni todos los archivos del proyecto.
- Cargar solo lo estrictamente necesario para la tarea actual.
- Al final de cada sesión importante: actualizar state/, registrar decisiones y comprimir lo valioso en logs/.
- Preferir referenciar archivos antes que copiar contenido largo al prompt.
- Convertir procedimientos repetitivos en skills reutilizables.
- Mantener AGENTS.md conciso y de alta densidad de información.

### 5. Resultado esperado

Al terminar debes entregarme:

1. La estructura de archivos creada (lista de archivos y carpetas).
2. El contenido completo de AGENTS.md.
3. Resumen de lo que pusiste en cada carpeta.
4. Instrucciones claras de cómo debo usar este sistema a partir de ahora (incluyendo qué decirte al inicio de futuras sesiones).
5. Cualquier mejora adicional que consideres valiosa según las buenas prácticas de optimización de contexto.

Sé práctico, concreto y orientado a reducir tokens. No generes archivos innecesarios ni texto floreado. Prioriza densidad de información y utilidad real.
```

# Resultado

Pendiente de registrar. Reemplaza la versión anterior del archivo (que solo tenía la parte 1/3 de la serie); ahora incluye el prompt completo y unificado con las 3 partes.
