# Resúmenes de Tesis

Plantillas de resúmenes de **pretesis**, **tesis** y **proyectos integradores**.
Cada resumen es un archivo con sus datos (autor, carrera, título, etc.) y el texto
del resumen.

## 1. Estructura

```
plantillas_resumen_tesis/
├── carreras.md                          # códigos de carrera (tabla de referencia)
└── plantillas/                          # plantillas en blanco
    ├── plantilla-pretesis-tesis.md
    └── plantilla-proyecto-integrador.md
```

## 2. Nombre del archivo

El nombre se forma con dos partes unidas por guiones: **`id-descripción.md`**

Ejemplo: `tes-C24-2026-1-003-modelo-deserción.md`

### 2.1. El `id` (identificador)

Es el identificador estable del resumen. Sigue el patrón
`tipo-carrera-semestre-correlativo` — ej. `tes-C24-2026-1-003`:

- **tipo**: `pti` (proyecto integrador) · `pre` (pretesis) · `tes` (tesis)
- **carrera**: código de carrera (ver [`carreras.md`](carreras.md))
- **semestre**: `AAAA-N` (N = 1 o 2)
- **correlativo**: 3 dígitos, de corrido en todo el semestre

### 2.2. La `descripción` corta

Son 2 o 3 palabras del título que hacen el nombre legible. Escríbela en minúsculas y
separa las palabras con guiones. Puedes usar tildes y ñ, pero no otros caracteres
especiales (`/`, `,`, `:`, `.`, `?`, paréntesis, comillas, etc.).

Ejemplo: en `tes-C24-2026-1-003-modelo-deserción.md`, la descripción corta es
`modelo-deserción` (del título «Modelo predictivo de deserción estudiantil»).

## 3. Contenido del documento

Cada archivo tiene dos partes: la **ficha de datos** y el **texto del resumen**.

La ficha va al inicio, entre líneas `---`, como una lista de `campo: valor`. El texto
del resumen va debajo del segundo `---`.

```yaml
---
id: tes-C24-2026-1-003
tipo: tesis
titulo: "Modelo predictivo de deserción estudiantil"
# ...resto de campos...
---

(aquí va el texto del resumen)
```

Campos de la ficha:

| Campo            | Proyecto integrador | Pretesis / Tesis | Descripción                                     |
|------------------|:-------------------:|:----------------:|-------------------------------------------------|
| `id`             | ✓                   | ✓                | Identificador estable (ver [Nombre del archivo](#2-nombre-del-archivo)) |
| `tipo`           | ✓                   | ✓                | `proyecto_integrador` / `pretesis` / `tesis`    |
| `departamento`   | ✓                   | ✓                | Departamento académico (`Tecnología Digital`)   |
| `carrera`        | ✓                   | ✓                | Nombre de la carrera (`Diseño y Desarrollo de Software`) (ver [`carreras.md`](carreras.md))     |
| `carrera_codigo` | ✓                   | ✓                | Código de carrera (`C24`)(ver [`carreras.md`](carreras.md))           |
| `semestre`       | ✓                   | ✓                | `AAAA-N` (N = 1 o 2)                             |
| `ciclo`          | ✓                   | ✓                | Ciclo académico (1–6)                           |
| `grupo`          | ✓                   | ✓                | Grupo                                           |
| `titulo`         | ✓                   | ✓                | Título del trabajo                              |
| `autores`        | ✓                   | ✓                | Lista de autores                                |
| `fecha`          | ✓                   | ✓                | `AAAA-MM-DD`                                     |
| `anio`           | ✓                   | ✓                | Año                                             |
| `palabras_clave` | ✓                   | ✓                | Palabras clave en español                       |
| `keywords`       | ✓                   | ✓                | Palabras clave en inglés                        |
| `seccion`        | ✓                   | —                | Solo proyecto integrador                        |
| `asesor`         | —                   | ✓                | Solo pretesis / tesis                           |

El campo `tipo` usa la palabra completa (`proyecto_integrador`, `pretesis`, `tesis`),
distinta del prefijo del `id` (`pti` / `pre` / `tes`).

## 4. Agregar un resumen

1. Descarga la plantilla que corresponda de [`plantillas/`](plantillas/): pretesis/tesis
   o proyecto integrador.
2. Completa el documento: la ficha de datos y el texto del resumen. Revisa que no queden textos de
   ejemplo.
3. Guarda el archivo como `id-descripción.md` (ver [Nombre del archivo](#2-nombre-del-archivo)).
4. Súbelo a la carpeta de Drive indicada: **[pega aquí el enlace del Drive]**.
