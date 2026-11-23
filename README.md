# TP3 - Visión por Computadora I

Esta carpeta contiene la resolución del TP3 de la materia Visión por Computadora I (CEIA / FIUBA). El trabajo consiste en encontrar el logo de Coca-Cola en un conjunto de imágenes a partir de un template.

## Autores

- Celeste Corominas
- Julián Fierens
- Christian Yanez

## Contenido

- `TP3.ipynb`: resolución del trabajo práctico.
- `images/`: las siete imágenes donde se busca el logo.
- `template/`: el template del logo (`pattern.png`).
- `requirements.txt`: dependencias necesarias para correr el notebook.
- `README.md`: este archivo.

## Entorno

Para correr el notebook se usa un entorno conda llamado `vision_cv`. Fue creado a partir del entorno `ia_env` (creado en otra materia del posgrado) agregando la librería de OpenCV, que es la única que faltaba para este trabajo.

Características del entorno:

- Python 3.12.13
- opencv-python 5.0.0
- numpy 2.5.0
- matplotlib 3.11.0
- jupyter (IPython 9.15.0, notebook)

## Creación del entorno

El entorno local se creó con estos comandos:

```
conda create -n vision_cv --clone ia_env
conda activate vision_cv
pip install opencv-python
```

## Creación del entorno en otra computadora

Para reproducir el entorno desde cero en otra máquina alcanza con:

```
conda create -n vision_cv python=3.12
conda activate vision_cv
pip install -r requirements.txt
```

El archivo `requirements.txt` reúne los paquetes que se necesitan para resolver este trabajo.

## Cómo ejecutar el notebook

Con el entorno activado, abrir Jupyter y lanzar el notebook:

```
conda activate vision_cv
jupyter notebook TP3.ipynb
```

La carpeta de trabajo debe ser esta misma carpeta, porque el notebook lee las imágenes y el template con rutas relativas.
