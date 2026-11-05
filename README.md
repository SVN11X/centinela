# Centinela

Reloj de supervivencia con inteligencia artificial local. Funciona sin internet y sin depender de un teléfono ni de otro aparato.

![Estado](https://img.shields.io/badge/estado-en%20desarrollo-orange)
![Etapa](https://img.shields.io/badge/etapa-0%20de%207-blue)
![Licencia](https://img.shields.io/badge/licencia-GPL--3.0--or--later-green)

> Este repositorio contiene la estructura de trabajo del proyecto. Todavía no hay código, diseños ni contenido final. Cada carpeta explica qué irá en ella y en qué etapa se completa.

## Qué es

Centinela es un reloj grande y resistente que reúne en la muñeca guías de emergencia, mapas, Wikipedia sin conexión y un asistente de inteligencia artificial que responde por voz. Todo ocurre dentro del reloj. Mientras se usa, no necesita teléfono, módulo de bolsillo ni internet.

El proyecto toma como referencia la aplicación [Nomad Pocket](https://github.com/franlindebl/nomad-pocket), que ofrece funciones parecidas en un teléfono.

## Principios

| Principio | Qué significa |
|---|---|
| Todo en uno | Ninguna función depende de otro aparato durante el uso. |
| Seguridad primero | Los procedimientos críticos salen de contenido revisado. La IA nunca los inventa. |
| La piel manda | La cara del reloj que toca la muñeca no pasa de 39 °C. |
| Medir antes de decidir | Cada decisión importante se respalda con una medición o una fuente registrada. |

## Organización del repositorio

```
centinela/
├── .github/      Plantillas de issues y pull requests, dueños del código
├── docs/         Visión, requisitos, arquitectura, etapas, decisiones y plantillas
├── hardware/     Electrónica: esquemáticos, placa y lista de materiales
├── mecanica/     Caja, correa y piezas impresas
├── software/     Programas del reloj y del módulo de IA
├── contenido/    Procedimientos, guías, banco de respuestas, mapas y rutas
├── modelos/      Modelos de IA, su origen y su licencia
├── pruebas/      Protocolos de prueba y resultados de mediciones
├── LICENSES/     Textos completos de las licencias
├── ROADMAP.md    Hoja de ruta por etapas
└── CHANGELOG.md  Registro de cambios por versión
```

## Etapas

El trabajo avanza por etapas. Cada una tiene objetivos, entregables y criterios para darla por cerrada. El resumen está en [ROADMAP.md](ROADMAP.md).

| Etapa | Nombre | Estado |
|---|---|---|
| 0 | [Definición](docs/etapas/etapa-0-definicion/) | En curso |
| 1 | [Prototipo de medición](docs/etapas/etapa-1-prototipo-de-medicion/) | Pendiente |
| 2 | [Contenido sin conexión](docs/etapas/etapa-2-contenido-sin-conexion/) | Pendiente |
| 3 | [Software](docs/etapas/etapa-3-software/) | Pendiente |
| 4 | [Electrónica propia](docs/etapas/etapa-4-electronica-propia/) | Pendiente |
| 5 | [Mecánica y térmica](docs/etapas/etapa-5-mecanica-y-termica/) | Pendiente |
| 6 | [Integración y pruebas en terreno](docs/etapas/etapa-6-integracion-y-pruebas-en-terreno/) | Pendiente |
| 7 | [Versión 1.0](docs/etapas/etapa-7-version-1-0/) | Pendiente |

## Cómo participar

Lee [CONTRIBUTING.md](CONTRIBUTING.md) antes de abrir un issue o un pull request. Las decisiones técnicas se registran en [docs/decisiones](docs/decisiones/) y toda la documentación está indexada en [docs](docs/).

## Licencias

| Parte | Licencia | Texto |
|---|---|---|
| Software | GPL-3.0-or-later | [LICENSE](LICENSE) |
| Hardware y mecánica | CERN-OHL-S-2.0 | [LICENSES/CERN-OHL-S-2.0.txt](LICENSES/CERN-OHL-S-2.0.txt) |
| Documentación | CC BY-SA 4.0 | [LICENSES/CC-BY-SA-4.0.txt](LICENSES/CC-BY-SA-4.0.txt) |
| Contenido de terceros | La de cada fuente | [docs/licencias-de-terceros.md](docs/licencias-de-terceros.md) |

La razón de esta elección está en la [decisión 0005](docs/decisiones/0005-licencias-del-proyecto.md).

## Aviso de seguridad

El proyecto está en desarrollo. No uses el reloj como única fuente de ayuda en una emergencia real. Si encuentras una respuesta o un procedimiento que podría dañar a alguien, repórtalo como indica [SECURITY.md](SECURITY.md).

## Cómo citar

Los datos para citar el proyecto están en [CITATION.cff](CITATION.cff). GitHub los muestra en el botón Cite this repository.
