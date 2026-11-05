# Cómo contribuir

Este documento explica cómo se organiza el trabajo, para que cualquier persona pueda seguirlo, incluida quien vuelva al proyecto después de un tiempo.

## Antes de empezar

1. Lee el [README](README.md) y la [hoja de ruta](ROADMAP.md).
2. Revisa en qué etapa está el proyecto.
3. Busca si ya existe un issue sobre lo que quieres hacer.

## Cómo se usa GitHub en este proyecto

| Herramienta | Uso |
|---|---|
| Hito (milestone) | Una etapa, con el nombre Etapa N |
| Issue | Una tarea, una falla, una medición o una propuesta de decisión |
| Pull request | Un cambio a los archivos, ligado a un issue |
| Projects | Tablero con las columnas Pendiente, En curso, En revisión y Hecho |
| Releases | Versión publicada al cerrar cada etapa |

## Flujo de trabajo

1. Crea o elige un issue con la plantilla que corresponda y asígnalo al hito de su etapa.
2. Crea una rama desde `main` con el formato `etapa-N/descripcion-corta`. Ejemplo: `etapa-1/medir-arranque`.
3. Haz los cambios y escribe commits claros.
4. Abre un pull request con la plantilla y escribe `Cierra #número` para enlazar el issue.
5. Revisa el pull request antes de unirlo a `main`. Si trabajas solo, revísalo al día siguiente con la lista de verificación de la plantilla.

En Settings, protege la rama `main` para que todo cambio entre por pull request.

## Mensajes de commit

Formato `tipo(área): descripción`, en minúsculas y en presente. Se basa en [Conventional Commits](https://www.conventionalcommits.org/).

| Tipo | Cuándo usarlo |
|---|---|
| docs | Documentación |
| hw | Electrónica |
| mec | Mecánica |
| sw | Software |
| cont | Contenido sin conexión |
| prueba | Protocolos y resultados |
| mant | Orden y mantenimiento del repositorio |

Ejemplos:

```
docs(etapa-1): agrega protocolo de medición de arranque
hw(placa): corrige el interruptor del módulo de IA
prueba(p-03): registra temperatura de la piel con 10 preguntas
```

## Nombres de archivos y carpetas

- Minúsculas, sin tildes, sin ñ y sin espacios. Las palabras se unen con guion. Ejemplo: `revision-de-cierre.md`.
- Fechas en formato AAAA-MM-DD.
- Decisiones numeradas con cuatro dígitos. Ejemplo: `0006-nombre-corto.md`.

## Unidades y números

- Sistema internacional: V, A, W, Wh, mAh, °C, mm y g.
- En textos, coma decimal (1,5 W). En archivos CSV, punto decimal (1.5), para que las planillas y los programas los lean sin errores.

## Archivos grandes

- No subas modelos de IA, mapas, Wikipedia ni videos. Anota en el README de su carpeta el enlace y la versión.
- Los archivos 3D (STEP, STL, 3MF y FreeCAD) se guardan con Git LFS. Instálalo una vez con `git lfs install`.
- Las hojas de datos de los fabricantes no se suben. Se guarda solo su enlace.

## Decisiones

Toda decisión que cambie la arquitectura, un componente principal o la meta de un requisito se registra en [docs/decisiones](docs/decisiones/) con la plantilla 0000.

## Mediciones

Cada medición se registra con la [plantilla de informe](docs/plantillas/informe-de-medicion.md) en `pruebas/resultados/AAAA-MM-DD-tema/`. Una tarea de medición se cierra solo con su informe enlazado.

## Seguridad de las personas

Los cambios en `contenido/procedimientos-criticos/` necesitan la revisión de un profesional de salud, con su nombre y la fecha en el archivo.

## Etiquetas sugeridas

| Etiqueta | Uso |
|---|---|
| etapa-0 a etapa-7 | Etapa a la que pertenece |
| tarea | Trabajo planificado |
| falla | Algo no funciona como se esperaba |
| medicion | Registro de una prueba |
| decision | Propuesta de decisión técnica |
| riesgo | Riesgo nuevo o que cambió |
| seguridad | Puede afectar a personas o datos |
| bloqueado | Espera algo externo |

## Versiones

Las versiones siguen [Versionado Semántico](https://semver.org/). Al cerrar cada etapa sube la versión: la etapa 0 publica la v0.1.0, la etapa 1 la v0.2.0, y así hasta la etapa 7, que publica la v1.0.0. Cada versión se anota en [CHANGELOG.md](CHANGELOG.md).
