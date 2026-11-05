# Arquitectura

Resumen de cómo se organiza el reloj por dentro. Las cifras vienen de las fuentes en [referencias.md](referencias.md) y se confirman con las mediciones de la etapa 1.

## Dos partes en una sola caja

El reloj tiene dos partes que trabajan juntas dentro de la misma caja.

La parte siempre encendida usa un microcontrolador ESP32-S3. Maneja la pantalla, la hora, los sensores, el GPS, LoRa, las respuestas preparadas, la búsqueda en guías y el control de energía y temperatura. Gasta poco y no se apaga.

El módulo de IA usa el chip AX630C del M5Stack Module LLM. Se enciende solo cuando hace falta una respuesta con IA, la voz, Wikipedia o el cálculo de una ruta, y después se apaga por completo. Según el fabricante, consume 0,5 W en reposo y 1,5 W a plena carga.

Las dos partes se comunican por un puerto serie (UART).

## Cómo responde

| Nivel | Qué hace | Lo resuelve | Tiempo esperado |
|---|---|---|---|
| 1. Respuesta preparada | Busca en un banco de preguntas y respuestas revisadas | ESP32-S3 | Al instante |
| 2. Fragmento de guía | Muestra el párrafo de guía más parecido, con su fuente | ESP32-S3 | Pocos segundos |
| 3. Respuesta con IA | El modelo responde apoyado en 1 o 2 fragmentos de guía | Módulo de IA | 10 a 25 s, más el arranque |

Los procedimientos críticos salen siempre del nivel 1 ([decisión 0003](decisiones/0003-respuestas-en-tres-niveles.md)).

## Capas, de arriba hacia abajo

| Capa | Función | Grosor estimado |
|---|---|---|
| Cristal y pantalla AMOLED táctil | Mostrar y tocar | 3 mm |
| Placa principal | ESP32-S3, GPS, LoRa, sensores y energía | 3 mm |
| Placa de aluminio unida al aro | Llevar el calor hacia los lados | 1,5 mm |
| Módulo de IA | AX630C, memoria y almacenamiento | 8 mm |
| Aislante térmico | Proteger del calor a la batería y a la piel | 1,5 mm |
| Batería | Unos 1.500 mAh | 6 mm |
| Tapa plástica | Sensor de temperatura de la piel y sensor de pulso | 2 mm |

El calor del módulo sube a la placa de aluminio y sale por el aro, no hacia la piel ni hacia la batería. Las antenas de GPS y LoRa necesitan una ventana de plástico en el aro, porque el metal las bloquea. Tamaño total estimado: 60 × 60 × 26 mm.

## Energía

| Dato | Valor estimado |
|---|---|
| Batería | Unos 1.500 mAh, cerca de 5,8 Wh |
| Parte siempre encendida | Del orden de 1 Wh al día |
| Una respuesta con IA, con unos 20 s de arranque | Cerca de 50 J |
| Duración con uso moderado | 2 a 3 días |
| Duración con uso intenso | Cerca de 1 día |
| Conversando sin parar con la IA | 3 a 4 horas |

El módulo de IA recibe 5 V desde un conversor y se corta con un interruptor electrónico que controla el ESP32-S3. Antes de cortar la energía, el módulo se apaga en orden para no dañar sus archivos.

## Límites conocidos

- El techo práctico de la IA son modelos de 1,5 a 2B parámetros. Uno de 7B no cabe en la memoria que el módulo reserva para la IA, que son 3 de sus 4 GB.
- El módulo está especificado para funcionar entre 0 y 40 °C.
- La versión 1.0 no tiene SOS satelital en Chile ([decisión 0004](decisiones/0004-sos-satelital-fuera-de-la-version-1-0.md)).

## Plan B

Si la etapa 1 muestra que el AX630C no alcanza, se evalúa la Radxa Cubie A7Z con chip A733, usada en ráfagas cortas, con más calor y menos batería ([decisión 0002](decisiones/0002-modulo-de-ia-ax630c.md)).
