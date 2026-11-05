# Modelos de IA

Aquí se registra qué modelos usa el reloj, de dónde salen y con qué licencia. Los archivos de los modelos no se guardan en git porque pesan cientos de megabytes.

## Modelos candidatos

| Uso | Modelo | Velocidad informada por M5Stack en el AX630C |
|---|---|---|
| Respuestas rápidas | Qwen3-0.6B | 10,28 tokens/s, primera palabra en 0,36 s |
| Respuestas de calidad | Qwen2.5-1.5B (INT4) | 4,63 tokens/s, primera palabra en 1,2 s |
| Visión | InternVL3-1B | 9,78 tokens/s, 2,3 s por imagen |
| Reconocimiento de voz | Whisper tiny o base | Por medir |
| Voz sintética | MeloTTS | Por medir |

Las velocidades se confirman en la etapa 1, con la prueba P-04. Las fuentes están en [referencias.md](../docs/referencias.md).

## Reglas

- Los modelos para el AX630C usan un formato propio. Se instalan desde el repositorio de M5Stack o se convierten con Pulsar2, la herramienta de Axera.
- Por cada modelo usado se anota el nombre exacto, la versión, la fecha, el origen, la licencia y la conversión aplicada.
- La licencia de cada modelo se registra en [licencias-de-terceros.md](../docs/licencias-de-terceros.md) antes de usarlo.

## Registro de modelos instalados

| Fecha | Modelo | Versión | Origen | Conversión | Licencia |
|---|---|---|---|---|---|
| | | | | | |
