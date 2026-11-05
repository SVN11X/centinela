# Etapa 5. Mecánica y térmica

| Estado | Hito en GitHub | Versión al cerrar |
|---|---|---|
| Pendiente | Etapa 5 | v0.6.0 |

## Objetivo

Diseñar y probar una caja de unos 60 × 60 × 26 mm que proteja el reloj, saque el calor hacia los lados y deje pasar la señal de las antenas.

## Entregables

| Entregable | Dónde queda |
|---|---|
| Modelo 3D de la caja | [mecanica/caja](../../../mecanica/caja/) |
| Correa y anclajes | [mecanica/correa](../../../mecanica/correa/) |
| Informes de pruebas térmicas, de agua y de caída | [pruebas/resultados](../../../pruebas/resultados/) |

## Tareas

- [ ] Modelar la caja con las capas de la [arquitectura](../../arquitectura.md)
- [ ] Diseñar el aro de aluminio unido a la placa interna que lleva el calor
- [ ] Diseñar la ventana de plástico para las antenas
- [ ] Fabricar prototipos de la caja
- [ ] P-03. Repetir la prueba de temperatura de la piel dentro de la caja
- [ ] P-08. Probar la protección contra agua y polvo
- [ ] P-09. Medir la señal de GPS y LoRa dentro de la caja
- [ ] Probar caídas desde la altura de la muñeca
- [ ] Ajustar la correa para uso prolongado

## Criterios de cierre

| Criterio | Meta | Requisito |
|---|---|---|
| Temperatura de la cara de la piel | 39 °C o menos | RNF-01 |
| Agua y polvo | IP65 como mínimo | RNF-09 |
| Tamaño | 60 × 60 × 26 mm o menos | RNF-07 |
| Señal de GPS y LoRa | Aceptada en la revisión de cierre | RF-05 y RF-08 |

## Riesgos principales

R-02 y R-08 en [riesgos.md](../../riesgos.md).

## Evidencias

Informes en `pruebas/resultados/` y archivos 3D en `mecanica/`.
