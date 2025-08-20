# 📊 Telecom X – Parte 2: Predicción de Cancelación (Churn)

## 🏢 **Acerca del Desafío**

Este proyecto forma parte del **Desafío Telecom X** y consiste en desarrollar **modelos predictivos** que permitan anticipar qué clientes tienen mayor probabilidad de cancelar sus servicios.

Después de un excelente desempeño en el análisis exploratorio de datos (**Parte 1**), ahora asumimos un nuevo reto: **construir un pipeline robusto para la predicción de cancelación (Churn)** utilizando técnicas de **Machine Learning**.

---

## 🎯 **Objetivos del Proyecto**

* ✅ Preparar los datos para modelado (**tratamiento, codificación, normalización**).
* ✅ Analizar la correlación entre variables y seleccionar las más relevantes.
* ✅ Entrenar al menos **dos modelos de clasificación**.
* ✅ Evaluar los modelos mediante métricas (Accuracy, Precision, Recall, F1-score, Matriz de Confusión).
* ✅ Interpretar resultados e identificar **factores clave en la cancelación**.
* ✅ Proponer **estrategias de retención** basadas en los insights.

---

## 🛠 **Tecnologías y Herramientas**

* **Lenguaje:** Python 3
* **Librerías principales:**

  * `pandas` – Manipulación y análisis de datos
  * `numpy` – Cálculos numéricos
  * `matplotlib` / `seaborn` – Visualización
  * `scikit-learn` – Modelado y evaluación
  * `imblearn` – Balanceo de clases (SMOTE, undersampling, oversampling)

---

## 📈 **Pipeline del Proyecto**

### 1. **Carga y Tratamiento de Datos**

* Importación del archivo tratado en la Parte 1 (CSV).
* Eliminación de columnas irrelevantes (ej. `customerID`).
* Revisión de datos faltantes y estandarización.

### 2. **Codificación de Variables Categóricas**

* Aplicación de **One-Hot Encoding** (`pd.get_dummies()` o `OneHotEncoder`).

### 3. **Análisis del Balance de Clases**

* Cálculo de la proporción `Churn vs No Churn`.
* Aplicación de técnicas de **balanceo** (SMOTE, undersampling u oversampling) si es necesario.

### 4. **Normalización o Estandarización**

* Evaluación según los modelos seleccionados:

  * **Modelos sensibles a escala:** Regresión Logística, KNN, SVM
  * **Modelos no sensibles a escala:** Árboles de Decisión, Random Forest

### 5. **Análisis de Correlación y Selección de Variables**

* Visualización de la **matriz de correlación**.
* Identificación de variables más influyentes en `Churn`.

### 6. **Entrenamiento de Modelos**

* División de datos: **70/30** o **80/20** (train/test).
* Entrenamiento de al menos dos modelos:

  * Regresión Logística / KNN (requieren normalización)
  * Random Forest / Árbol de Decisión (no requieren normalización)

### 7. **Evaluación de Modelos**

* Métricas: Accuracy, Precision, Recall, F1-score, Matriz de Confusión.
* Análisis crítico:

  * ¿Cuál modelo tiene mejor desempeño?
  * ¿Existe **overfitting** o **underfitting**?

### 8. **Interpretación e Insights**

* Identificación de **variables más importantes** en la predicción.
* Análisis estratégico:

  * ¿Qué factores influyen más en la cancelación?
  * ¿Qué estrategias de retención pueden implementarse?

---

## 📊 **Métricas Clave a Reportar**

* **Exactitud (Accuracy)**
* **Precisión**
* **Recall (Sensibilidad)**
* **F1-Score**
* **Matriz de Confusión**

---

## 📌 **Resultados Esperados**

* Identificación de **patrones y factores clave** asociados a la cancelación.
* Comparativa entre modelos y elección del más eficiente.
* Propuesta de **estrategias basadas en datos** para reducir el churn.

---

## 🚀 **Próximos Pasos**

* Implementar un pipeline automatizado (ETL + ML).
* Explorar modelos más avanzados (XGBoost, LightGBM).
* Desplegar el modelo en un entorno productivo.

---

## 📚 **Recursos de Apoyo**

* [Documentación oficial de pandas](https://pandas.pydata.org/)
* [Scikit-learn: Guía de Clasificación](https://scikit-learn.org/stable/supervised_learning.html)
* [Artículo sobre codificación categórica – Alura](https://www.alura.com.br)
* [Artículo sobre desbalanceo de clases](https://www.alura.com.br)
* [Normalización y estandarización en ML](https://medium.com)

---

## ✨ **Autor**

Proyecto desarrollado como parte del **Desafío de Machine Learning – Telecom X**.

---
