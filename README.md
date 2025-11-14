# FIFA World Cup — Data Scraping & 2026 Prediction

Este proyecto tiene como objetivo **extraer datos históricos de los Mundiales de Fútbol (FIFA World Cup)** usando Web Scraping desde Wikipedia, construir un **dataset limpio de resultados pasados** y posteriormente utilizar esa información para **predecir posibles resultados del Mundial 2026**.

Este repositorio incluye:
- Código de scraping (`webscraping_data.ipynb`)
- Código de predicción basado en machine learning (`prediction_2026_worldcup.ipynb`)
- Datasets generados con el scraping (CSV)

---

## 1. Objetivo del Proyecto

1. **Recolectar datos históricos** de todos los mundiales desde 1930 hasta 2018.  
2. **Limpiar, estructurar y guardar** esos datos en archivos CSV.  
3. **Entrenar modelos de machine learning** para analizar patrones de resultados.  
4. **Predecir los resultados del Mundial 2026** usando características históricas.

---

## 2. Contenidos del Repositorio
/
├── webscraping_data.ipynb # Script de Web Scraping con BeautifulSoup
├── prediction_2026_worldcup.ipynb # Modelo predictivo para el Mundial 2026 (Editando en Jupyter labs)
├── data/
│ ├── fifa_worldcup_historical_data.csv
│ └── fifa_worldcup_fixture_2026.csv
└── README.md

## 3. Web Scraping

El archivo **`webscraping_data.ipynb`**:

- Extrae resultados de cada partido por mundial  
- Omite los años que no se jugaron (1942 y 1946)  
- Guía paso a paso cómo usar `requests`, `BeautifulSoup` y `pandas`  
- Genera datasets limpios para análisis posteriores  

Tecnologías usadas:
- `requests`
- `BeautifulSoup4`
- `pandas`
- `lxml`

## 4. Predicción del Mundial 2026

En el archivo **`prediction_2026_worldcup.ipynb`** se:

- Cargan los datos históricos generados en el scraping  
- Se crean variables como goles, diferencias, rendimiento histórico, etc.  
- Se entrena un modelo de machine learning (RandomForest, XGBoost, u otro)  
- Se generan predicciones para los partidos del 2026

## Autor
Pool Jinez

## Creditos
Estas prácticas fueron realizadas siguiendo los lineamientos del YouTuber: Frank Andrade / canal: https://www.youtube.com/@thepycoachES
Estas son practicas realizadas para llevar un registro de los códigos utilizados en los proyectos y aprendizaje autodidacta mejorando mis habilidades como 'Data Science'
El valor añadido a este proyecto sera un analisis mas profundo en las predicciones en el Dataset utiliznado varios maodelos y metricas de precision.
