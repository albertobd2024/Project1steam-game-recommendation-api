
 ![banner-proyecto-1](https://github.com/user-attachments/assets/636b5174-2b09-45a4-a2d2-df92a7a36b25)
   




# Proyecto Individual de MLOps: Sistema de Recomendación de Videojuegos

## Descripción del Proyecto

Este proyecto consiste en el desarrollo de una API utilizando **FastAPI** para implementar un sistema de recomendación de videojuegos para la plataforma Steam. La API permite obtener información sobre los juegos, reseñas de usuarios y datos relacionados con los géneros de los videojuegos. Además, el proyecto incluye análisis de sentimientos sobre las reseñas de los usuarios y la clasificación de los juegos más jugados y más populares.

## Cómo Usar este Proyecto

### Clonar el repositorio

```bash
git clone https://https://github.com/albertobd2024/Project1steam-game-recommendation-api.git
cd tu-repositorio
Instalar dependencias
Asegúrate de tener Python 3.7 o superior instalado. Instala las dependencias usando pip:
pip install -r requirements.txt
Ejecutar la API localmente
Para ejecutar la API en tu entorno local, utiliza el siguiente comando:
uvicorn main:app --reload

Acceso desde Render 
Este proyecto está desplegado en Render. Puedes acceder a los endpoints de la API utilizando la URL proporcionada por Render:

https://project1steam-game-recommendation-api.onrender.com

Endpoints de la API
Aquí te presentamos los 6 endpoints disponibles en la API y sus descripciones:

1. Saludo Inicial:

Descripción: Endpoint de bienvenida que verifica que la API está funcionando correctamente.
URL: /
Respuesta:
{"message": "API is working!"}

2. Items más jugados:

Descripción: Devuelve una lista de los ítems (juegos) más jugados.
URL: /items/most_played?limit=10&offset=0
Respuesta: Lista de ítems con información de jugabilidad.

3. Reseñas positivas:

Descripción: Obtiene una lista de reseñas con sentimiento positivo.
URL: /reviews/positive?limit=10&offset=0
Respuesta: Lista de reseñas con análisis de sentimiento positivo.

4. Juegos gratuitos:

Descripción: Obtiene una lista de juegos que son gratuitos.
URL: /games/free?limit=10&offset=0
Respuesta: Lista de juegos con precio igual a cero.

5. Juegos de género Action:

Descripción: Filtra y devuelve los juegos del género "Action".
URL: /games/action?limit=10&offset=0

Respuesta: Lista de juegos del género de acción.

6. Reseñas más largas:

Descripción: Obtiene una lista de reseñas con mayor longitud.
URL: /reviews/longest?limit=10&offset=0
Respuesta: Lista de reseñas ordenadas por la longitud de texto.

Tecnologías Utilizadas
FastAPI: Framework para la creación de APIs rápidas y eficientes.
Ngrok: Herramienta para exponer la API de forma local para pruebas rápidas.
Render: Plataforma de despliegue para la API.
Pandas: Librería utilizada para el procesamiento y análisis de los datos.
Python: Lenguaje principal del proyecto.
Despliegue
El proyecto ha sido desplegado exitosamente en Render. Para acceder a la API en Render, puedes utilizar la URL:
(https://project1steam-game-recommendation-api.onrender.com)
Instrucciones Adicionales
Para cualquier duda o sugerencia, puedes ponerte en contacto a través de GitHub o abrir un "issue" en el repositorio.







