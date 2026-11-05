# Referencias

Fuentes usadas en el análisis de viabilidad. Las cifras de los documentos del proyecto salen de aquí y se confirman con mediciones propias.

## Base del proyecto

| Fuente | Para qué se usó |
|---|---|
| [Nomad Pocket](https://github.com/franlindebl/nomad-pocket) | Aplicación de referencia, motores que usa y licencia |
| [Paquetes de Nomad Pocket](https://github.com/franlindebl/nomad-pocket/releases) | Rutas y datos de Sudamérica para uso sin conexión |

## Módulo de IA

| Fuente | Para qué se usó |
|---|---|
| [Anuncio del Module LLM en CNX Software](https://www.cnx-software.com/2024/11/05/m5stack-releases-ax630c-powered-offline-module-llm-for-local-smart-home-and-ai-applications/) | Consumo, tamaño, peso, memoria y temperatura de operación |
| [Qwen3-0.6B en el Module LLM](https://docs.m5stack.com/en/stackflow/models/qwen3-0.6b) | Velocidad del modelo rápido |
| [Qwen2.5-0.5B en el Module LLM](https://docs.m5stack.com/en/stackflow/models/qwen2.5-0.5b-instruct) | Velocidad y largo de contexto |
| [Qwen2.5-1.5B en el Module LLM](https://docs.m5stack.com/en/stackflow/models/qwen2.5-1.5b-instruct) | Velocidad del modelo de calidad |
| [InternVL3-1B en el Module LLM (en chino)](https://docs.m5stack.com/zh_CN/stackflow/models/internvl3-1b) | Velocidad del modelo de visión |
| [MaixCAM2 en CNX Software](https://www.cnx-software.com/2026/01/27/maixcam2-modular-4k-ai-camera-is-based-on-axera-ax630-soc-with-3-2-tops-npu/) | Consumo del mismo chip con un modelo de visión |
| [Tarjeta AX8850 en la documentación de M5Stack (en chino)](https://docs.m5stack.com/zh_CN/guide/ai_accelerator/llm-8850/m5_llm_8850_qwen3_0.6b) | Velocidad del siguiente salto de chip y tiempo de carga de modelos |

## Prototipo y referencias de diseño

| Fuente | Para qué se usó |
|---|---|
| [M5Stack CoreS3](https://docs.m5stack.com/en/core/CoreS3) | Prototipo de la etapa 1 |
| [LILYGO T-Watch S3 Plus](https://wiki.lilygo.cc/get_started/en/Wearable/T-Watch-S3-PLUS/T-Watch-S3-PLUS.html) | Referencia de diseño y esquemático |
| [LILYGO T-Watch Ultra en CNX Software](https://www.cnx-software.com/2026/04/20/lilygo-t-watch-ultra-an-ip65-rated-esp32-s3-smartwatch-with-2-01-inch-amoled-lora-and-gnss/) | Referencia de tamaño y protección IP65 |

## Plan B

| Fuente | Para qué se usó |
|---|---|
| [Radxa Cubie A7Z](https://docs.radxa.com/en/cubie/a7z/hardware-use/hardware-info) | Características de la placa |
| [Consumo de la Cubie A7Z en LinuxLinks](https://www.linuxlinks.com/radxa-cubie-a7z-single-board-computer-running-linux-power-consumption/2/) | Consumo en reposo y con carga |
| [Mediciones de la comunidad sobre el A733](https://github.com/lilyco-42/awesome-radxa-a733) | Velocidad de modelos en el procesador y límites de su acelerador de IA |

## Temperatura y seguridad

| Fuente | Para qué se usó |
|---|---|
| [Límites de temperatura de contacto según IEC 62368-1](https://www.electronics-cooling.com/?p=36855) | Límites para equipos que tocan la piel |
| [Umbral de molestia por temperatura](https://www.electronics-cooling.com/?p=35375) | Meta de 39 °C en la piel |
| [Simulación térmica de un equipo usado sobre el cuerpo](https://www.comsol.com/blogs?p=131391) | Calor que el cuerpo tolera de forma continua |

## Comunicación satelital

| Fuente | Para qué se usó |
|---|---|
| [Garmin fēnix 8 Pro](https://www.garmin.com/en-US/newsroom/press-release/wearables-health/introducing-fenix-8-pro-the-first-ever-smartwatches-from-garmin-with-inreach-technology-for-satellite-and-cellular-connectivity/) | Ejemplo de SOS satelital en un reloj |
| [Caso de estudio de GSMA sobre Skylo](https://www.gsma.com/get-involved/gsma-foundry/wp-content/uploads/2026/02/Ensuring-Wearables-Can-Always-Connect_Feb-26.pdf) | Cobertura de la red satelital |
| [Nordic nRF9151 con satélite](https://www.nordicsemi.com/Nordic-news/2026/08/Nordics-nRF9151-opens-satellite-and-cellular-IoT-to-a-new-class-of-connected-devices) | Módulo para una futura versión con SOS |

## Contenido

| Fuente | Para qué se usó |
|---|---|
| [Tamaños de Wikipedia en español para Kiwix](https://mundobytes.com/en/How-to-download-Wikipedia/) | Espacio necesario. Fuente secundaria, confirmar en el catálogo de Kiwix |

## Buenas prácticas del repositorio

| Fuente | Para qué se usó |
|---|---|
| [Keep a Changelog](https://keepachangelog.com/) | Formato del registro de cambios |
| [Versionado Semántico](https://semver.org/) | Numeración de versiones |
| [Conventional Commits](https://www.conventionalcommits.org/) | Formato de los mensajes de commit |
| [Registros de decisiones (ADR)](https://adr.github.io/) | Formato de las decisiones |
| [Contributor Covenant](https://www.contributor-covenant.org/) | Código de conducta |
| [Citation File Format](https://citation-file-format.github.io/) | Archivo para citar el proyecto |
| [Lista de licencias SPDX](https://spdx.org/licenses/) | Nombres y textos de las licencias |
