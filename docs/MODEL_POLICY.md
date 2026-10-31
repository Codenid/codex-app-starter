# Política de modelos y cuota

Los nombres, disponibilidad y límites cambian. Elegir en el selector real de Codex en VS Code; esta política no configura el modelo automáticamente.

| Trabajo | Nivel recomendado | Escalar cuando |
| --- | --- | --- |
| Formato, tests simples, documentación, UI delimitada | Económico / razonamiento bajo | Fallos reproducibles no triviales |
| Endpoints, integraciones, lógica de negocio | Estándar / razonamiento medio | Contratos o dependencias ambiguas |
| Diseño de arquitectura, migraciones, debugging complejo | Razonamiento alto | Hay decisiones de alto impacto o riesgo |
| Revisión crítica puntual | Máximo disponible, excepcionalmente | El beneficio justifica el coste |

## Protocolo
1. Definir tarea y aceptación antes de elegir modelo.
2. Elegir el nivel mínimo que pueda cumplirla.
3. Limitar la exploración a archivos relevantes y una hipótesis comprobable.
4. Validar con comandos locales y tests.
5. Tras dos correcciones fallidas, detenerse y replantear; no repetir prompts equivalentes.
6. Si se cambia de modelo, entregar resumen de estado, archivos y errores, no todo el historial.

## Medición
Registrar en USAGE_LOG: tarea, modelo, tiempo, cuota visible antes/después (si existe), iteraciones y resultado. Comparar costo por tarea **validada**, no por número de mensajes.
