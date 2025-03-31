# 🎓 Predicting Student Dropout Using XGBoost & Neural Networks

This project was developed as part of the **Data Science Career Accelerator** (University of Cambridge) to predict student dropout risk using **supervised machine learning** and **deep learning** approaches. The model is designed to support universities and educational providers in identifying at-risk students early, enabling targeted interventions to improve retention and learning outcomes.

---

## 🎯 Project Objective

To build predictive models that can accurately classify students who are at risk of dropping out, using key features such as academic performance, attendance records, demographics, and institutional data.

---

## 🧠 Models Used

- ✅ **XGBoost**
- ✅ **Neural Networks (Keras)**
- SMOTE for handling class imbalance
- Grid Search CV for hyperparameter tuning

---

## 🧪 Features Included

- **Academic**: Credit Weighted Average  
- **Attendance**: Attendance %, Contact Hours, Unauthorised Absences  
- **Demographics**: Gender, Age  
- **Institutional**: Study Centre, Course Level, Progression Status  

---

## 📈 Key Findings

- **XGBoost + attendance features** outperformed all models with an AUC-ROC of **0.9863** and balanced accuracy of **0.9523**
- **CreditWeightedAverage** was the most predictive feature (57% importance)
- Adding **AttendancePercentage** and **ContactHours** significantly improved model performance
- **Neural Network** showed high precision (0.9968) and generalised well with strong true negative rate

---

## 📊 Visualizations Included

- ROC curves, confusion matrices
- Feature importance plots
- EDA: dropout distribution, attendance patterns, demographics, centre-level performance

---

## 🛠️ Tools & Libraries

- Python, Pandas, NumPy
- XGBoost, Keras, Scikit-learn
- Matplotlib, Seaborn
- SMOTE for class imbalance

---

## 📎 Acknowledgments

This mini-project was developed as part of the **University of Cambridge x FourthRev** Data Science Career Accelerator (2024 cohort).
