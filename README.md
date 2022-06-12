# Práctica Deep Learning

Este es el repositorio que contiene los archivos necesarios para realizar la práctica de la asignatura de Deep Learning del Bootcamp Big Data y Machine Learning.

## Objetivo

El objetivo es predecir el precio de la vivienda en la ciudad de Madrid a partir de un dataset de apartamentos de Airbnb. 
La predicción se realizará tendiendo en cuenta tanto datos numéricos como imágenes.

Se ha usado un dataset con datos reales pero reducido, con 14780 observaciones ya que lo importante en este caso no es el resultado, si no el procedimiento.

## Dataset 

El dataset usado en este proyecto se obtiene de [esta url](https://public.opendatasoft.com/explore/dataset/airbnb-listings/export/?disjunctive.host_verifications&disjunctive.amenities&disjunctive.features&q=Madrid&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJ5QXhpcyI6Imhvc3RfbGlzdGluZ3NfY291bnQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20ifV0sInhBeGlzIjoiY2l0eSIsIm1heHBvaW50cyI6IiIsInRpbWVzY2FsZSI6IiIsInNvcnQiOiIiLCJzZXJpZXNCcmVha2Rvd24iOiJyb29tX3R5cGUiLCJjb25maWciOnsiZGF0YXNldCI6ImFpcmJuYi1saXN0aW5ncyIsIm9wdGlvbnMiOnsiZGlzanVuY3RpdmUuaG9zdF92ZXJpZmljYXRpb25zIjp0cnVlLCJkaXNqdW5jdGl2ZS5hbWVuaXRpZXMiOnRydWUsImRpc2p1bmN0aXZlLmZlYXR1cmVzIjp0cnVlfX19XSwidGltZXNjYWxlIjoiIiwiZGlzcGxheUxlZ2VuZCI6dHJ1ZSwiYWxpZ25Nb250aCI6dHJ1ZX0%3D&location=16,41.38377,2.15774&basemap=jawg.streets)

## Resolución del problema

La resolución de la práctica se ha hecho en Python usando varios notebooks de Jupyter donde en cada uno se intenta explicar el procedimiento paso a paso.

### 1. Descargar imágenes de los apartamentos
Las imágenes no están incluidas en el repositorio GitHub. Pero el proceso de obtencisión se explica en el siguiente Notebook:

[Descarga de imágenes](descargarImagenes.ipynb)

### 2. Tratamiento de datos
Se realiza una serie de operaciones para la limpieza y el tratamiento de los datos. 
Se encuentra en el siguiente Notebook:

[Tratamiento de datos](limpiezaEscalado.ipynb)

### 3. Red neuronal regresión con datos numéricos
En este paso se usan los datasets que contienen únicamente datos numéricos para hacer una red neuronal tradicional y predecir el precio del apartamento.
Se encuentra en el siguiente Notebook:

[Red neuronal tradicional](redesNeuronalesNumerico.ipynb)

### 4. Red neuronal combinando datos numéricos (MLP) con imágenes (CNN)
En este paso se usa los datos numéricos para generar un modelo MLP y las imágenes para generar un modelo CNN. Luego se combina los modelos y se evalua los resultados de ese modelo final(conjunto).
Se encuentra en el siguiente Notebook:

[Redes neuronales mixtas](redesNeuronalesMixto.ipynb)