# 📊 Predicción de Impago de Créditos con Machine Learning

Este proyecto tiene como objetivo construir un pipeline end-to-end para predecir el riesgo de impago de clientes de tarjetas de crédito.  

Se utilizan técnicas de análisis exploratorio, Machine Learning, y consultas SQL sobre el dataset **UCI Credit Card**.

---

## 🚀 Tecnologías utilizadas
- Python (Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn)
- SQL (SQLite)
- Google Colab (entorno de trabajo)

---

## 📂 Dataset
**Fuente:** [UCI Credit Card Dataset (Kaggle)](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset)  
Contiene información de **30.000 clientes**, con variables demográficas, historial de pagos y la variable objetivo:  
- `default.payment.next.month`: 1 = impago, 0 = pagó.

---

## 📌 Flujo del proyecto
1. **Carga y limpieza de datos**
   - Revisión de nulos (no fue necesaria imputación).
   - Renombrado de columnas y tipificación.

2. **Análisis exploratorio (EDA)**
   - Matriz de correlación.
   - Distribuciones de variables relevantes.

3. **Feature Engineering**
   - Preparación de variables predictoras.
   - División en train/test.

4. **Modelado**
   - Logistic Regression.
   - Random Forest.
   - XGBoost.
   - Evaluación con métricas de clasificación y curvas ROC.

5. **SQL**
   - Creación de base de datos SQLite en memoria.
   - Ejecución de consultas analíticas (ej. distribución de clientes por sexo y estado civil, % de impagos).

---

## 📈 Resultados principales
- **Random Forest y XGBoost** obtuvieron el mejor rendimiento con un **AUC ≈ 0.76–0.77**.  
- **Logistic Regression** quedó por debajo con AUC ≈ 0.71.  
- Todos los modelos muestran buena precisión para clientes que pagan, pero menor recall en detectar impagos.  
- Se identifica la necesidad de técnicas de balanceo de clases o enriquecimiento de variables.

---

##
