# Programa del reloj

Corre en el ESP32-S3, la parte siempre encendida. Todavía no hay código, se escribe en la etapa 3.

## Funciones previstas

- [ ] Pantalla táctil y menús
- [ ] Hora, alarmas y vibración
- [ ] GPS, brújula y altitud
- [ ] Pantalla de emergencia con coordenadas, linterna y alarma sonora
- [ ] Respuestas preparadas (nivel 1) y búsqueda en guías (nivel 2)
- [ ] Encendido, apagado ordenado y corte de energía del módulo de IA
- [ ] Lectura de la temperatura de la piel y corte de la IA al llegar al límite
- [ ] Mensajes LoRa compatibles con Meshtastic
- [ ] Registro de eventos

## Preguntas abiertas

- Cómo integrar Meshtastic: dentro del mismo programa o con su firmware en un chip de radio aparte.
- Qué entorno de desarrollo usar, ESP-IDF o Arduino. Se registra como decisión.
