# Trabajo Práctico Integrador N°1 - Sistema de Análisis de Documentos Digitalizados

## Descripción

Este repositorio contiene un trabajo práctico de la materia **Procesamiento de Imágenes** del IFTS24, cuyo objetivo es desarrollar un sistema básico de análisis automático de documentos digitalizados. Se implementan técnicas de preprocesamiento de imágenes para mejorar la calidad y segmentar los documentos.

## Contenido

* **notebook.ipynb**: Cuaderno interactivo que realiza la carga, análisis, preprocesamiento y visualización de imágenes.
* **dataset/**: Carpeta que contiene 3 imágenes de ejemplo:

  1. Buena calidad
  2. Rotada
  3. Con problemas de iluminación o contraste

## Tecnologías y Librerías

* **Python 3.x**
* **Numpy**: manejo de matrices y operaciones numéricas.
* **OpenCV (cv2)**: carga, conversión de color, rotación, ecualización, umbralización.
* **Matplotlib**: visualización de imágenes y gráficos, incluyendo histogramas y grids comparativos.

## Funcionalidades

1. **Carga y visualización de imágenes**: convierte imágenes a RGB y muestra información básica (dimensiones, tipo, rango de valores).
2. **Inspección visual y análisis**: gráficos lado a lado y histogramas para evaluar contraste y brillo.
3. **Preprocesamiento básico**:

   * Conversión a escala de grises
   * Ecualización de histograma para mejorar contraste
   * Umbralización para segmentación
   * Corrección de rotación mediante transformaciones geométricas
4. **Comparación de resultados**: visualización de imágenes originales y procesadas en un grid.

## Uso

1. Clonar el repositorio.
2. Colocar tus 3 imágenes de documentos en la carpeta `dataset/`.
3. Ejecutar el notebook paso a paso.
4. Ajustar parámetros de umbral, rotación y ecualización según la imagen.

```python
# Ejemplo de carga de una imagen
from utils import cargar_imagen, mostrar_info_imagen

ruta = 'dataset/imagen1.jpg'
imagen = cargar_imagen(ruta)
mostrar_info_imagen(imagen, 'Imagen de ejemplo')
```

## Resultados

* Las imágenes se muestran lado a lado: originales vs procesadas.
* Se visualizan histogramas para cada imagen.
* Se aplican técnicas adaptadas según el tipo de problema de cada imagen.

## Reflexión

* Aprendizaje de técnicas básicas de preprocesamiento de imágenes.
* Identificación de problemas de iluminación, contraste y rotación.
* Visualización de cómo cada técnica impacta en la segmentación.

## Autor

* Nombre: \[COMPLETAR]
* Fecha de entrega: 24 de Septiembre de 2025
