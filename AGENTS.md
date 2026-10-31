# Reglas de Codex

## Objetivo
Entregar software verificable con mínimo alcance, retrabajo y consumo innecesario.

## Antes de editar
1. Leer `docs/REQUIREMENTS.md`, `docs/PLAN.md` y las secciones relevantes de `docs/ARCHITECTURE.md`.
2. Identificar una tarea aprobada, sus criterios de aceptación y archivos probablemente afectados.
3. Inspeccionar solo archivos pertinentes. Buscar rutas/símbolos antes de leer archivos completos.
4. Si el alcance es ambiguo o implica cambios de arquitectura, detenerse y solicitar decisión.

## Implementación
- Una tarea a la vez; evitar mejoras no solicitadas.
- Preferir componentes existentes y dependencias ya instaladas.
- No cambiar contratos públicos, esquemas, autenticación ni infraestructura sin aprobación.
- No agregar dependencias ni realizar refactorizaciones transversales sin justificarlo.
- Nunca imprimir ni almacenar secretos, tokens o datos personales en logs.
- No ejecutar comandos destructivos ni despliegues sin aprobación explícita.

## Verificación
- Ejecutar primero las pruebas más pequeñas relacionadas con el cambio.
- No ejecutar la suite completa si no es necesaria; hacerlo antes del merge cuando aplique.
- Máximo dos ciclos automáticos de reparación; después informar diagnóstico y pedir orientación.
- Si faltan pruebas, declarar qué no pudo validarse.

## Cierre
- Reportar resumen, archivos cambiados, pruebas y resultados, riesgos y siguiente paso.
- Actualizar `docs/PLAN.md` solo con evidencia de cumplimiento.
- Registrar decisiones arquitectónicas en `docs/DECISIONS.md`.
- No afirmar que algo funciona sin prueba o evidencia.

## Gestión de contexto
- Evitar pegar logs extensos; resumir y citar archivos/rutas.
- Al iniciar una sesión nueva, retomar desde el plan y el último commit, no reconstruir todo el historial.
- La selección de modelo la realiza el usuario según `docs/MODEL_POLICY.md`; este archivo no cambia el modelo automáticamente.
