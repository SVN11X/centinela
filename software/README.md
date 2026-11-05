# Software

Todavía no hay código. El software se escribe en la [etapa 3](../docs/etapas/etapa-3-software/), después de medir el prototipo.

| Carpeta | Corre en | Responsabilidad |
|---|---|---|
| [reloj](reloj/) | ESP32-S3 | Pantalla, hora, sensores, GPS, LoRa, respuestas preparadas, búsqueda en guías, energía y temperatura |
| [modulo-ia](modulo-ia/) | AX630C | Modelo de lenguaje, voz, Wikipedia y rutas |

Las dos partes se comunican por UART. El formato de los mensajes se define en la etapa 3, en un documento de interfaz que se guarda en esta carpeta.

Licencia: GPL-3.0-or-later.
