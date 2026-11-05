# Requisitos

Las metas son una propuesta inicial basada en el análisis de viabilidad ([arquitectura](arquitectura.md) y [referencias](referencias.md)). Cambiar una meta requiere registrar una decisión.

## Requisitos funcionales

| ID | Requisito | Se verifica en |
|---|---|---|
| RF-01 | Todas las funciones operan sin internet y sin otro aparato durante el uso | Etapa 6 |
| RF-02 | Responde preguntas en español en tres niveles: respuesta preparada, fragmento de guía y respuesta con IA | Etapa 3 |
| RF-03 | Los procedimientos críticos salen siempre de contenido revisado y nunca los genera la IA | Etapa 3 |
| RF-04 | Recibe preguntas por voz y responde con voz y en pantalla | Etapas 1 y 3 |
| RF-05 | Muestra hora, posición GPS, brújula y altitud | Etapa 3 |
| RF-06 | Muestra mapas y calcula rutas de Chile sin conexión | Etapa 3 |
| RF-07 | Abre artículos de Wikipedia en español sin conexión | Etapa 3 |
| RF-08 | Envía y recibe mensajes LoRa con otros equipos Meshtastic | Etapa 3 |
| RF-09 | Tiene una pantalla de emergencia con coordenadas, linterna y alarma sonora | Etapa 3 |
| RF-10 | Apaga por completo el módulo de IA cuando no se usa y lo detiene si la piel llega al límite de temperatura | Etapa 3 |
| RF-11 | Mide pulso y oxígeno en la sangre (deseable) | Etapa 4 |
| RF-12 | Describe imágenes con una cámara (deseable, después de la versión 1.0) | Por definir |

## Requisitos no funcionales

| ID | Requisito | Meta | Mínimo aceptable | Se verifica en |
|---|---|---|---|---|
| RNF-01 | Temperatura de la cara que toca la piel | 39 °C o menos | Límite fijo | Etapas 1 y 5 |
| RNF-02 | Duración de batería con uso moderado | 3 días | 2 días | Etapas 1 y 6 |
| RNF-03 | Duración de batería con uso intenso | 1 día | Por definir después de la etapa 1 | Etapa 6 |
| RNF-04 | Tiempo de una respuesta preparada | Menos de 1 s | 2 s | Etapa 3 |
| RNF-05 | Tiempo de una respuesta con IA, sin contar el arranque | 15 s | 25 s | Etapa 1 |
| RNF-06 | Arranque del módulo de IA hasta poder responder | 30 s | 60 s, con modo reposo | Etapa 1 |
| RNF-07 | Tamaño | 60 × 60 × 26 mm | Por definir | Etapa 5 |
| RNF-08 | Peso | Por definir | Por definir | Etapa 5 |
| RNF-09 | Protección contra agua y polvo | IP67 | IP65 | Etapa 5 |
| RNF-10 | Temperatura ambiente de uso | 0 a 40 °C | 0 a 40 °C | Etapas 1 y 6 |
| RNF-11 | Respuestas correctas en el set de 50 preguntas de prueba | 90 % | 80 % | Etapa 1 |
| RNF-12 | Idioma de la pantalla y la voz | Español de Chile | Español | Etapa 3 |

El rango de RNF-10 es el que especifica el fabricante del módulo de IA. Ampliarlo requiere pruebas y una decisión.
