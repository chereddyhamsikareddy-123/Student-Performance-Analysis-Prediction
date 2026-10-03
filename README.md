# Student Performance Analysis & Prediction

## Project Overview

This project analyzes student performance data to identify factors associated with exam scores and builds machine learning models to predict student exam performance.

## Objectives

- Clean and preprocess the student performance dataset
- Perform Exploratory Data Analysis (EDA)
- Analyze factors such as attendance, study hours, previous scores, and parental education
- Build and compare multiple machine learning regression models
- Evaluate models using MAE, RMSE, and R²
- Identify important features used by the prediction model

## Dataset

The dataset contains information about student study habits, attendance, parental involvement, access to resources, previous scores, tutoring, and other student-related factors.

**Target variable:** `Exam_Score`

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Machine Learning Models

The following regression models were developed and compared:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor

## Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Results

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 0.452 | 1.804 | 0.770 |
| Gradient Boosting | 0.790 | 1.947 | 0.732 |
| Random Forest | 1.084 | 2.161 | 0.670 |
| Decision Tree | 1.592 | 2.538 | 0.544 |

On this particular train/test split, Linear Regression produced the strongest results among the models tested.

## Key Insights

- Attendance showed the strongest relationship with exam scores among the numerical variables analyzed.
- Hours studied showed the second strongest relationship with exam scores.
- Previous scores and tutoring sessions showed weaker positive relationships.
- Sleep hours and physical activity showed very weak linear relationships with exam scores.
- Random Forest feature importance also identified attendance and hours studied as the two most important individual features.

These relationships represent patterns in the dataset and should not be interpreted as proof of causation.

## Project Structure

```text
Student-Performance-Analysis-Prediction/
│
├── Student_Performance_Analysis_Prediction.ipynb
├── StudentPerformanceFactors.csv
└── README.md
