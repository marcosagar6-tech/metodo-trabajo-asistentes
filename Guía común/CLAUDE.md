# Guía de Claude Code

Aquí solo van las reglas propias de Claude. La guía común de todos los asistentes está en `AGENTS.md`, en esta misma carpeta. El `CLAUDE.md` de cada proyecto añade lo suyo y, si algo choca, manda el del proyecto.

@AGENTS.md

## Alcance según el estado comercial
- Antes de que el cliente acepte: solo lo necesario para vender bien la propuesta (análisis corto, muestra, presentación y presupuesto).
- Después de la aceptación o el primer pago: el trabajo completo.
- Si el proyecto espera respuesta o está en pausa, no seguir construyendo salvo que el director lo pida.

## Arranque de cada fase (un chat nuevo por fase)
- Leer solo `Estado del proyecto.md` y `REVISION.md` del proyecto, y ejecutar la comprobación automática si existe.
- Después, solo los archivos que nombre la tarea en el `Estado`.

## Cierre de cada fase
1. Anotar el veredicto en `REVISION.md` y poner al día el `Estado`: quitar lo hecho, dejar escrita la tarea siguiente y rellenar el traspaso.
2. Escribir: **"Cambia de chat ahora para seguir con el estado"**.
3. Debajo, solo dentro de un bloque de código:
   ```
   Lee CLAUDE.md, Estado del proyecto.md y REVISION.md y sigue con la tarea siguiente: [tarea en una frase].
   ```
- Después de una implementación de Claude, lo normal es que siga Codex con una revisión independiente.

## Con el director
- Corto, sin tecnicismos y paso a paso. Recomendar una opción, no dar listas largas.
- Todo lo que haya que copiar y pegar va solo en un bloque de código.

## Agentes y modelos
- En el trabajo de un proyecto, usar sus agentes (`disenador`, `constructor`, `supervisor`, `redactor`, `ayudante`).
- Opus: decisiones, diseño nuevo, supervisor y legal. Sonnet: ejecutar lo ya decidido, traducir y comprobar.
- Los arreglos de 1 a 5 líneas los hace Claude directamente, sin agentes.
- TRASPASO a un agente (15 líneas como máximo): objetivo · rutas exactas · lo ya hecho · lista cerrada de cambios · criterios de aceptación · formato de respuesta.
- Como mucho 3 agentes a la vez, y de ellos como mucho 2 con Opus.

## Revisión
- Cada encargo lleva sus criterios de aceptación.
- Supervisor nuevo en cada fase, que lee `REVISION.md`. La ronda 2 solo comprueba los 🔴/🟠 abiertos; los 🟡 se arreglan sin volver a revisar.
- Como mucho 2 rondas. Si sigue un 🔴, decide el director.
