# Método de trabajo con Claude, Codex y Copilot

Una forma ordenada de trabajar con varios asistentes de IA a la vez: tú diriges, Claude construye, Codex revisa y Copilot ayuda en VS Code. Todos leen el mismo estado del proyecto, así que puedes pasar de uno a otro sin repetir nada.

## Qué hay aquí
- **Guía común/**: las reglas que valen para todos tus proyectos (`AGENTS.md` para todos los asistentes y `CLAUDE.md` con lo propio de Claude).
- **montar-proyecto/**: una skill que prepara cualquier carpeta de proyecto con sus instrucciones, su estado, su revisión y 5 agentes de Claude (diseñador, constructor, supervisor, redactor y ayudante).

## Instalación (una sola vez)
1. Descarga este repositorio: botón verde **Code → Download ZIP**, y descomprímelo.
2. Crea una carpeta principal para tus proyectos (por ejemplo, `Proyectos` en el Escritorio) y copia dentro los dos archivos de **Guía común**.
3. Copia la carpeta **montar-proyecto** en:
   - Claude Code: `~/.claude/skills/`
   - Codex: `~/.codex/skills/`
4. Para que Claude y Codex lean la guía en cualquier carpeta, añade esta línea:
   - Claude, en `~/.claude/CLAUDE.md`: `@/RUTA/A/TU/CARPETA/CLAUDE.md`
   - Codex, en `~/.codex/AGENTS.md`: `Antes de trabajar, lee y sigue /RUTA/A/TU/CARPETA/AGENTS.md como guía común.`

## Uso
- **Proyecto nuevo:** crea su carpeta dentro de tu carpeta principal, abre Claude en ella y escribe `/montar-proyecto`. Te hará como mucho 3 preguntas y te enseñará el montaje.
- **Cada fase:** al terminar, Claude te deja un mensaje listo para copiar en un chat nuevo. Si lo pierdes:
  ```
  Lee CLAUDE.md, Estado del proyecto.md y REVISION.md y sigue con la tarea siguiente.
  ```
- **Revisión:** cuando Claude termina, pásale el trabajo a Codex para una revisión independiente.

Adáptalo a tu manera de trabajar: todo son archivos de texto.
