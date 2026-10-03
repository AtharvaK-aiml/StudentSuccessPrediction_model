# 🎓 Student Placement Prediction

A beginner-friendly machine learning project that predicts whether a student is likely to be **Placed** or **Not Placed** based on academic, technical, and extracurricular attributes.

This project was built as a hands-on introduction to the end-to-end machine learning workflow — from exploring a dataset to training, evaluating, and comparing multiple classification models.

## 📌 Project Overview

The goal of this project is to explore whether student-related attributes can be used to predict placement outcomes.

The project covers:

* Exploratory Data Analysis (EDA)
* Data preprocessing
* Numerical feature scaling
* Categorical feature encoding
* Train/test splitting
* Multiple classification algorithms
* Hyperparameter tuning
* Model evaluation
* Comparison of classification metrics

## 📊 Dataset

The project uses a student career/placement dataset containing **50,000 student records** and multiple academic, technical, and extracurricular features.

Some of the features include:

* Age
* Gender
* University Year
* Major
* Attendance
* Study Hours
* CGPA
* Programming Skills
* Projects Completed
* Certifications
* Hackathons
* Internships
* Communication Skills
* Leadership Skills
* Interview Score
* Resume Score
* Employability Score

The target variable is:

```text
Placement_Status
```

with two classes:

```text
Placed
Not Placed
```

## 🔍 Exploratory Data Analysis

The EDA notebook explores:

* Dataset structure and dimensions
* Data types
* Missing values
* Numerical feature distributions
* Categorical feature distributions
* Placement class distribution
* Relationships between features and placement status
* Correlation between numerical variables

The dataset contains more students in the **Placed** class than the **Not Placed** class, so metrics such as precision, recall, and F1-score are considered alongside accuracy.

## ⚙️ Machine Learning Workflow

The project follows this workflow:

```text
Dataset
   ↓
Exploratory Data Analysis
   ↓
Feature Selection
   ↓
Train / Test Split
   ↓
Preprocessing
   ├── Numerical → StandardScaler
   └── Categorical → OneHotEncoder
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
```

The preprocessing steps are implemented using scikit-learn pipelines and a `ColumnTransformer`.

## 🤖 Models Tested

The following classification models were explored:

* Logistic Regression
* Gaussian Naive Bayes
* K-Nearest Neighbors
* Random Forest
* XGBoost
* Voting Classifier

K-Nearest Neighbors was also experimented with using hyperparameter tuning through cross-validation.

## 📈 Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Rather than relying only on accuracy, the project also looks at how well the models identify the **Not Placed** class.

This is important because a model can have good overall accuracy while still performing poorly on one of the classes.

## 🧠 What I Learned

Through this project, I learned about:

* The importance of understanding a dataset before training a model
* Exploratory Data Analysis
* Handling numerical and categorical features
* Building preprocessing pipelines
* Train/test splitting
* Classification algorithms
* Cross-validation and hyperparameter tuning
* Confusion matrices
* Precision, recall, and F1-score
* The effect of class imbalance on model performance

One of the biggest things I learned is that **a higher accuracy does not always mean a better model**. Looking at different evaluation metrics gives a better understanding of how a model is actually performing.

## 🚧 Future Improvements

This is a learning project, and there are several things I would like to explore next:

* Improve feature selection
* Experiment with class-balancing techniques
* Perform more systematic hyperparameter tuning
* Add ROC-AUC and PR-AUC evaluation
* Perform more detailed error analysis
* Save the final trained model
* Build a simple prediction interface using Streamlit
* Deploy the model

## 📁 Project Structure

```text
StudentSuccessPrediction_model/
│
├── data/
│   └── student_career_success_dataset.csv
│
├── data_EDA.ipynb
├── model_training.ipynb
├── README.md
└── .gitignore
```

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Jupyter Notebook

## 👨‍💻 About the Project

This project was created as a hands-on machine learning learning project to understand the complete workflow of building a classification model.

It is a starting point in my journey of learning **Machine Learning and AI**, and I plan to continue improving it as I learn more.

---

⭐ If you found the project interesting, feel free to explore the notebooks and share feedback!

