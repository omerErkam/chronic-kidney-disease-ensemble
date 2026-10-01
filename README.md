# Chronic Kidney Disease Prediction Using Machine Learning

## Project Overview
Chronic Kidney Disease (CKD) is a progressive and life-threatening condition often referred to as a "silent killer" due to its lack of early symptoms[cite: 1, 3]. Affecting approximately 10% of the global population, early detection is critical to preventing severe outcomes like kidney failure and the need for dialysis[cite: 1, 3]. 

This project develops and validates robust machine learning models to predict CKD early using electronic medical records[cite: 1, 3]. By accurately classifying patients and assessing their Estimated Glomerular Filtration Rate (eGFR), this tool assists medical professionals in proactive diagnosis and treatment planning[cite: 1, 3].

## Tech Stack & Tools
* **Language:** Python[cite: 2, 3]
* **Machine Learning Libraries:** Scikit-learn (Logistic Regression, Decision Tree, Support Vector Machine, BaggingClassifier)[cite: 1, 3]
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn (used for Boxplots and Confusion Matrices)[cite: 1, 3]
* **Environment:** Jupyter Notebook

## Methodology
The pipeline follows a structured machine learning workflow:
1. **Data Preprocessing:** Handled a dataset of 400 instances (250 CKD, 150 NOT_CKD) containing 25 features (11 numerical, 14 categorical) from the UCI Machine Learning Repository[cite: 1, 3].
2. **Data Splitting:** Divided the dataset into an 80% training set and a 20% testing set[cite: 1, 3].
3. **Cross-Validation:** Implemented 10-fold cross-validation during the training phase to ensure robust model evaluation[cite: 1, 3].
4. **Base Modeling:** Trained three independent classifiers: Logistic Regression (LR), Decision Tree (DT), and Support Vector Machine (SVM)[cite: 1, 3].
5. **Ensemble Learning:** Applied a Bagging Ensemble Technique (Bootstrap Aggregation) to the base learners to reduce variance and improve predictive reliability[cite: 1, 3].

## Results & Evaluation
The models were evaluated using Accuracy, Precision, Recall, and F1-score[cite: 1, 3]. The **Decision Tree coupled with the Bagging Ensemble** proved to be the most robust architecture, outperforming previous literature benchmarks[cite: 1, 3].

### Key Metrics
* **Decision Tree (Base):** 95.92% Accuracy, 0.99 Precision, 0.98 Recall, 0.98 F1-score[cite: 1, 3]
* **Decision Tree + Bagging (Final Model):** **97.23% Accuracy**[cite: 1, 3]
* **SVM + Bagging:** 95.70% Accuracy[cite: 1, 3]
* **Logistic Regression + Bagging:** 94.53% Accuracy[cite: 1, 3]
