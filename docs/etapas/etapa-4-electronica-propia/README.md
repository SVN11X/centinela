# Etapa 4. Electrónica propia

| Estado | Hito en GitHub | Versión al cerrar |
|---|---|---|
| Pendiente | Etapa 4 | v0.5.0 |

## Objetivo

Diseñar, fabricar y probar la placa principal que reemplaza al CoreS3 dentro del reloj. El módulo de IA sigue siendo el Module LLM, conectado a esta placa.

## Entregables

| Entregable | Dónde queda |
|---|---|
| Esquemático y diseño de la placa | [hardware/placa-principal](../../../hardware/placa-principal/) |
| Lista de materiales con precios | [hardware/bom](../../../hardware/bom/) |
| Informes de puesta en marcha | [pruebas/resultados](../../../pruebas/resultados/) |

## Tareas

- [ ] Calcular el presupuesto de energía de cada bloque
- [ ] Dibujar el esquemático con los bloques de [placa-principal](../../../hardware/placa-principal/)
- [ ] Revisar el esquemático con una lista de verificación
- [ ] Diseñar la placa y las antenas
- [ ] Fabricar y armar 3 placas
- [ ] Probar cada bloque por separado
- [ ] Medir el consumo en reposo y compararlo con el cálculo
- [ ] Completar la lista de materiales con proveedores y precios

## Criterios de cierre

| Criterio | Cómo se comprueba |
|---|---|
| Cada bloque pasa su prueba | Informes de puesta en marcha |
| El consumo en reposo no supera el cálculo en más de 20 % (meta propuesta) | Informe de consumo |
| La lista de materiales está completa | Carpeta hardware/bom |

## Riesgos principales

R-06, R-08 y R-11 en [riesgos.md](../../riesgos.md).

## Evidencias

Fotos, mediciones y registros en `pruebas/resultados/`.
