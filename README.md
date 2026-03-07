# 🤖 TelecomX LATAM — Predicción de Cancelación de Clientes (Churn)

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter)
![sklearn](https://img.shields.io/badge/scikit--learn-ML-green?style=flat-square&logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Completado-brightgreen?style=flat-square)

## 📋 Descripción

Este proyecto forma parte del **Challenge de Data Science — TelecomX LATAM**.  
A partir de datos reales de clientes, se construyó un pipeline completo de análisis y predicción de cancelación (churn), combinando un Análisis Exploratorio de Datos (EDA) con modelos de Machine Learning.

> **Tasa de cancelación detectada: 26.5%** sobre una base de 7,032 clientes analizados.

---

## 🗂️ Estructura del Repositorio

```
telecomx-challenge-part2/
│
├── 📁 notebooks/
│   └── telecomx_challenge_part2.ipynb
│
├── 📁 data/
│   └── TelecomX_Data.json
│
├── 📁 images/
│   └── (14 visualizaciones generadas)
│
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🗺️ Estructura del Notebook

| # | Sección | Descripción |
|---|---|---|
| 1 | 📥 Extracción y Limpieza | Pipeline ETL completo desde JSON |
| 2 | 🛠️ Preparación para ML | Encoding, SMOTE, normalización |
| 3 | 📊 Contexto Visual — EDA | 10 visualizaciones exploratorias |
| 4 | 🎯 Correlación y Selección | Matriz de correlación y análisis dirigido |
| 5 | 🤖 Modelado Predictivo | Regresión Logística + Random Forest |
| 6 | 📋 Evaluación | Métricas, matrices de confusión, curvas ROC |
| 7 | 🔍 Interpretación | Importancia de variables por modelo |
| 8 | 📄 Conclusión Estratégica | Hallazgos y recomendaciones de negocio |

---

## 📊 Análisis Exploratorio (EDA)

### Distribución de la Variable Objetivo
![Distribución Churn](images/01_distribucion_churn.png)

### Tasa de Churn por Variables Categóricas
![Variables Categóricas](images/02_churn_variables_categoricas.png)

### Tasa de Churn por Tipo de Contrato
![Tipo de Contrato](images/03_churn_tipo_contrato.png)

### Distribución de Variables Numéricas por Churn
![Distribución Numéricas](images/04_distribucion_numericas_churn.png)

### Boxplot de Variables Numéricas por Churn
![Boxplot](images/05_boxplot_numericas_churn.png)

### Tasa de Churn por Grupo de Antigüedad
![Antigüedad](images/06_churn_grupo_antiguedad.png)

### Tasa de Churn por Rango de Cargo Mensual
![Cargo Mensual](images/07_churn_cargo_mensual.png)

### Tasa de Churn por Rango de Cargo Total
![Cargo Total](images/08_churn_cargo_total.png)

### Cargo Mensual vs Antigüedad por Churn
![Scatter](images/09_scatter_cargo_antiguedad.png)

### Matriz de Correlación con Churn
![Correlación](images/10_matriz_correlacion.png)

---

## 🤖 Modelado Predictivo

### Matrices de Confusión
![Matrices de Confusión](images/11_matrices_confusion.png)

### Curvas ROC — Comparación de Modelos
![Curvas ROC](images/12_curvas_roc.png)

### Top 15 Variables — Regresión Logística
![Regresión Logística](images/13_top15_regresion_logistica.png)

### Top 15 Variables — Random Forest
![Random Forest](images/14_top15_random_forest.png)

---

## 📈 Resultados de los Modelos

| Modelo | ROC-AUC | Requiere Normalización |
|---|---|---|
| Regresión Logística | ~0.84 | ✅ Sí |
| Random Forest | ~0.87 | ❌ No |

> **Random Forest** obtuvo el mejor desempeño con mayor AUC y mejor detección de la clase minoritaria.

---

## 🔴 Principales Factores de Cancelación

| # | Factor | Impacto |
|---|---|---|
| 1 | Contrato mes a mes | ~42.7% de cancelación |
| 2 | Primeros 12 meses | ~48% de clientes nuevos cancela |
| 3 | Cargo mensual elevado | Promedio $74.44 vs $61.27 |
| 4 | Fibra óptica | ~42% de cancelación |
| 5 | Cheque electrónico | ~45% de cancelación |

---

## 💡 Recomendaciones Estratégicas

| # | Acción | Impacto |
|---|---|---|
| 1 | Incentivar contratos anuales/bianuales con descuentos | 🔴 Alto |
| 2 | Programa de onboarding intensivo primeros 12 meses | 🔴 Alto |
| 3 | Revisar calidad del servicio de Fibra Óptica | 🟠 Medio |
| 4 | Migrar clientes de cheque electrónico a débito automático | 🟠 Medio |
| 5 | Implementar modelo Random Forest para alertas tempranas | 🔴 Alto |

---

## 🛠️ Tecnologías Utilizadas

- **Python 3.10**
- **Pandas / NumPy** — manipulación de datos
- **Matplotlib / Seaborn** — visualizaciones
- **Scikit-learn** — modelos de ML y métricas
- **Imbalanced-learn** — balanceo con SMOTE
- **Google Colab** — entorno de ejecución

---

## 🚀 Cómo Ejecutar

1. Abre el notebook en Google Colab:  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JeaLPaHu/telecomx-challenge-part2/blob/main/notebooks/telecomx_challenge_part2.ipynb)

2. Ejecuta `Runtime → Run all`

3. Las 14 imágenes se descargarán automáticamente

---

## 👤 Autor

**JeaLPaHu**  
[![GitHub](https://img.shields.io/badge/GitHub-JeaLPaHu-black?style=flat-square&logo=github)](https://github.com/JeaLPaHu)

---

*Challenge Data Science — TelecomX LATAM* 🚀
