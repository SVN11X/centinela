# Hoja de ruta

El trabajo se ordena en ocho etapas, desde la definición hasta la versión 1.0. Cada etapa se cierra con una revisión que compara lo logrado con sus criterios de cierre, usando la [plantilla de revisión](docs/plantillas/revision-de-cierre-de-etapa.md).

## Resumen

| Etapa | Objetivo | Se cierra cuando | Depende de |
|---|---|---|---|
| 0. Definición | Dejar por escrito qué se construye y con qué límites | Requisitos, riesgos y decisiones están revisados | Nada |
| 1. Prototipo de medición | Medir arranque, calor, consumo y calidad en español | Las mediciones cumplen las metas o se elige el plan B | Etapa 0 |
| 2. Contenido sin conexión | Preparar todo lo que el reloj sabe | Los procedimientos críticos están revisados por un profesional de salud | Etapa 0 |
| 3. Software | Convertir el prototipo en un reloj completo | Todas las funciones pasan sus pruebas en el prototipo | Etapas 1 y 2 |
| 4. Electrónica propia | Reemplazar el prototipo por una placa propia | La placa pasa sus pruebas eléctricas | Etapa 1 |
| 5. Mecánica y térmica | Hacer una caja que proteja y saque el calor hacia los lados | La piel no pasa de 39 °C y la caja cumple IP65 | Etapa 4 |
| 6. Integración y pruebas en terreno | Probar el reloj completo fuera del laboratorio | Cumple los requisitos sin fallas críticas abiertas | Etapas 3, 4 y 5 |
| 7. Versión 1.0 | Dejar el producto listo para usar y fabricar | La versión 1.0.0 está publicada con su documentación | Etapa 6 |

El detalle de cada etapa está en [docs/etapas](docs/etapas/).

## Etapas en paralelo

La etapa 2 puede avanzar junto con la 1, porque escribir y revisar contenido no depende del hardware. La etapa 4 puede empezar cuando la etapa 1 confirme el módulo de IA, aunque el software de la etapa 3 siga en curso.

## Cómo se sigue el avance en GitHub

Cada etapa es un hito (milestone) llamado Etapa N. Cada tarea es un issue asignado a su hito, creado con la plantilla Tarea de etapa. La barra de avance del hito muestra cuánto falta. Un tablero de GitHub Projects con las columnas Pendiente, En curso, En revisión y Hecho permite ver todo junto.

## Versiones

Al cerrar cada etapa se publica una versión en Releases. La etapa 0 publica la v0.1.0, la etapa 1 la v0.2.0, y así hasta la etapa 7, que publica la v1.0.0.
