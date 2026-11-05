# Protocolos de prueba

Cada protocolo se escribe en su propio archivo, por ejemplo `p-01-arranque.md`, con objetivo, equipo, preparación, pasos, número de repeticiones y forma de registrar los datos.

| ID | Qué mide | Requisito | Etapa |
|---|---|---|---|
| P-01 | Tiempo desde que se enciende el módulo de IA hasta la primera respuesta | RNF-06 | 1 |
| P-02 | Consumo apagado, en reposo y respondiendo | RNF-02 y RNF-03 | 1 |
| P-03 | Temperatura de la cara de la piel durante 10 preguntas seguidas | RNF-01 | 1 y 5 |
| P-04 | Respuestas correctas en el set de 50 preguntas | RNF-05 y RNF-11 | 1 |
| P-05 | Voz en español: activación, reconocimiento y respuesta hablada | RF-04 | 1 |
| P-06 | Funcionamiento a 0 °C y a 40 °C | RNF-10 | 1 y 6 |
| P-07 | Duración real de la batería en salidas de 1 a 3 días | RNF-02 y RNF-03 | 6 |
| P-08 | Protección contra agua y polvo | RNF-09 | 5 |
| P-09 | Señal de GPS y LoRa dentro de la caja | RF-05 y RF-08 | 5 |

El set de 50 preguntas de prueba, con su respuesta esperada, se guarda en esta carpeta como `set-de-preguntas.md`.

Las metas de cada prueba están en [requisitos.md](../../docs/requisitos.md).
