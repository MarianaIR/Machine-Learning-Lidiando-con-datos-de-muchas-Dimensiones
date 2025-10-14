# 📉 MACHINE LEARNING: LIDIANDO CON DATOS DE MUCHAS DIMENSIONES

[![Python](https://img.shields.io/badge/Python-3670A0?style=flat&logo=python&logoColor=ffdd54)](https://www.python.org/)  
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)  
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)  
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)

Este proyecto aborda la problemática de la **Alta Dimensionalidad** en Machine Learning, donde un dataset posee un gran número de *features* (columnas). El objetivo es aplicar y comprender la técnica de **Reducción de Dimensionalidad** para transformar los datos a un espacio dimensional menor, manteniendo las propiedades originales esenciales, lo que se conoce como **Dimensión Intrínseca**.

---

## 🧠 Contenido del Proyecto

### 1️⃣ El Problema de la Alta Dimensionalidad
- **Contexto:** Se utiliza un dataset ficticio llamado `aluracare.csv` (adaptado de un dataset real de cáncer de mama de Kaggle) que contiene muchas características o dimensiones.
- **La Maldición de la Dimensionalidad:** Cuando el número de *features* es muy grande, los modelos de Machine Learning pueden volverse ineficientes, lentos e incluso propensos al sobreajuste (*overfitting*). Reducir la dimensionalidad es clave para mejorar el rendimiento.

### 2️⃣ Estrategias de Reducción de Dimensionalidad
El *notebook* explora diversas técnicas para lidiar con el alto número de dimensiones:

#### A. Selección de Features (Filtrado)
- Se utiliza el clasificador **Random Forest** para calcular la **Importancia de las Variables**.
- El objetivo es **filtrar** y quedarnos solo con las variables que tienen un mayor poder predictivo sobre la etiqueta de salida.

#### B. Extracción de Features (PCA)
- **Análisis de Componentes Principales (PCA):** Es la técnica principal de extracción.
- **Mecánica:** PCA identifica los ejes (componentes principales) que capturan la mayor varianza de los datos. Permite proyectar el dataset original en un nuevo subespacio con menos dimensiones.
- **Ventaja:** Permite pasar, por ejemplo, de 10 *features* a solo 2 o 3, simplificando el modelo sin perder información crucial.

### 3️⃣ Aplicación Práctica con SKLearn
- Se utilizan las utilidades de **Scikit-learn** para implementar tanto la Selección de Features como las transformaciones de **PCA**.
- La reducción de dimensionalidad es un paso fundamental en el **Preprocesamiento de Datos** para garantizar que el modelo de Machine Learning final sea eficiente, interpretable y generalice mejor.

---

## 🛠️ Librerías Utilizadas

| Librería       | Uso principal                               |
|----------------|---------------------------------------------|
| **Scikit-learn**| Implementación de PCA y modelos para determinar la Importancia de Variables|
| **Pandas**     | Carga y manipulación del dataset (`aluracare.csv`)|
| **NumPy**      | Operaciones numéricas subyacentes (inferido) |

---

## 🎯 Objetivo del Proyecto
Capacitar al usuario para identificar y resolver el problema de la **Alta Dimensionalidad** en Data Science. El proyecto enseña las diferencias y aplicaciones prácticas de la **Selección de Features** y la **Extracción de Features (PCA)**, permitiendo construir modelos de Machine Learning más robustos, rápidos y precisos.

---

## 📈 Resultados Clave
- Se demuestra cómo el **Análisis de Componentes Principales (PCA)** transforma un dataset complejo a una representación bidimensional o tridimensional más simple.
- Se identifica la **Dimensión Intrínseca** del dataset, es decir, el número óptimo de *features* necesarias para representar la información de manera eficiente.
- El proceso resulta en un conjunto de datos preprocesado y optimizado, listo para ser utilizado en cualquier modelo predictivo con menor riesgo de sobreajuste.

