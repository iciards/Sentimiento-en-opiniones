# Proyecto: Detección de Sentimiento en Opiniones de Productos de Amazon

## Descripción
Este proyecto forma parte del módulo de consolidación del Máster en Data Science de MBIT School. El objetivo es construir un modelo de clasificación de sentimiento utilizando Spark MLlib, entrenarlo con un subconjunto de reviews de productos de Amazon, y desplegarlo serializando el modelo en AWS S3.

## Dataset
- Fuente original: [Amazon Reviews Dataset](https://cseweb.ucsd.edu/~jmcauley/datasets/amazon_v2/)
- Subset utilizado: Opiniones sobre productos de la categoría Electronics, en formato Parquet

##  AWS y Spark
- Se utiliza AWS Glue para orquestación y lectura/escritura desde S3.
- El modelo se serializa en S3, permitiendo la reutilización en tareas de inferencia futuras.

##  Tecnologías y Herramientas
- Apache Spark (PySpark)
- AWS Glue
- AWS S3
- Python

## Objetivos del Proyecto
- Cargar y procesar el dataset en Spark
- Entrenar un modelo de clasificación de sentimientos
- Evaluar el modelo con métricas estándar
- Serializar y guardar el modelo en AWS S3
- Reutilizar el modelo en una nueva sesión para predicciones

## Estructura del Notebook
1. Configuración del entorno y lectura de datos desde S3
2. Preprocesamiento de texto
3. Creación del modelo de ML
4. Evaluación y métricas
5. Serialización y carga desde S3
