
# 📊 Análisis de Rotación de Empleados con Naive Bayes (HR Employee Attrition – Naive Bayes)

🌐 Disponible también en inglés: [README_EN.md](README_EN.md)

Este proyecto aplica variantes del algoritmo **Naive Bayes** para predecir la **renuncia de empleados (Attrition)** utilizando un dataset clásico de Recursos Humanos.  
El objetivo principal es comparar cómo diferentes supuestos probabilísticos afectan la capacidad predictiva del modelo.

---

## 🧰 Stack Tecnológico
- **Lenguaje:** Python 3.11  
- **Librerías:** Pandas, NumPy, Scikit-learn  
- **Visualización:** Matplotlib, Seaborn  
- **Entorno:** Jupyter Notebook  

---

## 🎯 Objetivos del proyecto
- Explorar factores demográficos y laborales asociados a la rotación de empleados.
- Entrenar y comparar tres variantes de Naive Bayes:
  1. **GaussianNB**
  2. **BernoulliNB**
  3. **MultinomialNB**
- Evaluar el impacto del **desbalance de clases** y analizar las métricas clave por clase.

---

## ⚙️ Flujo de trabajo

1. **Carga y exploración de datos (EDA)**  
   - Eliminación de variables no informativas y análisis de correlaciones.
   - Segmentación de atributos numéricos y categóricos.

2. **Preparación y modelado**  
   - Codificación mediante *One-Hot Encoding* y división estratificada de datos.
   - Entrenamiento de modelos bajo supuestos probabilísticos diferentes.

3. **Evaluación y comparación**  
   - Métricas utilizadas: *accuracy*, *precision*, *recall*, *f1-score* y *ROC–AUC*.
   - Visualización de matrices de confusión normalizadas y curvas ROC.

---

## 📈 Resultados principales

| Modelo | Accuracy | Recall (Renuncia) | F1 (Renuncia) | ROC–AUC |
|:--|:--:|:--:|:--:|:--:|
| GaussianNB | 0.73 | 0.63 | 0.43 | 0.74 |
| BernoulliNB | 0.82 | 0.32 | 0.37 | 0.72 |
| MultinomialNB | 0.51 | 0.61 | 0.28 | 0.56 |

- **GaussianNB** logra el mejor equilibrio general.
- **BernoulliNB** ofrece buen desempeño con binarización, pero pierde sensibilidad.
- **MultinomialNB** resulta menos adecuado al no existir variables basadas en conteos.

---

## 🧠 Conclusiones generales

Los resultados confirman que la **naturaleza de las variables** influye directamente en el rendimiento del modelo.  
GaussianNB demuestra ser la opción más estable para este dataset mixto, mientras que MultinomialNB exhibe limitaciones claras.
Este proyecto ilustra el valor comparativo de variantes probabilísticas y la importancia de suposiciones matemáticas.

---

## ✍️ Autor
**Elías Fernández**  
📧 Contacto: fernandezelias86@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/eliasfernandez208

---

📁 **Repositorio:** HR_Attrition_NaiveBayes

