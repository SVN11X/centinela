# Hardware

Electrónica del reloj. La carpeta está casi vacía a propósito: la placa propia se diseña en la [etapa 4](../docs/etapas/etapa-4-electronica-propia/), después de medir el prototipo de la etapa 1.

| Carpeta o archivo | Contenido | Etapa |
|---|---|---|
| [placa-principal](placa-principal/) | Proyecto de KiCad de la placa con ESP32-S3, GPS, LoRa, energía y sensores | 4 |
| [bom](bom/) | Lista de materiales con proveedor, código y precio | 4 |
| [hojas-de-datos.md](hojas-de-datos.md) | Enlaces a las hojas de datos de cada componente | 0 a 4 |

## Reglas

- Se usa KiCad y se anota la versión en el README de la placa.
- Las hojas de datos en PDF no se suben, porque tienen derechos de autor. Se guarda solo el enlace.
- Los archivos de fabricación no se guardan en git. Se publican en Releases con cada versión.
- Licencia: CERN-OHL-S-2.0.
