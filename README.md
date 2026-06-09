# RYLI03
Copa FutBotMX 2026 - Reto de Visión por Computadora 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

1)	Descripción del Proyecto
Este repositorio contiene nuestra entrega oficial para la **Copa FutBotMX (Capítulo Visión por Computadora)**, compitiendo en la categoría Amateur. Nuestro proyecto utiliza el **Segment Anything Model 3 (SAM 3)** de Meta para segmentar, rastrear y analizar de forma automatizada los partidos de fútbol robótico.

El objetivo principal es aplicar conceptos de visión por computadora para identificar el balón y los robots, generando estadísticas útiles y una narrativa visual del juego.

2)	Enfoque y Arquitectura
Nuestra solución está diseñada mediante el siguiente flujo de trabajo:
1. Detección y Segmentación (SAM 3): Utilizamos comandos y prompts) para indicarle al modelo cómo identificar de manera precisa a los robots y el balón en el campo de juego.
2. Seguimiento Visual (OpenCV): Implementamos OpenCV para dibujar cajas delimitadoras alrededor de los elementos detectados, permitiendo visualizar su trayectoria a lo largo de los fotogramas del video.
3. Análisis de Datos y Estadísticas: Desarrollamos una lógica de seguimiento que no solo observa el movimiento, sino que también clasifica a los robots por equipo y contabiliza métricas clave del partido, tales como:
•	*Número total de pases.
•	Conteo de goles.
•	Separación de estadísticas por equipo.

3)	Requisitos de Hardware y Software
Este proyecto fue desarrollado y optimizado para ejecutarse en la nube.
Entorno: Google Colab
Hardware: GPU NVIDIA T4
Versión de Python: 3.10+
Dependencias Principales: `torch` y `torchvision` (Requeridos para ejecutar el modelo SAM 3)
•	`opencv-python` (Para el procesamiento de video y dibujo)
•	`numpy`
•	`sam3` (Repositorio oficial de Meta)

4)	Instrucciones de Instalación y Reproducción
Para replicar nuestro entorno y obtener los resultados, sigue estos pasos:
1. Clonar el repositorio:
   ```bash
git clone [https://colab.research.google.com/drive/1euw_ejfaQBKeaXIYLDEllAd_hDxm09-k?usp=sharing]
 cd futbotmx-sam3
