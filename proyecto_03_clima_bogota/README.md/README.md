# Pipeline de Datos Climáticos de Bogotá 🌧️

## Descripción
Análisis exploratorio del clima de Bogotá durante 2024 usando datos horarios de la API Open-Meteo. El proyecto cubre extracción, limpieza y visualización de variables como temperatura, precipitación, velocidad del viento y humedad relativa.

## Tecnologías
- Python 3.11
- pandas
- matplotlib
- seaborn
- requests

## Estructura del proyecto
```

proyecto_03_clima_bogota/
├── data/
│   ├── raw/          # Datos crudos de la API (no incluidos en el repo)
│   └── processed/    # Datos procesados y visualizaciones
├── notebooks/
│   ├── 01_extraccion.ipynb
│   ├── 02_limpieza.ipynb
│   └── 03_visualizacion.ipynb
└── README.md
```
## Hallazgos principales

- **Temperatura estable**: Bogotá mantiene una temperatura promedio entre 13°C y 15°C durante todo el año, con una variación anual de apenas 1.5°C. No hay estaciones térmicas.

- **Régimen bimodal de lluvias**: Se identifican dos períodos lluviosos claros — abril-junio (pico en mayo con 223mm) y octubre-noviembre (pico en noviembre con 256mm), consistentes con el comportamiento climático histórico de la sabana de Bogotá.

- **Alta humedad relativa**: La mayoría de las horas del año la humedad supera el 90%, lo que explica la sensación de frío húmedo característica de la ciudad.

## Reproducción del proyecto

1. Clonar el repositorio
2. Instalar dependencias: `pip install -r requirements.txt`
3. Ejecutar los notebooks en orden: `01_extraccion` → `02_limpieza` → `03_visualizacion`

## Fuente de datos
[Open-Meteo Historical Weather API](https://open-meteo.com/en/docs/historical-weather-api) — API gratuita sin clave de acceso requerida.