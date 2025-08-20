# Reto Alura Telecom X 2

# 📊 Proyecto de Predicción de Churn con Machine Learning

Este proyecto implementa un modelo de **Machine Learning** para predecir la probabilidad de **Churn (abandono de clientes)** en una base de datos de telecomunicaciones. El flujo de trabajo incluye:

* Preprocesamiento de datos (Obtiene datos de csv ya procesado en reto TelecomX 1).
* Balanceo de clases con **SMOTE**.
* Entrenamiento de distintos modelos (Regresión Logística, Random Forest, SVM, etc.).
* Evaluación con métricas de rendimiento.
* Interpretación de variables influyentes.

---

## 🚀 Cómo usarlo

### 1. Clonar el repositorio (si estás en GitHub)

```bash
git clone https://github.com/tu_usuario/proyecto_churn.git
cd proyecto_churn
```

### 2. Abrir en Google Colab

* Sube el archivo `.ipynb` a **Google Colaboratory**.
* Conéctate a un entorno de ejecución con GPU/TPU si deseas acelerar entrenamientos pesados.

### 3. Instalar dependencias

Ejecuta la siguiente celda al inicio del notebook:

```python
!pip install scikit-learn imbalanced-learn matplotlib seaborn pandas numpy
```

### 4. Preparar los datos

Asegúrate de que el archivo de datos (ejemplo: `churn.csv`) esté en la misma carpeta del notebook o súbelo a Colab.

Ejemplo de carga de datos:

```python
import pandas as pd
datos = pd.read_csv("churn.csv")
```

### 5. Entrenar modelos

El notebook ya contiene bloques para:

* Escalado y normalización de datos.
* Aplicar **SMOTE** para balanceo.
* Entrenar modelos como:

  * Regresión Logística.
  * Random Forest.
  * Support Vector Machine (SVM).

### 6. Evaluación

Los modelos se evalúan con métricas como:

* **Accuracy**
* **Precisión**
* **Recall**
* **F1-score**
* **ROC-AUC**

### 7. Interpretación de Resultados

Se incluyen gráficos de:

* Importancia de variables en modelos lineales.
* Importancia de características en Random Forest.
* Matriz de confusión.
* Curva ROC.

---

## 📂 Estructura de Archivos

```
proyecto_churn/
│── churn.csv              # Dataset (ejemplo)
│── churn_notebook.ipynb   # Notebook principal con el flujo completo
│── README.md              # Este archivo
```

---

## ✨ Mejoras Futuras

* Optimización con **GridSearchCV** o **RandomizedSearchCV**.
* Uso de **XGBoost** o **LightGBM**.
* Implementación de interpretabilidad con **SHAP** o **LIME**.
* Creación de API para exponer el modelo.

---

¿Quieres que lo adapte a un **README más orientado a GitHub** (con ejemplos de ejecución desde consola y badges) 📌 o prefieres que quede enfocado **sólo para Colab**?
