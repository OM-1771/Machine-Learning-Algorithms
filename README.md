📌 Here I Provide All the  Machine Learning Algorithms

This repository contains implementations of All Important  Machine Learning algorithms with clear examples and datasets.
Lets Start :

1️⃣ Simple Linear Regression

Implemented Simple Linear Regression using a Height vs Weight dataset.

Objective: Predict Weight based on Height.

Type: Regression

2️⃣ Multiple Linear Regression

Implemented Multiple Linear Regression using multiple input features.

Objective: Predict a continuous target variable using more than one independent variable.

Type: Regression

3️⃣ Logistic Regression

Implemented Logistic Regression for binary classification problems.

Objective: Predict class labels (0/1) using probability-based classification.

Type: Classification

4️⃣ Ridge Regression

Implemented Ridge Regression (L2 Regularization) to reduce overfitting.

Objective: Improve model performance by penalizing large coefficients.

Type: Regression (Regularized)

5️⃣ Lasso Regression

Implemented Lasso Regression (L1 Regularization) for feature selection and overfitting control.

Objective: Reduce overfitting and automatically remove less important features by shrinking some coefficients to zero.

Type: Regression (Regularized)



6️⃣ 🌳 ## Decision Tree Classifier
Decision Tree is trained on the same dataset (`student-performance.csv`) to predict `final_grade`.

Includes:
- Confusion Matrix
- Classification Report
- Tree visualization using `plot_tree()`



7️⃣ 🧩 Support Vector Machine (SVM) Classifier
Dataset: `student-performance.csv`  
Target column: `final_grade`

This implementation uses an **SVM (Support Vector Classifier)** for multiclass classification.

### Steps included:
- One-Hot Encoding for categorical features
- Standard Scaling for numeric features (important for SVM)
- Train-test split with stratification
- Model training using `SVC`
- Evaluation using:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Confusion Matrix visualization


## 8️⃣  🌲 Random Forest Classifier
Dataset: `student-performance.csv`  
Target column: `final_grade`

Random Forest is an ensemble learning algorithm that builds multiple decision trees and combines their results to improve accuracy and reduce overfitting.

### Steps included:
- One-Hot Encoding for categorical features
- Train-test split with stratification
- Model training using `RandomForestClassifier`
- Evaluation using:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Confusion Matrix visualization

### Hyperparameters used:
- `n_estimators=200` → number of trees
- `max_depth=12` → controls tree depth to reduce overfitting
- `min_samples_split=10` → prevents unnecessary splits
- `min_samples_leaf=5` → avoids tiny leaf nodes
- `class_weight="balanced"` → handles grade imbalance
- `n_jobs=-1` → faster training using all CPU cores

9️⃣ ---

## 🤝 K-Nearest Neighbors (KNN) Classifier
Dataset: `student-performance.csv`  
Target column: `final_grade`

KNN is a distance-based classification algorithm that predicts the class based on the **K nearest data points**.

### Steps included:
- One-Hot Encoding for categorical features
- Standard Scaling for numeric features (important for KNN)
- Train-test split with stratification
- Model training using `KNeighborsClassifier`
- Evaluation using:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Confusion Matrix visualization

### Hyperparameters used:
- `n_neighbors=7` → number of neighbors (K)
- `weights="distance"` → closer neighbors have more influence
- `p=2` → Euclidean distance


🔟 🧠###   Naive Bayes Classifier (GaussianNB)

Dataset: student-performance.csv
Target column: final_grade

Naive Bayes is a probability-based classification algorithm built on Bayes’ Theorem.
This implementation uses Gaussian Naive Bayes, which works well when features are continuous (like scores, attendance, and study hours).

Steps included:

One-Hot Encoding for categorical features

Numerical features passed directly

Train-test split with stratification

Model training using GaussianNB

Evaluation using:

Accuracy Score

Confusion Matrix

Classification Report

Confusion Matrix visualization

Final Grade Distribution plot

Model Performance:

Achieved accuracy: ~89.86%

Why GaussianNB?

Suitable for continuous numerical features

Fast training and prediction

Works well as a baseline model for multi-class classification