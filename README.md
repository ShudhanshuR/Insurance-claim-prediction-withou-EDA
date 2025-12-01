📌 Project Overview

This project was provided by Datamites as part of the Data Scientist Certification program.
The key rule for this assignment was not to perform any Exploratory Data Analysis (EDA).
The task was to directly build a machine learning model and evaluate its performance on a highly imbalanced insurance claim dataset.

The goal is to predict whether a customer will make an insurance claim or not using only raw data and model-driven learning.

📂 Project Constraints (Important)

EDA strictly not allowed

No feature exploration

No feature engineering

No data visualization

Must work with missing values (-1)

Must train directly on raw dataset

These conditions simulate a real corporate scenario where analysts get restricted or anonymous datasets.

⚙️ Methods Used

LightGBM Classifier (best for missing values + fast + handles imbalance)

Stratified Train–Test Split

Class Weighting to fight imbalance

Validation Split for Early Stopping

Multiple Evaluation Metrics to understand imbalance performance

📊 Model Performance

Because the dataset is extremely imbalanced and EDA was not allowed, performance is naturally limited.

Final Test Results:

Metric	Score
ROC AUC	Low (due to imbalance)
PR AUC	Very Low
Accuracy	Moderate (but misleading)
Precision	Low
Recall	Moderate
F1 Score	Low
MCC Score	Low

Confusion Matrix Summary:

High True Negatives

High False Positives

Claims are very hard to detect because the model sees very few positive examples

This outcome is expected for highly imbalanced data without EDA or feature engineering.

📝 Conclusion

This project shows the challenges of working with imbalanced real-world datasets under restricted conditions. Since EDA was not allowed, it was not possible to understand the data, remove noise, create new features, or balance classes properly.

Even after using LightGBM, class balancing, and validation-based early stopping:

The model still struggles to catch claim cases

Metrics like ROC AUC and PR AUC remain low

The imbalance heavily reduces model learning capability

Still, the project successfully demonstrates:

Handling missing values with LightGBM

Managing imbalance using class weights

Impact of restricted EDA environments

Importance of AUC over accuracy in imbalanced problems

This aligns exactly with the learning goals of the Datamites assignment.

⚠️ Project Risks

1.Severe Class Imbalance reduces model learning capability.

2.No EDA means zero understanding of data distribution.

3.Unknown Feature Meaning restricts interpretability.

4.High False Positives & False Negatives risk in real deployment.

5.Risk of Overfitting due to imbalance.

6.Weak generalization on new or unseen datasets.


🚀 Technologies Used

# Python

# Pandas

# NumPy

# LightGBM

# Scikit-Learn

📞 Author

This project was completed by Shudhanshu Ranjan as part of the Datamites Certified Data Scientist Program.
