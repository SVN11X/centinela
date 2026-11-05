# 0001. Reloj todo en uno, sin dispositivos externos

| Estado | Fecha | Etapa |
|---|---|---|
| Aceptada | 2026-11-05 | 0 |

## Contexto

El reloj debe funcionar solo. Una primera idea separaba el cálculo de IA en un módulo de bolsillo o de antebrazo, para manejar mejor el calor y la batería.

## Opciones consideradas

| Opción | A favor | En contra |
|---|---|---|
| Dos piezas: reloj y módulo aparte | Más potencia de IA y más batería | Depende de otro aparato. El enlace entre ambos puede fallar |
| Todo en uno | Una sola pieza en la muñeca | La IA queda limitada por el calor y la batería que caben en un reloj |

## Decisión

Todas las funciones van dentro del reloj. Mientras se usa, no depende de un teléfono, de un módulo de bolsillo, de internet ni de ningún otro aparato.

Preparar el contenido antes de salir sí está permitido, igual que se cargan mapas en un GPS. Esto incluye mapas, Wikipedia, modelos y el banco de respuestas.

## Consecuencias

- El módulo de IA debe consumir poco ([decisión 0002](0002-modulo-de-ia-ax630c.md)).
- El tamaño estimado del reloj es de unos 60 × 60 × 26 mm.
- Las funciones que no caben en ese consumo quedan fuera de la versión 1.0.
