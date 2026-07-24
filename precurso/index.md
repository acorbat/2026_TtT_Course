---
title: Material Precurso
subtitle: Contenidos y actividades preparatorias requeridas antes del inicio del curso.
---

## Acerca del material precurso

El siguiente material precurso es **obligatorio** para todos los participantes seleccionados. Los contenidos de este curso asumen que los participantes ya dominan estos temas antes del primer día. Si ya dominas los temas, no hace falta que los realices.

::: {.callout-important}
## Prerequisitos del Curso

Al comenzar el curso, los participantes deberán ser capaces de:

### Línea de Comandos (CLI)

- Navegar el sistema de archivos desde la terminal (`cd`, `ls`/`dir`, `pwd`).

- Crear, copiar, mover y eliminar archivos y directorios.

- Ejecutar programas y scripts desde la línea de comandos.

### FIJI / ImageJ

- Abrir y visualizar imágenes en FIJI.

- Aplicar operaciones básicas de procesamiento (filtros, ajuste de brillo/contraste).

- Navegar menús y plugins de FIJI.

### Python

- Conocer la sintaxis básica de Python (variables, tipos de datos, funciones, bucles, condicionales).

- Utilizar Jupyter Notebooks o un entorno interactivo de Python.

- Importar y utilizar bibliotecas estándar (`numpy`, `matplotlib`).

- Leer y manipular arreglos numéricos básicos.

:::

## Programas y material para el curso

::: {.callout-important}

Es fuertemente recomendado instalar varios programas y descargar paquetes de datos antes del curso ya que puede que las descargas desde la universidad sean lentas. Para eso recomendamos realizar todos los pasos de ésta sección.

:::

### Pixi

[Pixi](https://pixi.prefix.dev/latest/) es un administrador de paquetes y puede instalarse siguiendo los pasos descriptos [aquí](https://pixi.prefix.dev/latest/#installation).

### Git

Una vez instalado `Pixi`, lo mejor es instalar `Git` a traves de `Pixi` con el siguiente comando

```bash
pixi global install git
```

### Fiji

[Fiji](https://imagej.net/software/fiji/) es un paquete para procesamiento de imágenes, también llamado ImageJ2 con baterias. Se distribuye en una versión [portable](https://imagej.net/software/fiji/downloads), es decir, que no hace falta instalarlo.

### Material del curso

Para descargar el material del curso, 

### ilastik

Para descargar e instalar ilastik, recomendamos seguir los pasos en su [página](https://www.ilastik.org/documentation/basics/installation#basic-installation).

### QuPath (opcional)

Si soles trabajar con muestras de histología o histopatología, muestras teñidas de gran tamaño o afínes, recomendamos que instales QuPath desde [su página](https://qupath.github.io/). Aunque no hay talleres específicamente dedicados, abordaremos algunos temas y habrá tiempo para que lo explores.

## Secciones

Cada sección incluye un video introductorio en YouTube y un taller práctico en GitHub para que puedas prepararte a tu propio ritmo.

| Tema | Descripción |
|------|-------------|
| [Línea de Comandos (CLI)](cli.md) | Fundamentos de la terminal y navegación del sistema de archivos. |
| [FIJI / ImageJ](fiji.md) | Introducción al procesamiento de imágenes con FIJI. |
| [Python](python.md) | Fundamentos de programación en Python para análisis de datos. |
