# Proyecto Individual Nº1: Sistema de Recomendación para Steam

## Descripción del Proyecto

Este proyecto tiene como objetivo el desarrollo de un sistema de recomendación de videojuegos para la plataforma Steam, utilizando técnicas de Machine Learning y procesamiento de datos en un entorno de MLOps. La solución incluye el diseño y deployment de una API RESTful con FastAPI, que permite realizar consultas sobre los datos de los juegos y usuarios, así como un sistema de recomendación basado en la similitud entre juegos y usuarios.

### Rol del MLOps Engineer

Como parte de este proyecto, he trabajado en la creación de un pipeline completo de Machine Learning que cubre el ciclo de vida de los datos: desde la limpieza y transformación de los datasets hasta el entrenamiento de un modelo de recomendación. Además, se ha construido una API que expone estos resultados a través de endpoints específicos para su consumo por otras aplicaciones o equipos dentro de la empresa.

## Datasets Utilizados

1. **steam_games.json.gz**: Contiene información sobre los juegos disponibles en Steam, incluyendo géneros, precios y desarrolladores.
2. **user_reviews.json.gz**: Incluye reseñas de los usuarios sobre los juegos, que han sido analizadas mediante técnicas de NLP para clasificar el sentimiento de las reseñas (positivo, neutro o negativo).
3. **users_items.json.gz**: Información sobre las interacciones de los usuarios con los juegos, incluyendo horas jugadas y recomendación de juegos.

## Funcionalidades de la API

La API cuenta con los siguientes endpoints:

- **`/developer/{desarrollador}`**: Devuelve la cantidad de ítems y el porcentaje de contenido gratuito por año, según la empresa desarrolladora.
  
- **`/userdata/{user_id}`**: Devuelve información sobre el dinero gastado por el usuario, porcentaje de recomendación en base a las reseñas y la cantidad de ítems jugados.

- **`/UserForGenre/{genero}`**: Muestra el usuario que acumula más horas jugadas en un género dado y una lista con la acumulación de horas jugadas por año de lanzamiento.

- **`/best_developer_year/{año}`**: Devuelve los 3 mejores desarrolladores con juegos más recomendados por los usuarios para el año seleccionado.

- **`/developer_reviews_analysis/{desarrollador}`**: Análisis de reseñas de los juegos de un desarrollador específico, mostrando la cantidad de reseñas positivas y negativas.

- **`/recomendacion_juego/{id_producto}`**: Recomendación basada en la similitud entre juegos (modelo item-item).

- **`/recomendacion_usuario/{id_usuario}`**: Recomendación basada en la similitud entre usuarios (modelo user-item).

## Feature Engineering

Se ha creado una nueva columna llamada `sentiment_analysis` en el dataset de reseñas de usuarios. Esta columna clasifica las reseñas en tres categorías:
- 0: Reseña negativa
- 1: Reseña neutral
- 2: Reseña positiva

En caso de que una reseña esté ausente, se le asigna el valor 1 (neutral).

## Análisis Exploratorio de Datos (EDA)

Se ha realizado un análisis exploratorio de los datasets para identificar patrones, anomalías y relaciones entre las variables. Este proceso incluye la identificación de outliers y la generación de visualizaciones como nubes de palabras para entender mejor la frecuencia de ciertos términos en los títulos y descripciones de los juegos.

## Modelo de Recomendación

Se han implementado dos enfoques para el sistema de recomendación:
1. **Recomendación ítem-ítem**: Basada en la similitud entre juegos, utilizando la similitud del coseno para recomendar juegos similares a uno seleccionado.
2. **Recomendación usuario-ítem**: Basada en la similitud entre usuarios, donde se recomiendan juegos que les gustaron a usuarios similares al usuario consultado.

Ambos modelos están expuestos a través de la API, permitiendo consultas dinámicas.

## Deployment

El proyecto ha sido deployado en **Railway**, y la API puede ser consumida desde cualquier dispositivo con acceso a internet. Esto asegura que tanto los modelos de recomendación como los datos estén disponibles para los departamentos de Analytics y Machine Learning.

## Video Demostrativo

El video de demostración del proyecto muestra el funcionamiento de la API, las consultas realizadas y una breve explicación de los modelos utilizados. Tiene una duración de menos de 7 minutos y puede ser visualizado en el siguiente enlace:

[Enlace al video](URL_DEL_VIDEO)

## Estructura del Repositorio

- `proyecto1_machinelearning_alberto_bernal.py`: Código del proyecto, incluyendo la limpieza de datos, entrenamiento de modelos y definición de la API.
- `steam_games_cleaned_simple.csv`: Dataset de juegos, después de la limpieza y transformación.
- `users_items_preprocesado.csv`: Dataset de usuarios y sus interacciones, listo para el modelo.
- `requirements.txt`: Archivo con las dependencias necesarias para ejecutar el proyecto.
- `README.md`: Este archivo.

## Requisitos Técnicos

Para ejecutar el proyecto de forma local, se necesita tener instaladas las siguientes dependencias:
- Python 3.8 o superior
- FastAPI
- Pandas
- Scikit-learn
- Uvicorn

## Conclusión

Este proyecto es una demostración del ciclo completo de MLOps, desde la recolección y tratamiento de datos hasta la implementación de un sistema de recomendación y su exposición a través de una API. A través de este MVP, se entrega una solución funcional y escalable para la plataforma Steam, facilitando la personalización de recomendaciones para los usuarios de la plataforma.

