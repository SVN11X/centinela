# 0004. SOS satelital fuera de la versión 1.0

| Estado | Fecha | Etapa |
|---|---|---|
| Aceptada | 2026-11-05 | 0 |

## Contexto

El SOS satelital en un reloj ya existe: el Garmin fēnix 8 Pro envía SOS por satélite sin teléfono, usando la red de Skylo. Esa red cubre Norteamérica, Europa, Brasil y partes de Asia y Oceanía, y Chile no aparece en esa cobertura. Para proyectos propios existe el módulo nRF9151 de Nordic, que combina red celular y satélite del mismo tipo.

## Opciones consideradas

| Opción | A favor | En contra |
|---|---|---|
| Incluir SOS satelital con el nRF9151 | Aviso real a servicios de rescate | Sin cobertura en Chile hoy. Exige plan de datos y certificación |
| Solo LoRa con Meshtastic | Sin costo mensual. Funciona entre equipos cercanos | No llega a servicios de rescate |

## Decisión

La versión 1.0 no incluye SOS satelital. La comunicación queda en LoRa con Meshtastic, que solo llega a otros equipos cercanos.

## Consecuencias

- El manual debe decir con claridad que el reloj no avisa a servicios de rescate.
- Esta decisión se revisa cuando exista cobertura satelital en Chile para módulos como el nRF9151.
- La placa principal deja espacio reservado para ese módulo.

## Evidencia

Fuentes en [referencias.md](../referencias.md), sección Comunicación satelital.
