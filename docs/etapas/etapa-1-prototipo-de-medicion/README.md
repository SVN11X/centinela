# Etapa 1. Prototipo de medición

| Estado | Hito en GitHub | Versión al cerrar |
|---|---|---|
| Pendiente | Etapa 1 | v0.2.0 |

## Objetivo

Medir con hardware real los datos que deciden si el diseño funciona en la muñeca: arranque del módulo de IA, calor, consumo y calidad de las respuestas en español.

## Hardware

El prototipo es un M5Stack CoreS3 con un M5Stack Module LLM apilado. Juntos miden unos 54 × 54 × 29 mm y, con una correa ancha, ya forman un reloj todo en uno.

| Componente | Uso | Precio de referencia |
|---|---|---|
| M5Stack CoreS3 | Parte siempre encendida, pantalla y batería | US$59,90 en la tienda oficial |
| M5Stack Module LLM | Módulo de IA con chip AX630C | US$49,90 en la tienda oficial |
| Medidor de consumo USB | Medir energía | Por cotizar |
| Termómetro de contacto o termocupla | Medir la temperatura de la piel | Por cotizar |
| Correa ancha | Usar el prototipo en la muñeca | Por cotizar |

Los precios no incluyen envío ni impuestos de importación.

## Entregables

| Entregable | Dónde queda |
|---|---|
| Protocolos P-01 a P-06 | [pruebas/protocolos](../../../pruebas/protocolos/) |
| Informes de cada medición | [pruebas/resultados](../../../pruebas/resultados/) |
| Set de 50 preguntas de prueba | [pruebas/protocolos](../../../pruebas/protocolos/) |
| Decisión 0002 aceptada o plan B registrado | [decisiones](../../decisiones/) |

## Tareas

- [ ] Comprar el hardware de la tabla
- [ ] Escribir los protocolos P-01 a P-06
- [ ] Armar un set de 50 preguntas de prueba con su respuesta esperada
- [ ] P-01. Medir el tiempo desde que se enciende el módulo de IA hasta la primera respuesta
- [ ] P-02. Medir el consumo apagado, en reposo y respondiendo
- [ ] P-03. Medir la temperatura de la cara de la piel durante 10 preguntas seguidas
- [ ] P-04. Evaluar el set de 50 preguntas con un modelo de 0,6B y con uno de 1,5B
- [ ] P-05. Probar en español la activación por voz, el reconocimiento y la respuesta hablada
- [ ] P-06. Probar el funcionamiento a 0 °C y a 40 °C, los extremos que indica el fabricante del módulo
- [ ] Calcular la duración de la batería con los consumos medidos
- [ ] Registrar si se acepta la decisión 0002 o se pasa al plan B

## Criterios de cierre

| Criterio | Meta | Mínimo aceptable | Requisito |
|---|---|---|---|
| Temperatura de la cara de la piel en uso normal | 39 °C o menos | Límite fijo | RNF-01 |
| Arranque del módulo hasta la primera respuesta | 30 s | 60 s, con modo reposo | RNF-06 |
| Respuesta con IA, sin contar el arranque | 15 s | 25 s | RNF-05 |
| Duración calculada con uso moderado | 3 días | 2 días | RNF-02 |
| Respuestas correctas en el set de 50 preguntas | 90 % | 80 % | RNF-11 |

Si algún criterio no se cumple, la revisión de cierre decide entre repetir la medición, ajustar el diseño o pasar al plan B de la [decisión 0002](../../decisiones/0002-modulo-de-ia-ax630c.md).

## Riesgos principales

R-01, R-02, R-03, R-04, R-07 y R-12 en [riesgos.md](../../riesgos.md).

## Evidencias

Cada medición se guarda en `pruebas/resultados/AAAA-MM-DD-tema/` con la [plantilla de informe](../../plantillas/informe-de-medicion.md).
