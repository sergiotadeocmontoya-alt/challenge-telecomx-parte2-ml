# Telecom X — Predicción de Cancelación (Churn) | Challenge (Parte 2)

Este proyecto desarrolla un flujo básico de **Machine Learning** para predecir la **cancelación de clientes (Churn)** en **Telecom X**.  
La meta es identificar clientes con mayor probabilidad de cancelar para proponer acciones de retención.

---

## Objetivo
- Preparar datos (limpieza previa, selección de columnas relevantes, codificación y escalado según el modelo).
- Analizar desbalance de clases.
- Entrenar **dos modelos** de clasificación:
  - **Regresión Logística** (requiere estandarización)
  - **Random Forest** (no requiere estandarización)
- Evaluar el rendimiento con métricas:
  - Accuracy, Precision, Recall, F1-score y Matriz de confusión.
- Generar un **informe final** con hallazgos y recomendaciones.

---

## Dataset
Se utiliza un archivo ya tratado en la Parte 1 del challenge:

- `datos_tratados_TelecomXParte2.csv`

Incluye variables como:
- Demografía: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- Servicios: `PhoneService`, `InternetService`, `OnlineSecurity`, etc.
- Contrato/pago: `Contract`, `PaymentMethod`, `PaperlessBilling`
- Cargos: `Charges.Monthly`, `Charges.Total`
- Variable objetivo: `Churn` (0 = no cancela, 1 = cancela)

---

## Tecnologías y librerías
- Python 3
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- imbalanced-learn

---

## Cómo ejecutar el proyecto (Google Colab)
1. Abre el notebook en Google Colab.
2. Sube el archivo `datos_tratados_TelecomXParte2.csv` al entorno (panel izquierdo → Files → Upload).
3. Ejecuta las celdas en orden.

Ejemplo de carga:
```python
import pandas as pd
df = pd.read_csv("/content/datos_tratados_TelecomXParte2.csv")
df.head()
