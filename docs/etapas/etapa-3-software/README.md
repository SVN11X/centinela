# Etapa 3. Software

| Estado | Hito en GitHub | Versión al cerrar |
|---|---|---|
| Pendiente | Etapa 3 | v0.4.0 |

## Objetivo

Convertir el prototipo de la etapa 1 en un reloj completo, con todas las funciones de la versión 1.0. Es la primera etapa que agrega código al repositorio.

Mientras no exista la placa propia, el GPS y LoRa se prueban en un LILYGO T-Watch S3 Plus o Ultra, usado solo como banco de pruebas. Ese equipo no forma parte del reloj.

## Entregables

| Entregable | Dónde queda |
|---|---|
| Documento de interfaz entre el reloj y el módulo de IA | [software](../../../software/) |
| Programa del reloj | [software/reloj](../../../software/reloj/) |
| Programa del módulo de IA | [software/modulo-ia](../../../software/modulo-ia/) |
| Resultados de las pruebas de cada función | [pruebas/resultados](../../../pruebas/resultados/) |

## Tareas

- [ ] Definir los mensajes entre el reloj y el módulo de IA
- [ ] Hora, alarmas, brújula, altitud y posición GPS
- [ ] Pantalla de emergencia con coordenadas, linterna y alarma sonora
- [ ] Respuestas en tres niveles ([decisión 0003](../../decisiones/0003-respuestas-en-tres-niveles.md))
- [ ] Encendido y apagado automático del módulo de IA, con apagado ordenado
- [ ] Corte de la IA cuando la piel llega al límite de temperatura
- [ ] Voz con activación, pregunta y respuesta
- [ ] Mapas y rutas sin conexión
- [ ] Wikipedia sin conexión
- [ ] Mensajes LoRa compatibles con Meshtastic
- [ ] Registro de eventos para encontrar fallas
- [ ] Probar cada función y guardar su resultado

## Criterios de cierre

| Criterio | Cómo se comprueba |
|---|---|
| RF-02 a RF-10 funcionan en el prototipo | Informes de prueba |
| El corte por temperatura funciona | Informe de la prueba P-03 |
| No hay fallas críticas abiertas | Issues con la etiqueta falla |

## Riesgos principales

R-01, R-03 y R-04 en [riesgos.md](../../riesgos.md).

## Evidencias

Informes en `pruebas/resultados/` y pull requests enlazados a cada tarea.
