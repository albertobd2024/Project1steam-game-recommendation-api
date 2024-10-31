
 ![banner-proyecto-1](https://github.com/user-attachments/assets/636b5174-2b09-45a4-a2d2-df92a7a36b25)
   

🚀 Proyecto Individual de MLOps: Sistema de Recomendación de Videojuegos
🎮 Descripción del Proyecto
Este proyecto desarrolla una API utilizando FastAPI para implementar un sistema de recomendación de videojuegos en Steam. Incluye:

Información detallada de videojuegos 🎲
Análisis de reseñas de usuarios 📝
Clasificación de juegos por popularidad, género, y más 💡

🛠️ Clonación e Instalación
Clonar el repositorio

bash
Copiar código
git clone https://github.com/albertobd2024/Project1steam-game-recommendation-api.git
cd Project1steam-game-recommendation-api
Instalar dependencias
Asegúrate de tener Python 3.7 o superior. Instala las dependencias:

bash
Copiar código
pip install -r requirements.txt

🏃‍♂️ Ejecución de la API Localmente
Para ejecutar la API en tu entorno local, usa:

bash
Copiar código
uvicorn main:app --reload
🌐 Acceso desde Render
El proyecto está desplegado en Render y accesible en:

🔗 https://project1steam-game-recommendation-api.onrender.com

📂 Endpoints de la API
Aquí te presentamos los endpoints disponibles en la API y sus descripciones:

👋 Saludo Inicial

Descripción: Endpoint de bienvenida para verificar el funcionamiento de la API.
URL: /
Respuesta:
json
Copiar código
{"message": "API is working!"}
🎮 Items más jugados

Descripción: Lista de los juegos más jugados.
URL: /items/most_played?limit=10&offset=0
Respuesta: Información de jugabilidad de los juegos.
😊 Reseñas positivas

Descripción: Reseñas con sentimiento positivo.
URL: /reviews/positive?limit=10&offset=0
Respuesta: Lista de reseñas con sentimiento positivo.
💸 Juegos gratuitos

Descripción: Juegos disponibles de forma gratuita.
URL: /games/free?limit=10&offset=0
Respuesta: Lista de juegos con precio igual a cero.
🎯 Juegos de género Action

Descripción: Juegos filtrados por el género "Action".
URL: /games/action?limit=10&offset=0
Respuesta: Lista de juegos del género de acción.
📏 Reseñas más largas

Descripción: Reseñas ordenadas por longitud.
URL: /reviews/longest?limit=10&offset=0
Respuesta: Lista de reseñas con mayor longitud de texto.


🔧 Tecnologías Utilizadas
FastAPI 🚀: Framework para crear APIs rápidas y eficientes.
Ngrok 🌐: Herramienta para exponer la API de forma local para pruebas rápidas.
Render 🚀: Plataforma de despliegue para la API.
Pandas 📊: Librería para el procesamiento y análisis de datos.
Python 🐍: Lenguaje principal del proyecto.

🚀 Despliegue
El proyecto ha sido desplegado exitosamente en Render. Para acceder a la API, utiliza:

🔗 https://project1steam-game-recommendation-api.onrender.com

📬 Instrucciones Adicionales
Para dudas o sugerencias, contáctanos en GitHub o abre un "issue" en el repositorio.





