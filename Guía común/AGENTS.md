# Guía común de trabajo

La leen todos los asistentes (Claude, Codex y Copilot) en cualquier proyecto de esta carpeta. Antes de trabajar, identifica el proyecto y lee sus instrucciones y su `Estado del proyecto.md`. Si algo choca, mandan las instrucciones del proyecto y, por encima de todo, el encargo explícito del director.

## Equipo

- **El director eres tú.** Decides prioridades, alcance, presupuesto y aprobaciones finales.
- **Claude Code**: implementaciones amplias, cambios coordinados en muchos archivos, fases largas y recursos propios de Claude (skills, agentes).
- **Codex**: revisión independiente, diagnóstico, segunda opinión, presentaciones e imágenes.
- **Copilot**: consultas y cambios pequeños dentro de VS Code, y comprobar entregas cuando el director lo pide.
- Es una preferencia, no un límite. Si a alguien le falta uso, pasa la parte al siguiente capaz con un traspaso corto.
- Una skill, un agente o una configuración se encargan al asistente de esa plataforma; los demás solo la revisan.

## Coordinación

- Los chats no se comunican entre sí. «Pasar trabajo a otro asistente» significa dejarle al director un único bloque breve, listo para copiar en el otro chat.
- Un solo asistente edita un conjunto de archivos a la vez. Se pueden pedir dos **opiniones** independientes, pero nunca la misma **implementación** a dos asistentes.
- Si se pide una revisión o una lista de propuestas, no se aplican cambios sin autorización.
- En tareas con varias partes, recomienda antes quién hace cada una, quién revisa y la alternativa si falta uso. En tareas pequeñas u obvias, sin ceremonia.
- Al terminar una intervención, di siempre quién sigue: el director, Claude, Codex, Copilot o nadie.
- Cuando Codex revise un trabajo de Claude y haga falta que Claude siga, termina con un único bloque de código autosuficiente (proyecto, objetivo, hallazgos, archivos, comprobaciones y límites). Si no hace falta, dilo.

## Tareas en internet

- Cuando al director le toque hacer algo en internet (formularios, fichas, dominios, buscar datos…), déjale debajo de los pasos un único bloque listo para pegar en **Claude in Chrome**: qué conseguir, en qué web, los datos exactos, cómo saber que está terminado y qué contar al acabar.
- En ese bloque, que pare y pregunte antes de pagar, enviar, publicar, borrar o aceptar condiciones, y que nunca escriba contraseñas.

## Chats y contexto

- Un chat por fase u objetivo. Las correcciones pequeñas siguen en el mismo chat.
- Si cambia el proyecto, la fase o la dirección, actualiza primero el estado y deja un único bloque para el chat nuevo.
- El chat nuevo se pone al día con las instrucciones, `Estado del proyecto.md` y `REVISION.md`; no hace falta la conversación anterior.
- Cada asistente lee solo lo que necesita su parte y no repite análisis o pruebas que ya estén apuntados y sigan valiendo.

## Proyecto nuevo

- Para preparar un proyecto se usa la skill `/montar-proyecto`. Si al empezar en una carpeta falta `CLAUDE.md` o `AGENTS.md`, propón hacer el montaje antes que nada.

## Al empezar y terminar

- Confirma la carpeta del proyecto y sus archivos vigentes; no confundas versiones de «Descartado» o «Archivados» con la activa.
- Mira el estado comercial antes de decidir el alcance: propuesta, esperando respuesta, aceptado, en producción, publicado o archivado. Antes de que el cliente acepte, solo lo necesario para vender bien la propuesta.
- Al terminar trabajo importante, actualiza el estado del proyecto con decisiones, cambios y siguiente paso.
- Limita los cambios a lo pedido. **No publiques, compres, envíes ni borres nada sin el visto bueno del director.**
- No inventes datos (clientes, opiniones, cifras, precios, horarios): lo que falte, `[PENDIENTE]`; lo que haya que comprobar, `[VERIFICAR]`.
- En temas legales, da una lista de comprobaciones preliminar; no la presentes como asesoramiento legal definitivo.

## Nombres y orden de carpetas

- Nombres sencillos en español que se entiendan solos. Nada de números delante, guiones bajos, códigos, abreviaturas ni fechas si no hacen falta.
- Cada proyecto usa las mismas carpetas básicas, solo las que hagan falta: «Web», «Presentaciones», «Presupuestos», «Análisis», «Fotos y logos», «Encargos» y «Descartado».
- Lo viejo y lo que ya no se usa va a «Descartado» del propio proyecto. No se borra nada sin el visto bueno del director.
- Dentro de las carpetas de código (`index.html`, `css`, `js`, `img`…) se mantienen los nombres técnicos.
- Los archivos de los asistentes conservan su nombre y su sitio: `CLAUDE.md`, `AGENTS.md`, `Estado del proyecto.md`, `REVISION.md`, `.claude/`, `.github/`, `.vscode/`.
- Si mueves o renombras algo, arregla los sitios que lo nombran.
