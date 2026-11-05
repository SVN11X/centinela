# 0005. Licencias del proyecto

| Estado | Fecha | Etapa |
|---|---|---|
| Propuesta | 2026-11-05 | 0 |

## Contexto

El repositorio mezcla software, hardware, mecánica y documentación. El proyecto toma como referencia Nomad Pocket, que usa la licencia GPL-3.0-or-later. Si se copia código de Nomad Pocket, el software del reloj debe usar una licencia compatible.

## Opciones consideradas

| Opción | A favor | En contra |
|---|---|---|
| Licencias abiertas que exigen compartir cambios | Compatibles con Nomad Pocket. Las mejoras de otros vuelven al proyecto | Nadie puede cerrar una versión derivada |
| Licencias permisivas | Más libertad para usos comerciales cerrados | No permiten copiar código GPL de Nomad Pocket |

## Decisión

| Parte | Licencia | Qué permite |
|---|---|---|
| Software | GPL-3.0-or-later | Usar, modificar y vender, compartiendo el código de los cambios con la misma licencia |
| Hardware y mecánica | CERN-OHL-S-2.0 | Lo mismo para esquemáticos, placas y piezas |
| Documentación | CC BY-SA 4.0 | Copiar y adaptar, citando la fuente y con la misma licencia |
| Contenido de terceros | La de cada fuente | Se registra en [licencias-de-terceros.md](../licencias-de-terceros.md) |

## Consecuencias

- Cualquiera puede fabricar y vender el reloj, siempre que comparta sus cambios.
- Si en el futuro se quiere un producto cerrado, hay que decidirlo antes de incorporar código GPL de terceros.
- Esta decisión no reemplaza una revisión legal antes de vender el producto.
