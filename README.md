# Proyecto Individual de MLOps: Sistema de Recomendación de Videojuegos

## Descripción del Proyecto

Este proyecto consiste en el desarrollo de una API utilizando **FastAPI** para implementar un sistema de recomendación de videojuegos para la plataforma Steam. La API permite obtener información sobre los juegos, reseñas de usuarios y datos relacionados con los géneros de los videojuegos. Además, el proyecto incluye análisis de sentimientos sobre las reseñas de los usuarios y la clasificación de los juegos más jugados y más populares.

## Cómo Usar este Proyecto

### Clonar el repositorio

```bash
git clone https://github.com/tuusuario/tu-repositorio.git
cd tu-repositorio
Instalar dependencias
Asegúrate de tener Python 3.7 o superior instalado. Instala las dependencias usando pip:
pip install -r requirements.txt
Ejecutar la API localmente
Para ejecutar la API en tu entorno local, utiliza el siguiente comando:
uvicorn main:app --reload

Acceso desde Render 
Este proyecto está desplegado en Render. Puedes acceder a los endpoints de la API utilizando la URL proporcionada por Render:

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
Railway: Plataforma de despliegue para la API.
Pandas: Librería utilizada para el procesamiento y análisis de los datos.
Python: Lenguaje principal del proyecto.
Despliegue
El proyecto ha sido desplegado exitosamente en Railway. Para acceder a la API en Railway, puedes utilizar la URL:
https://{tu-url-de-railway}/
Instrucciones Adicionales
Para cualquier duda o sugerencia, puedes ponerte en contacto a través de GitHub o abrir un "issue" en el repositorio.

Video Demostrativo
El video de demostración del proyecto puede encontrarse en este enlace [enlace a video].

1. Modifica el texto donde dice `https://{tu-url-de-railway}/` con la URL de Railway una vez que despliegues la API.
2. El video demostrativo se puede añadir después de haberlo grabado y subido a una plataforma (YouTube, Google Drive, etc.).

Si estás listo, puedo generar este archivo `README.md` y subirlo junto al código que tienes para que lo utilices en tu proyecto.




