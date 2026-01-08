# Práctica: IA Local con Docker y Ollama

Este repositorio contiene el resultado de la práctica para desplegar un entorno de Inteligencia Artificial conversacional 100% local, garantizando la privacidad y soberanía de los datos.

## 🛠️ Arquitectura Final

El sistema se compone de los siguientes servicios orquestados con Docker Compose:

*   **Motor IA:** `Ollama` - Encargado de ejecutar los modelos de lenguaje.
*   **Interfaz Web:** `Open WebUI` - Proporciona la interfaz de chat para interactuar con la IA.
*   **Modelo LLM:** `qwen2.5:0.5b` - Seleccionado tras las pruebas por ser el modelo más ligero que ofrece un equilibrio óptimo entre bajo consumo de recursos y respuestas fiables.

## 🚀 Cómo Poner en Marcha el Proyecto

Para replicar este entorno, se necesitan los siguientes pasos:

1.  **Iniciar los servicios:**
    ```bash
    docker compose up -d
    ```

2.  **Descargar el modelo de IA:**
    ```bash
    docker compose exec ollama ollama pull qwen2.5:0.5b
    ```

3.  **Acceder a la aplicación:**
    Abre un navegador y visita la URL `http://localhost:3000`.

## 📂 Contenido del Repositorio

*   `docker-compose.yml`: Archivo de configuración de los servicios.
*   `reflexion.md`: Documento con el análisis, las dificultades encontradas y las conclusiones de la práctica.
*   `captura-interfaz.png`: Captura de pantalla que muestra la interfaz funcionando.
*   `captura-conversacion.png`: Captura de pantalla con un ejemplo de conversación.

## 👤 Autor

Alejandro Cayero
