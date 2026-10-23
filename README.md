# Proyecto final — Programación Analítica II

## Arroyo Capital: inversión y portafolio en la industria del cine

Proyecto final de **Vicente Alvarez** para la Licenciatura en Ciencia de Datos para Negocios de la Universidad de Montevideo.

El objetivo es analizar películas estrenadas entre 1980 y 2020 y construir una propuesta para distribuir **USD 500 millones** entre distintos tipos de producciones cinematográficas.

## Contenido del análisis

El notebook desarrolla las cinco etapas del proyecto:

1. Análisis exploratorio, limpieza y justificación de las correcciones.
2. Ajuste de presupuesto y recaudación por inflación.
3. Análisis de retorno, riesgo, géneros y puntuación IMDb.
4. Visualizaciones estáticas e interactivas.
5. Tesis de inversión y simulación del portafolio.

## Resultados principales

- La base limpia contiene 7.668 películas.
- El análisis financiero utiliza 5.389 películas con presupuesto y recaudación disponibles.
- Terror y Animación presentan los mejores resultados históricos entre los géneros con una cantidad representativa de observaciones.
- La propuesta distribuye los USD 500 millones entre 21 proyectos de cuatro segmentos.
- En 10.000 simulaciones, el retorno mediano estimado del portafolio fue 92,97 % durante los tres años.
- La probabilidad simulada de terminar con menos capital que el inicial fue 0,71 %.

Los resultados de la simulación utilizan información histórica y supuestos simplificadores. No representan una garantía de rendimiento futuro.

## Estructura del repositorio

```text
programacion-analitica-2-portafolio-cine-alvarez/
├── README.md
├── requirements.txt
├── .gitignore
├── datos/
│   ├── peliculas.csv
│   └── ipc_eeuu.csv
├── notebooks/
│   └── analisis.ipynb
└── salidas/
    └── riesgo_retorno_segmentos.html
```

## Cómo ejecutar el proyecto

Desde una terminal abierta en la carpeta del proyecto:

```powershell
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook notebooks/analisis.ipynb
```

Luego se debe seleccionar el kernel de `.venv` y ejecutar todas las celdas en orden.

## Herramientas utilizadas

- Python
- pandas y NumPy
- Matplotlib
- Plotly
- Jupyter Notebook

El código utiliza principalmente las herramientas trabajadas en Programación Analítica II y mantiene explicaciones junto a cada decisión y visualización.
