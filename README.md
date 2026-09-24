# Análisis de Clientes y Consumo - ConnectaTel

## Objetivo del Proyecto
El objetivo principal de este proyecto es analizar el comportamiento de los clientes de la empresa de telecomunicaciones ConnectaTel en Latinoamérica (con datos hasta 2024). A través de la exploración, limpieza y segmentación de los datos, se busca identificar patrones de consumo, detectar comportamientos atípicos (heavy users) y generar insights ejecutivos para el diseño de estrategias de retención y mejora de planes comerciales.

## Datasets Utilizados
El análisis se fundamenta en tres bases de datos principales:
* `plans.csv`: Información de los planes actuales (Básico y Premium), incluyendo precios, minutos y GB incluidos, y costos adicionales.
* `users_latam.csv`: Información demográfica de los clientes (edad, ciudad, plan contratado, fechas de registro y abandono).
* `usage.csv`: Registro detallado del uso real de los servicios, especificando tipo (llamadas o mensajes), fecha, duración y cantidad.

## Etapas del Análisis Realizadas
1. **Carga y Exploración:** Lectura inicial de los datos e identificación de la estructura general y tipos de datos.
2. **Limpieza de Datos:** Tratamiento de valores nulos (técnica MAR), corrección de valores centinela (ej. edad -999) y estandarización de fechas.
3. **Estadísticas y Agrupación:** Consolidación del consumo por usuario (mensajes, llamadas, minutos) y unión con la base de datos demográfica.
4. **Análisis de Distribuciones y Outliers:** Visualización con histogramas y diagramas de caja para entender la dispersión y justificar la retención de usuarios atípicos (heavy users).
5. **Segmentación de Clientes:** Clasificación mediante lógica condicional para agrupar clientes por Nivel de Uso (Bajo, Medio, Alto) y Grupo de Edad (Joven, Adulto, Adulto Mayor).
6. **Insight Ejecutivo:** Conclusiones estratégicas y recomendaciones comerciales basadas en los hallazgos.

## Cómo ejecutar el notebook
Para reproducir este análisis:
1. Clona este repositorio o descarga el archivo `.ipynb`.
2. Sube el notebook a **Google Colab** o ábrelo localmente usando **Jupyter Notebook**.
3. Asegúrate de tener instaladas las librerías `pandas`, `seaborn` y `matplotlib`.
4. Carga los datasets en las rutas especificadas en el primer bloque de código (`/datasets/...`) o ajusta las rutas según tu entorno local.
5. Ejecuta las celdas en orden (Run All) para replicar el proceso de limpieza y generar las visualizaciones.
