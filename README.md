# fraud-detection-logistic-vs-tree-vs-perceptron
Colegio de Matemáticas Bourbaki - WA2503 - Machine Learning &amp; AI for the Working Analyst - Examen Modulo I -  Proyecto de aprendizaje supervisado para detección de fraude. Incluye EDA, preparación de datos y comparación de modelos (Perceptrón, Árbol de Decisión y Regresión Logística) aplicados al dataset FraudeCanastas.csv.

# 🧠 Práctica Integrada de Clasificación — Detección de Fraude

Este repositorio contiene la práctica final del módulo de **Aprendizaje Supervisado (Clases 1–13)**, 
centrada en la construcción, entrenamiento y evaluación de modelos de clasificación binaria 
para identificar posibles fraudes en transacciones financieras.

---

## 🎯 Objetivo del proyecto
Desarrollar un modelo de **Machine Learning supervisado** que prediga si una transacción es fraudulenta (1) o no (0), 
siguiendo el flujo completo del proceso de modelado:

1. **Lectura del dataset**
2. **Exploración de datos (EDA)**
3. **Preparación y limpieza de datos**
4. **Elección del modelo**
5. **Entrenamiento y prueba**
6. **Evaluación de resultados**

---

## 🧩 Dataset
**Fuente:** `FraudeCanastas.csv`  
Contiene información sobre compras financiadas y una variable objetivo `fraud_flag` 
que indica si la operación fue fraudulenta (1) o legítima (0).

- **Registros:** 115,988  
- **Variables:** 147  
- **Tasa de fraude:** ~1.4%

---

## ⚙️ Modelos evaluados
| Modelo | Concepto | Tipo |
|:--|:--|:--|
| **Perceptrón** | Clasificador lineal basado en hiperplano | Lineal |
| **Árbol de Decisión (ID3)** | División por ganancia de información (entropía) | No lineal |
| **Regresión Logística** | Clasificación probabilística mediante función sigmoide | Lineal |

---

## 📊 Resultados principales
| Modelo | Precision (clase 1) | Recall (clase 1) | F1-score (clase 1) | Accuracy |
|:--|:--|:--|:--|:--|
| **Regresión Logística** | 0.33 | 0.75 | 0.46 | **0.75** |
| **Perceptrón** | 0.26 | 0.82 | 0.39 | 0.64 |
| **Árbol de Decisión** | 0.27 | 0.72 | 0.39 | 0.69 |

**Conclusión:**  
La **Regresión Logística** fue el modelo con mejor equilibrio entre *precision* y *recall*, 
además de ofrecer interpretabilidad y capacidad probabilística para ajustar umbrales de decisión.

---

## 🧾 Conclusiones generales
- Los tres modelos logran detectar fraudes, pero la **Regresión Logística** se muestra más estable y generalizable.  
- El **Perceptrón** prioriza recall (detecta más fraudes, pero con muchos falsos positivos).  
- El **Árbol de Decisión** es útil para interpretación, pero tiende a sobreajustar.  
- El pipeline propuesto puede ampliarse con técnicas de **regularización**, **tuning** o **ensembles (Random Forest, XGBoost)**.

---

## 🧰 Librerías utilizadas
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn  

---

## 📂 Estructura del repositorio
