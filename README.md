# Codex App Starter

Plantilla ligera, agnóstica al stack, para desarrollar aplicaciones con Codex en VS Code sin desperdiciar cuota.

## Inicio rápido
1. En GitHub, usa **Use this template** (si habilitas la opción Template repository) o copia este repositorio.
2. Completa `docs/REQUIREMENTS.md` y `docs/ARCHITECTURE.md`.
3. Desglosa el MVP en `docs/PLAN.md` con tareas de 30–90 minutos y criterios verificables.
4. En Codex: «Lee AGENTS.md y docs/PLAN.md. Propón la próxima tarea, sin modificar archivos».
5. Aprueba una tarea; implementa, prueba, revisa el diff y haz commit.
6. Actualiza estado, decisiones y siguiente paso antes de abrir otra sesión.

## Principios
- Primero planificar, luego implementar; una tarea por ejecución.
- Seleccionar el modelo por complejidad, no por costumbre.
- Pruebas deterministas y herramientas locales antes de más razonamiento.
- Presupuesto de exploración y máximo dos ciclos de corrección automática.
- No inventar métricas de ahorro: registrar consumo real en `docs/USAGE_LOG.md`.

## Archivos clave
- `AGENTS.md`: reglas operativas del agente.
- `docs/MODEL_POLICY.md`: selección de modelos y escalamiento.
- `docs/PLAN.md`: backlog y estado.
- `docs/TASK_TEMPLATE.md`: contrato por tarea.
- `docs/DECISIONS.md`: ADRs breves.
- `docs/USAGE_LOG.md`: seguimiento del consumo.

No contiene una aplicación ejecutable: es una plantilla de proceso, no un starter de un framework concreto.
