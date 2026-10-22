# 🎓 Student Performance Prediction Using Machine Learning

## 📌 Project Overview

This project uses supervised machine learning to predict students' writing scores based on demographic information, test preparation, lunch category, and their math and reading scores.

The project compares two regression algorithms — **Linear Regression** and **Random Forest Regressor** — to evaluate their predictive performance.

## 🎯 Objectives

- Understand the machine learning workflow.
- Prepare input features for model training.
- Train and test regression models.
- Evaluate model performance using MAE, RMSE, and R².
- Visualize actual versus predicted scores.
- Compare different algorithms and interpret their results.

## 🛠️ Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📂 Dataset

The dataset contains 1,000 student records and 8 columns, including:

- Gender
- Race/ethnicity
- Parental level of education
- Lunch type
- Test preparation course
- Math score
- Reading score
- Writing score (prediction target)

The dataset contains no missing values in the supplied CSV.

## ⚙️ Machine Learning Workflow

1. Load and inspect the dataset.
2. Check for missing values and duplicate records.
3. Separate input features and the target variable.
4. Encode categorical variables using One-Hot Encoding.
5. Split the dataset into 80% training data and 20% testing data.
6. Train Linear Regression and Random Forest models.
7. Evaluate both models using regression metrics.
8. Visualize model performance and compare results.

## 🤖 Models Implemented

### 1. Linear Regression
A baseline regression algorithm that models the relationship between input features and writing scores.

### 2. Random Forest Regressor
An ensemble learning algorithm that combines multiple decision trees to predict numerical outcomes.

## 📊 Model Evaluation

The models were evaluated on a held-out test set using the following metrics:

| Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MAE | 3.20 | 3.66 |
| RMSE | 3.86 | 4.55 |
| R² Score | 0.938 | 0.914 |

**Best-performing model on this test split: Linear Regression.**

- **MAE:** Measures average absolute prediction error.
- **RMSE:** Penalizes larger prediction errors more heavily.
- **R²:** Measures how well the model explains variation in the target scores.

Lower MAE and RMSE are better; a higher R² is generally better.

## 📈 Visualizations

The project generates the following charts:

- Actual vs. predicted writing scores.
- Comparison of model prediction errors.
- Reading score vs. writing score.
- Correlation between math, reading, and writing scores.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd student-performance-prediction
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual repository URL.

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the model

```bash
python train_model.py
```

The evaluation metrics will be displayed in the terminal, and performance charts will be saved in the `visualizations/` folder.

You can also open `notebooks/model_training.ipynb` in Jupyter Notebook and run the cells step by step.

## 📁 Project Structure

```text
student-performance-prediction/
├── data/
│   └── StudentsPerformance.csv
├── notebooks/
│   └── model_training.ipynb
├── visualizations/
│   ├── actual_vs_predicted.png
│   └── model_error_comparison.png
├── train_model.py
├── requirements.txt
└── README.md
```

## 📚 Learning Outcomes

- Understanding supervised machine learning.
- Training regression models with Scikit-learn.
- Encoding categorical features.
- Evaluating predictive performance.
- Creating meaningful data visualizations.
- Comparing machine learning algorithms.

## 🔮 Future Improvements

- Apply cross-validation and hyperparameter tuning.
- Compare additional regression algorithms.
- Analyze prediction errors in more detail.
- Develop a simple web interface for interactive predictions.

## ⚠️ Disclaimer

This project is intended for educational purposes only. Predictions may be inaccurate or affected by biases in the dataset. The model should not be used for grading, admissions, or other high-stakes decisions about students.

## 👨‍💻 Author

Created as a hands-on project to learn machine learning, regression, and model evaluation.

⭐ If you find this project useful, consider starring the repository!
