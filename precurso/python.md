---
title: "Python"
subtitle: "Fundamentos de programación en Python para análisis de datos."
format: html
---

::: {.callout-tip}
## Objetivos de Aprendizaje

Al finalizar esta preparación, los participantes serán capaces de:

- Conocer la sintaxis básica de Python (variables, tipos de datos, funciones, bucles, condicionales).

- Utilizar Jupyter Notebooks o un entorno interactivo de Python.

- Importar y utilizar bibliotecas estándar (`numpy`, `matplotlib`).

- Leer y manipular arreglos numéricos básicos.

:::

Python es un lenguaje de programación de alto nivel, dinámico y multipropósito, ampliamente utilizado en ciencia de datos y análisis de bioimágenes por su sintaxis clara y su robusto ecosistema de bibliotecas. A continuación se presentan los enlaces al material del taller, aunque realizaremos la instalación de Python de una manera diferente.

## Taller y Material de Referencia

Aunque recomendamos realizar una instalación como la que se describe en la siguiente sección, el material oficial de referencia para este taller se encuentra en:

- [Taller de Python en GitHub](https://github.com/maurosilber/python-tutorial) (repositorio original).

- [Página web del Tutorial](https://maurosilber.github.io/python-tutorial).

## Configuración del Entorno de Trabajo

Para este curso, en lugar de realizar una instalación global de Python o usar otras herramientas, utilizaremos `pixi` para inicializar y gestionar el entorno de forma reproducible. Sigue estos pasos:

1. **Crear una carpeta de trabajo**: Abre tu terminal y crea un nuevo directorio llamado `python-tutorial`, luego ingresa a él:

   ```bash
   mkdir python-tutorial
   cd python-tutorial
   ```

2. **Inicializar el proyecto**: Crea un nuevo proyecto de `pixi` ejecutando:

   ```bash
   pixi init
   ```

3. **Agregar dependencias**: Añade Python, Jupyter y las librerías científicas necesarias corriendo:

   ```bash
   pixi add python jupyter numpy matplotlib
   ```

4. **Iniciar Jupyter Notebook**: Para abrir Jupyter Notebook y comenzar a escribir código, ejecuta:

   ```bash
   pixi run jupyter notebook
   ```
   Esto iniciará el servidor de Jupyter y abrirá la interfaz en tu navegador web. Desde allí podrás crear cuadernos interactivos (`.ipynb`) y seguir el tutorial.

## Actividades a Realizar

Debes seguir los pasos del material del taller disponible en [https://maurosilber.github.io/python-tutorial](https://maurosilber.github.io/python-tutorial) y completar las explicaciones y ejercicios hasta la sección de **Numpy y matplotlib** inclusive.

## Citation

Mauro Silberberg. (2026). maurosilber/python-tutorial: 20260724 (Version 20260724) [Computer software]. Zenodo. https://doi.org/10.5281/zenodo.21539956
