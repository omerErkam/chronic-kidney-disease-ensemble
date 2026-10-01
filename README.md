# Chronic Kidney Disease Prediction Using Machine Learning

## Project Overview
Chronic Kidney Disease (CKD) is a progressive and life-threatening condition often referred to as a "silent killer" due to its lack of early symptoms. Affecting approximately 10% of the global population, early detection is critical to preventing severe outcomes like kidney failure and the need for dialysis. 

This project develops and validates robust machine learning models to predict CKD early using electronic medical records. By accurately classifying patients and assessing their Estimated Glomerular Filtration Rate (eGFR), this tool assists medical professionals in proactive diagnosis and treatment planning.

## Tech Stack & Tools
* **Language:** Python
* **Machine Learning Libraries:** Scikit-learn (Logistic Regression, Decision Tree, Support Vector Machine, BaggingClassifier)
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## Methodology
The pipeline follows a structured machine learning workflow to replicate and evaluate medical research:
1. **Data Preprocessing:** Handled a dataset of 400 instances (250 CKD, 150 NOT_CKD) containing 25 features (11 numerical, 14 categorical) from the UCI Machine Learning Repository.
2. **Data Splitting:** Divided the dataset into an 80% training set and a 20% testing set.
3. **Cross-Validation:** Implemented K-Fold cross-validation (with a fixed random seed of 42) during the training phase to ensure robust model evaluation[cite: 29].
4. **Base Modeling:** Trained three independent classifiers: Logistic Regression (LR), Decision Tree (DT), and Support Vector Machine (SVM).
5. **Ensemble Learning:** Applied a Bagging Ensemble Technique (Bootstrap Aggregation) to the base learners to reduce variance and verify predictive reliability.

## Results & Evaluation
The models were evaluated using Accuracy, Precision, Recall, and F1-score. The Python replication successfully validated the effectiveness of the machine learning algorithms, achieving near-perfect classification on the dataset[cite: 29]. 

### Key Metrics (Replication Results)
* **Logistic Regression (Base & Bagging):** 100.00% Accuracy, 1.00 Precision, 1.00 Recall, 1.00 F-score[cite: 29]
* **Support Vector Machine (Base & Bagging):** 100.00% Accuracy, 1.00 Precision, 1.00 Recall, 1.00 F-score[cite: 29]
* **Decision Tree (Base & Bagging):** 98.75% Accuracy, 0.99 Precision, 0.99 Recall, 0.99 F-score[cite: 29]

*Note: Minor metric variations compared to the original reference paper are due to specific preprocessing steps, hyperparameter defaults in the current Scikit-learn version, and explicit random seed initialization.*
