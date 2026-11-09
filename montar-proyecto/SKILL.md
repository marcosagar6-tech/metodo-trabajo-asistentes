---
name: montar-proyecto
description: Monta las instrucciones de trabajo (Claude, Codex y Copilot) en un proyecto nuevo o ya empezado. Usar con "/montar-proyecto", "monta el proyecto", "proyecto nuevo", "prepara las instrucciones de este proyecto".
---

# Montar un proyecto

Prepara la carpeta actual para trabajar con Claude, Codex y Copilot a la vez, con un estado compartido y una revisión por fases. La plantilla está en la carpeta `plantilla/`, junto a este archivo.

## Pasos
1. **Carpeta principal.** Busca la guía común (`AGENTS.md`) en la carpeta madre del proyecto o en las de más arriba. Si no la encuentras, pregunta al director dónde está su carpeta principal de proyectos. Esa ruta sustituye a `[CARPETA PRINCIPAL]` en todos los archivos.
2. **Copiar la plantilla** a la raíz del proyecto:
   - `AGENTS.md`, `CLAUDE.md`, `Estado del proyecto.md` y `REVISION.md`, tal cual.
   - `plantilla/claude/agents/` → `.claude/agents/`
   - `plantilla/github/copilot-instructions.md` → `.github/copilot-instructions.md`
   (En la plantilla no llevan punto para que se vean al compartirla. En el proyecto sí, porque es donde los leen los asistentes.)
3. **Si algo ya existe, no sobrescribas nada.** Añade las reglas que falten respetando las propias del proyecto y guarda una copia de cómo estaba en `Descartado/Instrucciones anteriores/` con nombre «… anterior.md». En `.claude/` y `.github/` copia solo lo que no exista y no toques ajustes ni permisos (`settings*.json`, `launch.json`…). Si un agente ya existe con el mismo nombre, conserva los dos y pregunta cuál vale. Si dos reglas chocan, márcalo con `[VERIFICAR]` y pregunta.
4. **Rellenar.** Cambia `[NOMBRE DEL PROYECTO]` por el nombre de la carpeta y pon la fecha de hoy en el `Estado`.
5. **Preguntar** lo que falte para el apartado «Proyecto» de `CLAUDE.md`, como mucho 3 preguntas: qué es, estado comercial y lo que no se pueda deducir mirando los archivos.
6. **Si el proyecto no es una web**, adapta `constructor` y `disenador` a lo que sea (documento, app, presentación…).
7. **Enseñar el montaje** al director (qué has creado, qué has juntado y qué queda pendiente de su decisión) y no empieces a trabajar sin su okey.
