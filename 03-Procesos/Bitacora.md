# Bitácora

Registro cronológico corto. Una entrada nueva arriba de todo, no se editan las anteriores.

---

## 2026-08-27

- Se crea la estructura de Bookstack para documentar diseño, prompts, procesos, decisiones, investigación, referencias y arquitectura del proyecto.
- Carpeta conectada: `Bookstack_Cristi` (vacía al momento de crear la estructura).
- Pendiente: conectar la carpeta del proyecto Android original (creado en Google AI Studio) para migrar `Design.md`, analizar la arquitectura actual y proponer el plan de conversión a app Android nativa.
- Se conecta el repo `Bookstack-Design` a Git local (Git ya estaba instalado en el equipo) y se hace el primer push exitoso desde PowerShell, usando el Git Credential Manager para autenticar sin necesidad de token.
- Se crea el skill `actualizar-bookstack`: decide en qué carpeta documentar información nueva, la redacta siguiendo las convenciones de este archivo y de `08-Agentes/AGENTS.md`, y siempre entrega los comandos de git listos para pegar en PowerShell — el push nunca se hace desde la nube, solo desde la máquina local.
