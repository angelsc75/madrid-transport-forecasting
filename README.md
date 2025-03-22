# madrid-transport-forecasting
Comparación de varios modelos en la predicción del tráfico de Madrid (práctica de series temporales)
madrid-transport-forecasting/
│
├── data/
│   ├── raw/
│   │   ├── CRTM_Evolucion_demanda_diaria.xlsx    # Datos originales de transporte
│   │   └── madrid_weather_data.csv               # Datos meteorológicos de Madrid
│   │
│   └── processed/
│       ├── transport_data_cleaned.csv            # Datos de transporte procesados
│       ├── weather_data_cleaned.csv              # Datos meteorológicos procesados
│       └── combined_dataset.csv                  # Dataset combinado (transporte + clima)
│
├── notebooks/
│   ├── 1_exploratory_data_analysis.ipynb         # Análisis exploratorio (incluye tu dashboard)
│   ├── 2_baseline_models.ipynb                   # Modelos ingenuos/baseline
│   ├── 3_linear_models.ipynb                     # Modelos lineales y VAR
│   ├── 4_simple_neural_networks.ipynb            # Redes neuronales simples
│   ├── 5_deep_neural_networks.ipynb              # Redes neuronales profundas
│   ├── 6_arima_models.ipynb                      # Modelos ARIMA/SARIMA
│   └── 7_comparative_analysis.ipynb              # Comparativa de todos los modelos
│
├── src/
│   ├── data/
│   │   ├── __init__.py
│   │   ├── make_dataset.py                       # Scripts para procesar datos
│   │   └── feature_engineering.py                # Creación de características
│   │
│   ├── models/
│   │   ├── __init__.py
│   │   ├── naive.py                              # Implementación de modelos ingenuos
│   │   ├── linear.py                             # Implementación de modelos lineales
│   │   ├── neural_networks.py                    # Implementación de redes neuronales
│   │   └── arima.py                              # Implementación de modelos ARIMA
│   │
│   ├── visualization/
│   │   ├── __init__.py
│   │   └── visualize.py                          # Funciones para visualización
│   │
│   └── evaluation/
│       ├── __init__.py
│       └── metrics.py                            # Funciones de evaluación (RMSE, MAPE, etc.)
│
├── results/
│   ├── figures/                                  # Gráficos para el artículo
│   ├── model_comparisons/                        # Tablas y datos de comparación
│   └── predictions/                              # Predicciones guardadas de cada modelo
│
├── docs/
│   ├── article/                                  # Borradores y archivos del artículo
│   └── references/                               # Referencias y documentación externa
│
├── requirements.txt                              # Dependencias del proyecto
├── README.md                                     # Documentación general
└── .gitignore                                    # Archivos a ignorar por git