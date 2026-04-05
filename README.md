# Task-11
# Breast Cancer Classification using SVM

## 📌 Project Overview
This project implements a Breast Cancer Classification system using Support Vector Machine (SVM). The model predicts whether a tumor is malignant or benign based on various features extracted from cell nuclei.

---

## 📊 Dataset
- Source: Sklearn Breast Cancer Dataset (`load_breast_cancer()`)
- Total Samples: 569
- Features: 30 numerical features
- Classes:
  - 0 → Malignant
  - 1 → Benign

---

## 🛠 Tools & Technologies
- Python
- Scikit-learn
- NumPy
- Matplotlib

---

## ⚙️ Steps Performed

1. Loaded dataset and explored feature distribution
2. Applied feature scaling using StandardScaler
3. Split dataset into training and testing sets
4. Trained SVM with Linear Kernel
5. Trained SVM with RBF Kernel
6. Tuned hyperparameters using GridSearchCV
7. Evaluated model using:
   - Accuracy
   - Confusion Matrix
   - Classification Report
8. Plotted ROC Curve and calculated AUC score
9. Saved final model pipeline (Scaler + SVM)

---

## 📈 Results

| Model              | Accuracy |
|-------------------|---------|
| SVM (Linear)      | ~96%    |
| SVM (RBF)         | ~97–98% |
| Tuned SVM (Best)  | ~98%    |

- Best performance achieved using **RBF kernel with tuned parameters**

---

## 🔍 Key Insights
- SVM performs well for binary classification problems
- Feature scaling is critical for SVM performance
- RBF kernel captures non-linear relationships better
- Hyperparameter tuning improves accuracy significantly

---

## 📊 Outputs
- Confusion Matrix
- Classification Report
- ROC Curve
- AUC Score
- Saved Model (.pkl)

---

## 🚀 How to Run

1. Install dependencies:
   pip install numpy matplotlib scikit-learn

2. Run the notebook:
   jupyter notebook

---

## 💾 Model Saving
The trained model pipeline is saved using:
joblib.dump(model, 'svm_breast_cancer.pkl')

---

## 📌 Future Improvements
- Use cross-validation for better generalization
- Try different kernels (Polynomial)
- Deploy model using Flask/Streamlit

---

## 👨‍💻 Author
Navya Mahamkali
