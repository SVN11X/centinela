# 0002. Módulo de IA con chip AX630C

| Estado | Fecha | Etapa |
|---|---|---|
| Propuesta, se acepta al cerrar la etapa 1 | 2026-11-05 | 0 |

## Contexto

La primera versión del diseño usaba la Radxa Cubie A7Z, con chip Allwinner A733. Las mediciones publicadas muestran que esa placa consume 2,2 W en reposo sin pantalla y 5,4 W con el procesador al máximo, y otro usuario midió cerca de 8 W con carga. Una simulación de un equipo usado sobre el cuerpo encontró que solo puede soltar unos 1,75 W de calor en forma continua sin pasar los 43 °C. La A733 supera varias veces ese margen.

## Opciones consideradas

| Opción | A favor | En contra |
|---|---|---|
| Cubie A7Z (A733) | Más rápida con modelos chicos en el procesador. Contexto largo | De 5 a 8 W con carga. Según la comunidad, su acelerador de IA no ayuda con modelos de lenguaje. Placa de 65 × 30 mm |
| M5Stack Module LLM (AX630C) | 0,5 W en reposo y 1,5 W a plena carga. Trae micrófono, parlante y voz sin conexión. Mide 54 × 54 × 13 mm, pesa 17,4 g y cuesta unos US$50 | Modelos chicos, y lentos con 1,5B. Contexto corto. Formato de modelo propio. Especificado de 0 a 40 °C |
| Tarjeta AX8850 | Unas tres veces más rápida que el AX630C con un modelo de 1,5B | Es una tarjeta M.2 que necesita otro computador. Hoy no cabe en un reloj |

## Decisión

Usar el M5Stack Module LLM, con chip AX630C, como módulo de IA del reloj.

## Consecuencias

- El reloj usa modelos de 0,6B a 1,5B. El techo práctico es de 1,5 a 2B.
- Las respuestas se apoyan en el sistema de tres niveles ([decisión 0003](0003-respuestas-en-tres-niveles.md)) para compensar la calidad de los modelos chicos.
- Hay que convertir los modelos al formato de Axera o usar los que publica M5Stack.
- La etapa 1 debe medir arranque, calor, consumo y calidad antes de aceptar esta decisión.
- El módulo va conectado a la placa principal, de modo que se pueda cambiar por uno más rápido cuando exista en tamaño reloj.

## Plan B

Si la etapa 1 muestra que el AX630C no alcanza, se evalúa la Cubie A7Z usada en ráfagas cortas, con más calor y menos batería.

## Evidencia

Fuentes en [referencias.md](../referencias.md), secciones Módulo de IA, Plan B y Temperatura y seguridad.
