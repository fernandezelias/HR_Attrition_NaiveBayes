
# 📊 Employee Attrition Analysis with Naive Bayes (HR Employee Attrition – Naive Bayes)

🇪🇸 También disponible en español: [README.md](README.md)

This project applies different variants of the **Naive Bayes** algorithm to predict **employee attrition** using a classic HR dataset.  
The goal is to compare how distinct probabilistic assumptions impact predictive performance.

---

## 🧰 Tech Stack
- **Language:** Python 3.11  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  

---

## 🎯 Project Objectives
- Explore demographic and work-related factors influencing attrition.
- Train and compare three Naive Bayes variants:
  1. **GaussianNB**
  2. **BernoulliNB**
  3. **MultinomialNB**
- Evaluate the effect of **class imbalance** and analyze class-level metrics.

---

## ⚙️ Workflow

1. **Data Loading and EDA**  
   - Removal of non-informative variables and correlation analysis.
   - Inspection of numerical and categorical distributions.

2. **Preprocessing and Modeling**  
   - One-Hot Encoding and stratified train/test split.
   - Model training under different probabilistic assumptions.

3. **Evaluation and Comparison**  
   - Metrics: *accuracy*, *precision*, *recall*, *f1-score* and *ROC–AUC*.
   - Visualization: normalized confusion matrices and ROC curves.

---

## 📈 Main Results

| Model | Accuracy | Recall (Attrition) | F1 (Attrition) | ROC–AUC |
|:--|:--:|:--:|:--:|:--:|
| GaussianNB | 0.73 | 0.63 | 0.43 | 0.74 |
| BernoulliNB | 0.82 | 0.32 | 0.37 | 0.72 |
| MultinomialNB | 0.51 | 0.61 | 0.28 | 0.56 |

- **GaussianNB** achieves the most balanced performance.
- **BernoulliNB** performs well with binary features but loses sensitivity.
- **MultinomialNB** is less suitable due to the absence of discrete count-based variables.

---

## 🧠 General Conclusions

The results confirm that the **nature of the features** directly affects performance.  
GaussianNB proves to be the most stable variant for mixed-type data, while MultinomialNB shows clear limitations.
This project highlights the comparative value of probabilistic variants and the importance of underlying assumptions.

---

## ✍️ Author
**Elías Fernández**  
📧 Contact: fernandezelias86@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/eliasfernandez208

---

📁 **Repository:** HR_Attrition_NaiveBayes

