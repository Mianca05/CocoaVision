# Introducción
Este repositorio contiene los scripts del proyecto "Cocoa Vision". Se desarrollaron modelos de ML y DL para la de detección monilia (Moniliophthora roreri) en los cultivos de cacao, la cual es una enfermedad muy grave en dichos cultivos. Básicamente el modelo clasifica si una planta se encuentra con monilia y si está sana. Para ello se utilizó un conjunto de datos privado. 
# Contenido
* **1_Preprocesamiento_img**: este directorio contiene la fase de preprocesamiento de imágenes de cacao. Las actividades realizadas fueron generar nuevas imágenes (data aumentation), redimensionar, eliminar el fondo de las imágenes y sacar el ruido.
* **2_extraccion_caracteristicas**: en el archivo Colores_dataset.ipynb se extraen los vectores de características por escala de colores. En cambio, en el archivo Textura_dataset.ipynb se extrae la textura superficial de las imágenes de cacao. Ambas características se guardan en archivos de datos h5.
* **ML** : se utiliza el modelo SVM, aunque no es necesario utilizar la técnica OvO se utilizó ya que en base a hiperparámetros se obtuvo se mejoró el modelo. 
* **DL** : se utiliza Inception_v3 y MobileNetV2, con ambos modelos se obtuvieron resultados muy prometedores para la continuidad del proyecto.

## Librerías utilizadas
* Numpy
* OpenCV
* Tensorflow
* Keras
* Rembg
* Scikit-learn
* h5py
* Mahotas
* Seaborn