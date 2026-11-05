# Visión y alcance

> Borrador para revisar en la etapa 0.

## Problema

En una emergencia lejos de la ciudad, el teléfono puede estar sin batería, sin señal o guardado en la mochila. Una guía impresa no responde preguntas ni indica dónde está el refugio más cercano.

## Propuesta

Un reloj grande y resistente que reúne en la muñeca lo necesario para orientarse y actuar en una emergencia, con un asistente de IA que funciona sin internet y sin otro aparato.

## Para quién

Por definir en la etapa 0. Grupos a evaluar: personas que hacen trekking o montañismo, y quienes trabajan en zonas sin cobertura.

## Qué hace la versión 1.0

| Función | Detalle |
|---|---|
| Asistente | Responde por voz y en pantalla, en tres niveles |
| Emergencia | Procedimientos críticos revisados, coordenadas, linterna y alarma sonora |
| Orientación | GPS, brújula, altitud, mapas y rutas de Chile sin conexión |
| Conocimiento | Wikipedia en español sin conexión |
| Comunicación | Mensajes LoRa con otros equipos Meshtastic cercanos |

## Qué no hace

| Límite | Motivo |
|---|---|
| No reemplaza la atención médica ni los servicios de emergencia | Es una ayuda, no un profesional |
| No envía SOS satelital en Chile | Hoy no hay cobertura ([decisión 0004](decisiones/0004-sos-satelital-fuera-de-la-version-1-0.md)) |
| No usa modelos de IA de 7B o más | No caben en el consumo ni en la memoria del módulo |

## Cómo se sabe que está listo

Cuando cumple todos los [requisitos](requisitos.md) y se cierra la etapa 7.
