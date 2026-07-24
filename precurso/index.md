---
title: Material Precurso
subtitle: Contenidos, software y actividades preparatorias requeridas antes del inicio del curso.
---

## Acerca del material precurso

Para poder aprovechar al máximo las sesiones presenciales, es fundamental realizar una preparación previa. El material precurso es **obligatorio** para todos los participantes seleccionados. El diseño del curso asume que los participantes ya dominan estos conceptos y herramientas antes del primer día, permitiéndonos centrar las clases presenciales en dinámicas de aprendizaje activo, pedagogía y resolución de dudas complejas.

El material compartido está diseñado para que te prepares a tu propio ritmo e incluye:
- **Ejercicios prácticos** y guías paso a paso para consolidar lo aprendido.
- **Material de lectura** y recursos complementarios.
- **Videos explicativos** con talleres paso a paso o exposiciones teóricas.

### ⚠️ Requisitos de Software e Instalación de Datos

Antes de comenzar el curso, es necesario descargar e instalar varios programas y conjuntos de datos. **La conexión a internet en las aulas de la universidad puede ser lenta o inestable**, por lo que es sumamente importante que realices todas las descargas e instalaciones en tu hogar o lugar de trabajo antes de asistir al taller.

### 🧠 Conocimientos Básicos Necesarios

Además de las herramientas de software, existe una base de conocimientos y terminología conceptual que debes comprender antes del inicio de las clases. Asegúrate de revisar y familiarizarte con estos conceptos básicos para que no te encuentres con barreras lingüísticas o conceptuales durante las discusiones.

### 💬 Consultas y Resolución de Dudas

Si tienes preguntas sobre los temas teóricos, problemas al instalar el software o dificultades con los ejercicios prácticos, no dudes en consultar. Puedes solicitar ayuda de las siguientes maneras:

- A través del chat del curso en **Zulip**.

- Abriendo un **GitHub issue** en el repositorio oficial del curso: [GitHub Issues](https://github.com/acorbat/2026_TtT_Course/issues).

---

## Programas y Material para el Curso

Recomendamos instalar y configurar las siguientes herramientas antes de asistir:

### Pixi

[Pixi](https://pixi.prefix.dev/latest/) es un moderno gestor de paquetes y entornos que utilizaremos para asegurar que todos trabajemos con las mismas versiones de software. Sigue los pasos de instalación en [Pixi Installation](https://pixi.prefix.dev/latest/#installation).

### Git

Una vez que tengas Pixi en tu sistema, la forma recomendada de instalar Git de manera global es ejecutando en tu terminal:

```bash
pixi global install git
```

### Fiji

[Fiji](https://imagej.net/software/fiji/) es una distribución de ImageJ preconfigurada con una amplia colección de plugins. Se distribuye como una versión portable (no requiere instalación formal, solo descomprimir). Descarga la versión adecuada para tu sistema operativo desde la [página de descargas de Fiji](https://imagej.net/software/fiji/downloads).

### ilastik

[ilastik](https://www.ilastik.org/) es una herramienta interactiva para segmentación y clasificación de imágenes basada en aprendizaje automático. Consulta la [guía de instalación de ilastik](https://www.ilastik.org/documentation/basics/installation#basic-installation).

### QuPath (Opcional)

Si tu trabajo está relacionado con muestras histológicas o imágenes de gran tamaño (WSI), te sugerimos instalar QuPath desde [su página oficial](https://qupath.github.io/). Aunque no forma parte de los talleres principales, abordaremos conceptos compatibles y dispondrás de espacio para resolver dudas sobre su uso.

---

## Secciones y Temas Preparatorios

A continuación, se detallan los temas del precurso. Debes ingresar a cada página, completar las lecturas, ver los videos correspondientes y resolver los talleres prácticos indicados. Si manejas los temas descriptos en los objetivos de aprendizaje, no es necesario que hagas los ejercicios.

### 💻 [Línea de Comandos (CLI)](cli.md)

**Resumen:** Introducción a la terminal y comandos básicos para la navegación del sistema de archivos. Indispensable para ejecutar herramientas de desarrollo, versionado y automatización de flujos de trabajo.

* **Objetivos de Aprendizaje:**

  - Navegar el sistema de archivos desde la terminal (`cd`, `ls`/`dir`, `pwd`).

  - Crear, copiar, mover y eliminar archivos y directorios.

  - Ejecutar programas y scripts desde la línea de comandos.

---

### 🔬 [FIJI / ImageJ](fiji.md)

**Resumen:** Introducción al procesamiento y análisis cuantitativo de bioimágenes utilizando la Fiji.

* **Objetivos de Aprendizaje:**

  - Abrir y visualizar imágenes en FIJI.

  - Utilizar herramientas de selección y medición (ROIs).

  - Navegar menús y plugins de FIJI.

---

### 🐍 [Python](python.md)

**Resumen:** Fundamentos de sintaxis y programación en Python utilizando entornos interactivos, que servirán de base para las herramientas de análisis y automatización avanzadas.

* **Objetivos de Aprendizaje:**

  - Conocer la sintaxis básica de Python (variables, tipos de datos, funciones, bucles, condicionales).

  - Utilizar Jupyter Notebooks o un entorno interactivo de Python.

  - Importar y utilizar bibliotecas estándar (`numpy`, `matplotlib`).

  - Leer y manipular arreglos numéricos básicos.

---

## 📚 Conceptos Básicos y Lenguaje Técnico

Antes de iniciar el taller, es fundamental hablar el mismo idioma en cuanto a los términos propios de la disciplina. Te recomendamos dedicar un tiempo a estudiar la introducción y el glosario de términos esenciales de análisis de bioimágenes (píxeles, bits, dimensiones, formatos de archivo, etc.). A continuación encontrarás una clase de imagen digital dictada en el Curso de Fundamentos de Microscopía Óptica y de FLuorescencia de 2026 donde se abordan estos temas.

{{< video https://www.youtube.com/watch?v=FPcSHpwuAYc>}}

Corbat, A. A. (2026, May 11). Digital Image Lecture at Curso de Fundamentos de Microscopia Optica. Zenodo. https://doi.org/10.5281/zenodo.20126291
