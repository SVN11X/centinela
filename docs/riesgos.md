# Registro de riesgos

Evaluación inicial. Se revisa al cerrar cada etapa.

| ID | Riesgo | Impacto | Probabilidad | Respuesta | Dueño | Estado |
|---|---|---|---|---|---|---|
| R-01 | El módulo de IA tarda demasiado en arrancar y cargar el modelo | Alto | Media | Medir en la etapa 1. Si tarda más de 60 s, dejarlo en reposo durante las salidas | Por asignar | Abierto |
| R-02 | La cara de la piel supera 39 °C | Alto | Media | Aluminio unido al aro, aislante y corte automático por temperatura | Por asignar | Abierto |
| R-03 | Los modelos chicos responden mal en español | Alto | Media | Respuestas en tres niveles, banco revisado y set de 50 preguntas | Por asignar | Abierto |
| R-04 | No hay voz en español de buena calidad para el módulo | Medio | Media | Probar en la etapa 1. La pantalla queda como respaldo | Por asignar | Abierto |
| R-05 | Una respuesta equivocada causa daño en una emergencia | Alto | Media | Procedimientos críticos solo desde contenido revisado por un profesional de salud. Avisos claros en el manual | Por asignar | Abierto |
| R-06 | El Module LLM deja de fabricarse o sube mucho de precio | Medio | Media | Conector en la placa principal que permita cambiar el módulo de IA | Por asignar | Abierto |
| R-07 | El módulo de IA solo está especificado de 0 a 40 °C | Medio | Alta | Pruebas en frío y calor. Límites claros en el manual | Por asignar | Abierto |
| R-08 | La caja de metal bloquea las antenas | Medio | Media | Ventana de plástico en el aro y prueba P-09 | Por asignar | Abierto |
| R-09 | Una fuente de contenido o un modelo tiene una licencia incompatible | Medio | Baja | Registrar cada fuente antes de usarla | Por asignar | Abierto |
| R-10 | No hay SOS satelital en Chile | Medio | Confirmado | Decisión 0004 y aviso en el manual | Por asignar | Aceptado |
| R-11 | Fabricar placas propias cuesta más tiempo o dinero de lo previsto | Medio | Media | Fabricar pocas unidades y revisar el esquemático antes de pedirlas | Por asignar | Abierto |
| R-12 | La batería no alcanza 2 días con uso moderado | Alto | Media | Medir en la etapa 1, reducir encendidos del módulo o subir la capacidad si cabe | Por asignar | Abierto |

## Cómo usar este registro

Cuando aparece un riesgo nuevo se agrega una fila y se abre un issue con la etiqueta riesgo. Un riesgo se cierra cuando ya no puede ocurrir o cuando su respuesta está probada.
