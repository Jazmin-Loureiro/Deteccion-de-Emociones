# Detector de Emociones Multimodal (NLP & Computer Vision) 🧠📸

Este proyecto implementa un modelo de **Inteligencia Artificial** híbrido capaz de clasificar emociones tanto en textos de redes sociales como en expresiones faciales a través de imágenes.
Desarrollado como proyecto de extensión para la **Diplomatura en Programación de IA (IFES)**.

🚀 **Resumen Técnico / Technical Overview**

**🇦🇷 Español**

* **Objetivo:** Identificar múltiples emociones (Alegría, Tristeza, Odio, Miedo, etc.) basadas en la rueda de Plutchik en textos en español y rostros humanos.
* **Modelo NLP:** Clasificador multiclase entrenado con el dataset **HRECPW** (Hispanic Responses for Emotional Classification).
* **Modelo de Visión:** Implementación de **DeepFace** y **Haar Cascades** para el reconocimiento de expresiones faciales y determinación de la emoción dominante.
* **Procesamiento de Datos:**
    * Carga eficiente de datos mediante formato **Parquet**.
    * Limpieza de texto profunda usando **Regex** (eliminación de etiquetas HTML, URLs y caracteres especiales).
    * Análisis exploratorio de datos (EDA) con **Seaborn** para verificar el balanceo de clases emocionales.
* **Resultados:** El sistema permite una detección dual (texto e imagen) con métricas de confianza para cada emoción detectada.

**🇺🇸 English**

* **Objective:** Identify multiple emotions (Joy, Sadness, Hate, Fear, etc.) based on Plutchik's Wheel in Spanish text and human faces.
* **NLP Model:** Multiclass classifier trained on the **HRECPW** dataset (Hispanic Responses for Emotional Classification).
* **Vision Model:** Implementation of **DeepFace** and **Haar Cascades** for facial expression recognition and dominant emotion determination.
* **Data Processing:**
    * Efficient large-scale data loading using **Parquet** format.
    * Deep text cleaning using **Regex** (removal of HTML tags, URLs, and special characters).
    * Exploratory Data Analysis (EDA) with **Seaborn** to verify emotional class balancing.
* **Results:** The system enables dual detection (text and image) with confidence metrics for each detected emotion.

🛠️ **Tecnologías / Tech Stack**

* **Lenguaje:** Python 🐍
* **Librerías principales:** * **Pandas & PyArrow** (Manipulación de datos y manejo de Parquet)
    * **DeepFace & TensorFlow** (IA para Visión Artificial)
    * **OpenCV** (Procesamiento de imágenes y detección facial)
    * **NLTK** (Procesamiento de lenguaje natural)
    * **Matplotlib & Seaborn** (Visualización estadística de datos)

📂 **Estructura del Repositorio**

* **Detector_de_Emociones.ipynb:** Notebook principal que contiene todo el flujo de trabajo: carga, limpieza, entrenamiento y pruebas.
* **Data/:**
    * `train.parquet` & `validation.parquet`: Datasets originales en formato optimizado.
    * **Imagenes/:** Carpeta local para alojar las muestras (.jpg, .png) para pruebas de reconocimiento facial.

💻 **Instalación y Uso**

1. Clona el repositorio.
2. Asegúrate de tener instaladas las dependencias:
   `pip install pandas numpy opencv-python deepface tf-keras matplotlib seaborn pyarrow`

