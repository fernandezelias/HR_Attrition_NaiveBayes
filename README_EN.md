
# 📊 Employee Attrition Analysis (HR Employee Attrition)

🌐 Disponible en [Español](README.md)

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![ML](https://img.shields.io/badge/Model-Naive%20Bayes-orange.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)

This project applies **supervised Machine Learning** techniques to predict **employee attrition** using a classic HR dataset.  
The goal is to identify relevant factors associated with voluntary resignation and compare different probabilistic classifiers.

---

## 🧰 Tech Stack
- **Language:** Python 3.11  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  

---

## 🎯 Project Objectives
- Analyze demographic, job-related, and satisfaction variables related to attrition.  
- Train and compare **three Naive Bayes variants**:  
  1. GaussianNB  
  2. BernoulliNB  
  3. MultinomialNB  
- Evaluate the impact of **class imbalance** in binary classification.

---

## ⚙️ Workflow

1. **Data Exploration (EDA)**  
   - Transformation of categorical variables.  
   - Correlation and distribution analysis linked to attrition.  

2. **Preprocessing and Modeling**  
   - One-Hot Encoding and stratified train/test split.  
   - Training of probabilistic classifiers.  

3. **Evaluation and Comparison**  
   - Metrics: *accuracy*, *precision*, *recall*, *f1-score*, ROC-AUC.  

---

## 📈 Main Results

| Model | Accuracy | ROC-AUC | Observation |
|:--|:--:|:--:|:--|
| GaussianNB | ~0.73 | ~0.74 | Best overall performance |
| BernoulliNB | ~0.82 | ~0.72 | Penalized by binary simplification |
| MultinomialNB | ~0.51 | ~0.56 | Not ideal for non-count features |

---

## 🧾 General Conclusions

GaussianNB presents the best trade-off between performance and interpretability.  
MultinomialNB performs poorly due to the lack of word-frequency-style features, while BernoulliNB loses relevant information by binarizing inputs.

Overall, Naive Bayes proves to be a **fast, interpretable, and competitive baseline** for employee attrition prediction.

---

## 🪪 License
This project is distributed under the MIT License.  
See the [LICENSE](LICENSE) file.

---

## ✍️ Author
**Elías Fernández**

---

## 📫 Contact
📧 [fernandezelias86@gmail.com](mailto:fernandezelias86@gmail.com)  
🔗 LinkedIn: [Profile](https://www.linkedin.com/in/eliasfernandez208)
