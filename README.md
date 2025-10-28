
# 📊 Análisis de Rotación de Empleados (HR Employee Attrition)

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![ML](https://img.shields.io/badge/Model-Naive%20Bayes-orange.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)

🌐 Disponible también en inglés: [README_EN.md](README_EN.md)

Este proyecto aplica técnicas de **Machine Learning supervisado** para predecir la **renuncia de empleados (Attrition)** utilizando un dataset clásico de Recursos Humanos.  
El objetivo es identificar los factores más relevantes que influyen en la decisión de renunciar y comparar distintos modelos de clasificación.

---

## 🧰 Stack Tecnológico
- **Lenguaje:** Python 3.11  
- **Librerías:** Pandas, NumPy, Scikit-learn  
- **Visualización:** Matplotlib, Seaborn  
- **Entorno:** Jupyter Notebook  

---

## 🎯 Objetivos del proyecto
- Analizar variables demográficas, laborales y de satisfacción que puedan explicar la rotación del personal.  
- Entrenar y comparar **tres variantes de Naive Bayes**:  
  1. GaussianNB  
  2. BernoulliNB  
  3. MultinomialNB  
- Evaluar el impacto del **desbalance de clases**.

---

## ⚙️ Flujo de trabajo

1. **Carga y exploración de datos (EDA)**  
   - Transformación de variables categóricas.  
   - Visualización de correlaciones y distribuciones asociadas a la renuncia.  

2. **Preparación y modelado**  
   - One-Hot Encoding, separación train/test con estratificación.  
   - Entrenamiento de cada variante probabilística.  

3. **Evaluación y comparación**  
   - Métricas: *accuracy*, *precision*, *recall*, *f1-score*, ROC-AUC.  

---

## 📈 Resultados principales

| Modelo | Accuracy | ROC-AUC | Observación |
|:--|:--:|:--:|:--|
| GaussianNB | ~0.73 | ~0.74 | Mejor desempeño general |
| BernoulliNB | ~0.82 | ~0.72 | Penaliza información no binaria |
| MultinomialNB | ~0.51 | ~0.56 | Poco adecuado para datos no discretos |

---

## 🧠 Conclusiones generales

La comparación entre variantes de **Naive Bayes** evidencia cómo distintos supuestos probabilísticos afectan el desempeño al predecir rotación.  
GaussianNB muestra el mejor equilibrio general, mientras que MultinomialNB resulta menos apropiado para características no basadas en conteo.

Este proyecto demuestra una aproximación rápida, interpretable y reproducible a la predicción de rotación laboral.

---

## ✍️ Autor
**Elías Fernández**  
📧 Contacto: fernandezelias86@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/eliasfernandez208

---
📁 **Repository:** HR_Attrition_NaiveBayes
