# Problem Set 2 - Machine Learning
Este repositorio contiene los materiales, scripts y resultados del Problem Set 2 de Machine Learning en la Maestría en Economía de la UNLP. El objetivo principal es predecir la pobreza a nivel de hogares en Colombia utilizando datos del DANE y la Misión para el Empalme de las Series de Empleo, Pobreza y Desigualdad (MESEP). A continuación, se detalla la estructura del repositorio y el flujo de trabajo.

## Estructura del repositorio

```plaintext
Problem_Set_2/
├── document/
│   └── PS2.pdf                 # Informe con la metodología, análisis y resultados
├── scripts/
│   ├── 1_Working_data.ipynb    # Limpieza, transformación y preparación de datos
│   └── 2_analisis.ipynb        # Modelado predictivo y análisis de resultados
├── stores/
│   ├── train_set_final.csv     # Conjunto de datos finales para entrenamiento
│   └── test_set_final.csv      # Conjunto de datos finales para prueba
├── views/
│   ├── *.png                   # Gráficos con análisis descriptivos y resultados de modelos
├── README.md
└── requirements.txt            # Librerías y dependencias necesarias
```
## 1. document
Contiene un archivo PDF (report.pdf) que documenta todo el proceso, incluyendo los objetivos, la metodología y los resultados clave.
Consulta este archivo para obtener un resumen completo del proyecto sin necesidad de ejecutar el código.

## 2. scripts
1_Working_data.ipynb:
Contiene los pasos iniciales de procesamiento y limpieza de datos:

Carga de datos: Lectura y combinación de datasets individuales y de hogares.
Limpieza: Tratamiento de valores faltantes, eliminación de redundancias y estandarización de variables.
Construcción de variables:
Variables binarias 
Indicadores de proporciones relativas como mayoria_infancia y gen_relativo.
Transformaciones logarítmicas de variables de ingresos.
Exportación de datasets finales: train_set_final.csv y test_set_final.csv.

2_analisis.ipynb:
Implementa modelos de predicción del ingreso per cápita y clasificación de hogares pobres:

Análisis Descriptivo:
 - Estadísticas descriptivas y elección de variables.
Modelos Predictivos:
- Regresión Lineal.
- Elastic Net.
- Árboles de Decisión (CART).
- Random Forest.
- Logit (Regresión Logística).
  
Evaluación de Resultados.

## 3. stores
Almacena los conjuntos de datos finales preparados después del preprocesamiento:

train_set_final.csv: Datos de entrenamiento con 34 predictores y la variable objetivo (Ingtot).
test_set_final.csv: Datos de prueba listos para modelado.

## 4. views
Contiene las visualizaciones generadas durante el análisis.

## Cómo usar este repositorio
### Instalar Dependencias

Este proyecto utiliza Python y varias bibliotecas. Instalá las dependencias necesarias con:

```plaintext
pip install -r requirements.txt
```

### Ejecutar los scripts
Abrí los notebooks en Jupyter Lab o Google Colab:
- 1_Working_data.ipynb para preparar los datos.
- 2_analisis.ipynb para el modelado y análisis.
  
Ejecuta las celdas en orden para reproducir los resultados:
- Cargar y procesar los datos.
- Realizar análisis exploratorio.
- Entrenar y evaluar modelos.

### Características principales
- Limpieza y Preparación de Datos
- Análisis Exploratorio
- Modelado Predictivo
- Resultados

### Requisitos
- Python 3.8 o superior
- Librerías:
pandas, 
numpy, 
seaborn, 
matplotlib, 
scikit-learn

### Créditos
Este proyecto fue desarrollado como parte del Problem Set 2 en la materia Machine Learning de la Maestría en Economía de la UNLP, bajo la dirección del profesor Ignacio Sarmiento Barbieri.

