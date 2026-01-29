# 🏦 Sistema de Predicción de Riesgo Crediticio con Machine Learning

![Estado del Proyecto](https://img.shields.io/badge/Estado-Completo-green)
![Tecnologías](https://img.shields.io/badge/Stack-SQL%20|%20Python%20|%20ML-blue)

Este proyecto implementa un ecosistema completo de análisis de datos para una entidad bancaria, pasando desde la ingesta de datos crudos en **SQL Server** hasta la creación de un modelo predictivo de **Machine Learning** en Python para determinar la probabilidad de impago (Default).

## 🚀 Resumen del Pipeline Técnico

El proyecto se dividió en tres fases críticas para garantizar la integridad y utilidad de los hallazgos:

### 1. Ingeniería de Datos (SQL Server)
* **ETL Avanzado**: Procesamiento de más de 32,000 registros mediante scripts de limpieza.
* **Normalización**: Diseño de tablas relacionales (`Clientes` y `Prestamos`) para optimizar la estructura de datos.
* **Lógica de Negocio**: Implementación de una **Vista de Semáforo de Riesgo** que clasifica clientes en categorías (Rojo, Amarillo, Verde) mediante lógica transaccional.

### 2. Análisis y Conectividad (Python)
* **Integración**: Conexión robusta entre **Jupyter Notebook** y **SQL Server** mediante la librería `pyodbc`.
* **EDA (Exploratory Data Analysis)**: Visualización de distribuciones de préstamos y correlaciones entre ingresos y morosidad utilizando `Seaborn` y `Matplotlib`.

### 3. Machine Learning (Random Forest)
* **Algoritmo**: Se utilizó un **Random Forest Classifier** por su capacidad para manejar variables categóricas y relaciones no lineales.
* **Variables Multidimensionales**: El modelo evalúa simultáneamente Edad, Ingreso Anual, Situación de Vivienda, Motivo del Préstamo y Tasa de Interés.
* **Interpretabilidad**: Generación de un ranking de importancia de variables (*Feature Importance*) para entender qué factores pesan más en el riesgo crediticio.



## 📊 Hallazgos de Negocio
* **Variables Críticas**: Se identificó que la **Tasa de Interés** y el **Ingreso Anual** son los principales indicadores de riesgo.
* **Segmentos de Alerta**: Los clientes con viviendas rentadas y préstamos para "Consolidación de Deuda" presentan una probabilidad de mora significativamente superior al promedio.

 ## 🎯 Impacto y Resultados de Negocio

Mi modelo no solo predice, sino que genera una lista de acción para el equipo de cobranzas, priorizando a los clientes que tienen un 100% de probabilidad de default basándose en su situación de vivienda y nivel de ingresos.

### Beneficios del proyecto:
* **Optimización de Cobranzas**: El equipo de riesgo ya no llama al azar, sino que contacta primero a los perfiles detectados por el Machine Learning.
* **Precisión en la Evaluación**: Identificación de patrones de riesgo (ej: Clientes en RENTA con bajos ingresos) que pasan desapercibidos en análisis tradicionales.
* **Automatización de Punta a Punta**: Desde la ingesta en SQL hasta el reporte final en Excel.

## 🛠️ Estructura del Repositorio
* `/sql`: Scripts de creación de base de datos, tablas y vistas.
* `/cuadernos`: Notebooks de Jupyter con el proceso de ML de punta a punta.
* `/datos`: Archivos procesados y reportes finales en Excel/CSV.
* `/paneles`: Capturas de pantalla de las gráficas y análisis visual.

## 👨‍💻 Autor
**Maidana Ignacio**
* [LinkedIn](TU_LINK_AQUÍ)
* [Portfolio](TU_LINK_AQUÍ)
