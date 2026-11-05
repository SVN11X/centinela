# 0003. Respuestas en tres niveles

| Estado | Fecha | Etapa |
|---|---|---|
| Propuesta | 2026-11-05 | 0 |

## Contexto

Los modelos que caben en el reloj son chicos y pueden equivocarse. En una emergencia, una respuesta equivocada puede causar daño. Además, encender el módulo de IA toma tiempo y energía.

## Opciones consideradas

| Opción | A favor | En contra |
|---|---|---|
| Todo lo responde la IA | Simple de construir | Lento, gasta batería y puede inventar pasos críticos |
| Tres niveles, de lo revisado a lo generado | Rápido, seguro y ahorra batería | Exige preparar y revisar contenido antes |

## Decisión

| Nivel | Qué hace | Lo resuelve | Tiempo esperado |
|---|---|---|---|
| 1. Respuesta preparada | Busca en un banco de preguntas y respuestas revisadas | ESP32-S3 | Al instante |
| 2. Fragmento de guía | Muestra el párrafo de guía más parecido, con su fuente | ESP32-S3 | Pocos segundos |
| 3. Respuesta con IA | El modelo responde apoyado en 1 o 2 fragmentos de guía | Módulo de IA | 10 a 25 s, más el arranque |

Los procedimientos críticos salen siempre del nivel 1 y nunca los genera la IA.

## Consecuencias

- La etapa 2 debe producir el banco de respuestas y las guías en fragmentos.
- El banco se genera antes de salir con un modelo grande y se revisa completo. Como alternativa, el propio reloj puede generarlo mientras se carga, con menor calidad y la misma revisión.
- Las preguntas que están en el banco se responden sin encender la IA, lo que ahorra batería.
