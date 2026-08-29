# Propósito
Plantilla reutilizable para construir, con ayuda de un asistente de IA, una presentación web interactiva para presentar cualquier proyecto a stakeholders (Demo Day, Sprint Review, Kickoff, reunión de avance, etc.) — cubre desde el rol y contexto que se le da a la IA hasta los requisitos técnicos, restricciones y criterios de aceptación de la presentación. Generalizada a partir de un prompt original usado para el Demo Day de Glucky.

# Prompt
Rol: Eres un asistente de ingeniería frontend. Tu tarea es construir una presentación web interactiva para [tipo de reunión, ej. Demo Day, Sprint Review, Kickoff] de [nombre del producto/proyecto]. La presentación acompaña un guión hablado de [duración, ej. 5 minutos] y se navega con flechas del teclado.

Contexto del proyecto:

- Producto: [nombre del producto/proyecto]
- Para quién: [audiencia objetivo del producto]
- URL viva del demo: [URL del demo]
- Repositorio: [URL del repositorio]
- Feature: [feature o funcionalidad principal a mostrar]

Antes de escribir código:
1. Inspecciona el repositorio en tu máquina local.
2. Identifica el framework (Next.js, Vite, etc.), sistema de rutas, sistema de estilos (Tailwind, CSS Modules, styled-components) y componentes existentes.
3. Identifica tokens de color, tipografía y espaciado en design tokens o archivo equivalente.
4. Reutiliza estos elementos; no crees un design system nuevo.

Contenido de las diapositivas:

1. Portada:
   - [nombre del producto/proyecto]: [propuesta de valor en una línea]
   - [para quién es / a quién va dirigido]
   - [URL del demo]

2. Problema (0:00-0:30):
   - [problema que resuelve el proyecto]
   - Usuario: [perfil de usuario objetivo]
   - [qué necesita o busca el usuario]
   - Criterio de éxito: [cómo se sabe que el proyecto funcionó]

3. Demo en vivo (0:30-2:30):
   - [Botón grande: Abrir [URL del demo]]
   - Paso 1: [primer paso del flujo a mostrar]
   - Paso 2: [segundo paso del flujo a mostrar]
   - Fuera de cámara: [qué NO está listo todavía / limitaciones conocidas]

4. Decisiones: qué delegué y qué retuve (2:30-4:30):
   - Delegué a [herramientas de IA usadas]: [qué tareas se delegaron, ej. layouts, borradores de microcopy]
   - Retuve: [qué se mantuvo bajo control humano, ej. tono final, alcance, definición de éxito, verificación de riesgos]
   - Por qué retuve: [riesgo específico del dominio del proyecto]
   - Tarea estrella: [tarea puntual que mejor representa ese criterio humano]

5. Verificación y transparencia (2:30-4:30):
   - Herramientas: [herramientas usadas y para qué, ej. Cursor para layouts, ChatGPT para microcopy, Vercel para deploy]
   - Datos que entraron: [qué datos/información alimentó la demo]
   - QA: [qué se verificó — flujo completo, accesibilidad, contraste, etc.]
   - Hallazgo grave: [algo riesgoso que la IA propuso/inventó y hubo que corregir o eliminar]
   - No alcancé: [qué quedó pendiente de validar, ej. pruebas con usuarios reales, analítica]

6. Cierre: postmortem y aprendizaje (4:30-5:00):
   - Pensaba que lo difícil sería: [tu suposición inicial]
   - Realmente fue: [lo que resultó ser el verdadero reto]
   - Si reiniciara: [qué harías distinto desde el inicio]
   - Aprendizaje clave: [la lección principal de este proceso]

Requisitos técnicos:
- Navegación: flechas izquierda/derecha del teclado entre diapositivas. Indica en pantalla cuál es la tecla activa.
- Responsive: legible en mobile (375px), tablet y desktop. Una diapositiva a la vez, nunca dos.
- Tipografía: grande, legible a tres metros. Mínimo 24px en cuerpo, 36px en títulos.
- Contraste: WCAG AA como mínimo en todos los textos. Usa tokens de color del design system.
- Semántica: encabezados h1, h2, h3 según nivel. Listas con <ul> y <li>.
- Foco: visible y de contraste alto en todos los botones y elementos interactivos.
- Accesibilidad: respeta prefers-reduced-motion; sin animaciones si está activo.

Prohibido:
- Inventar datos, métricas, pantallas o features que no estén en el contexto.
- Mostrar código fuente o snippets en las diapositivas.
- Reemplazar o modificar la URL viva [URL del demo].
- Tocar el flujo principal del producto ni otras rutas existentes.
- Añadir analítica, telemetría o llamadas a backend.
- Crear mockups ficticios de pantallas no implementadas.

Criterios de aceptación:
1. Ruta [ruta de la presentación] existe, aislada del flujo principal, sin modificar otras rutas.
2. Seis diapositivas se navegan con flechas del teclado; izquierda va atrás, derecha va adelante.
3. Una sola diapositiva visible por vez, 100% del viewport.
4. Tipografía mínimo 24px cuerpo, 36px títulos. Legible a tres metros.
5. Botón «Abrir demo en vivo» en diapositiva 3 apunta a [URL del demo] y abre en pestaña nueva.
6. Contraste WCAG AA en todos los textos verificado con herramienta de accesibilidad.
7. Recorrido completo con solo teclado: Tab, Enter, flechas. Sin ratón obligatorio.
8. Verificado en móvil (375px, 768px, 1024px) y desktop. Sin scroll dentro de diapositiva.

Antes de darte por terminado:
- Levanta el servidor de desarrollo.
- Abre http://localhost:3000/[ruta de la presentación] (o el puerto de tu app) en navegador.
- Recorre todas las seis diapositivas con flechas del teclado.
- Verifica tipografía, contraste y que el botón de demo en vivo funciona.
- Prueba en móvil.
- Indica la ruta local donde revisar la presentación y confirma que está lista.

# Resultado
Pendiente — aún no se ha probado.
