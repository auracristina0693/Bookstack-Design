# Bitácora

Registro cronológico corto. Una entrada nueva arriba de todo, no se editan las anteriores.

---

## 2026-08-30

- Se guarda en `02-Prompts/AI-Studio/` el prompt "Editar imagen exacta en Google AI Studio", para pedir un cambio puntual sobre una imagen ya subida (ej. reemplazar solo una foto o un screenshot) sin que el modelo regenere ni reinterprete el resto de la imagen.

## 2026-08-28

- Se reemplaza el prompt "Buenas prácticas de contexto" en `02-Prompts/Claude-Code/2026-08-27-buenas-practicas-de-contexto.md`: la versión anterior solo tenía la parte 1/3 (incompleta); se sustituye por el prompt completo y unificado (partes 1/3, 2/3 y 3/3: análisis del proyecto, estructura de memoria persistente, contenido de AGENTS.md, reglas de comportamiento y resultado esperado).

## 2026-08-27

- Se guarda en `02-Prompts/Claude-Code/` el prompt "Buenas prácticas de contexto" (1/3 de una serie), sobre cómo analizar qué se pierde entre sesiones y crear una estructura de memoria persistente (AGENTS.md, decisions/, state/, skills/, gotchas/, logs/).
- Se crea la estructura de Bookstack para documentar diseño, prompts, procesos, decisiones, investigación, referencias y arquitectura del proyecto.
- Carpeta conectada: `Bookstack_Cristi` (vacía al momento de crear la estructura).
- Pendiente: conectar la carpeta del proyecto Android original (creado en Google AI Studio) para migrar `Design.md`, analizar la arquitectura actual y proponer el plan de conversión a app Android nativa.
- Se conecta el repo `Bookstack-Design` a Git local (Git ya estaba instalado en el equipo) y se hace el primer push exitoso desde PowerShell, usando el Git Credential Manager para autenticar sin necesidad de token.
- Se crea el skill `actualizar-bookstack`: decide en qué carpeta documentar información nueva, la redacta siguiendo las convenciones de este archivo y de `08-Agentes/AGENTS.md`, y siempre entrega los comandos de git listos para pegar en PowerShell — el push nunca se hace desde la nube, solo desde la máquina local.
- Se reencuadra Bookstack: deja de ser la documentación de un solo proyecto y pasa a ser la librería general de Cristi para todos sus proyectos. Se actualizan `README.md`, `00-Inicio/`, `01-Diseño/`, `07-Arquitectura/` y `08-Agentes/AGENTS.md` para reflejarlo.
