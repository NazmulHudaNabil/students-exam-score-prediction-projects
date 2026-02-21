# 🎓 Student Exam Score Predictor

## 📝 Project Overview
This project aims to predict students' exam scores based on various academic, personal, and environmental features using a machine learning regression model. By utilizing a linear regression approach, the model processes multiple student attributes to forecast final academic performance, offering insights into the factors that most heavily influence student success.

## ✨ Features & Workflow

* **Data Cleaning & Preprocessing:** Handles raw student data, converting categorical variables like courses and study methods into numerical form using one-hot encoding.
* **Feature Scaling:** Applies `MinMaxScaler` to normalize continuous variables (like attendance and hours studied) so they contribute equally to the model without skewing the regression coefficients.
* **Predictive Modeling:** Utilizes a trained Linear Regression model to accurately predict final exam scores based on standardized user input.
* **Data Visualization:** Includes actual vs. predicted score scatter plots with a line of best fit to visually interpret the model's accuracy.

## 🛠️ Technology Stack
* **Python:** Core programming language.
* **Pandas & NumPy:** For data manipulation, structuring the dataframes, and numerical analysis.
* **Scikit-learn:** For the Linear Regression algorithm, `MinMaxScaler`, and calculating model evaluation metrics.
* **Matplotlib:** For plotting the actual vs. predicted evaluation graphs and analyzing data distributions.

## 📊 Dataset Features
The model evaluates the following features to make an accurate prediction:
* `hours`: Number of hours studied.
* `attendance`: Student's overall attendance percentage.
* `exam_difficulty`: Rated difficulty of the upcoming exam.
* `sleep_hours`: Average hours of sleep per night.
* `facility_rating`: Rating of the educational facilities available to the student.
* `sleep_quality`: Rated quality of the student's sleep.
* `course`: One-hot encoded categorical variable representing the specific course (7 distinct categories).
* `study_method`: One-hot encoded categorical variable representing the student's preferred study approach (5 distinct categories).

## 🤖 Model Performance
After being trained on the scaled dataset, the Linear Regression model was evaluated against unseen testing data, yielding the following performance metrics:
* **Mean Absolute Error (MAE):** 7.86
* **Mean Squared Error (MSE):** 95.46
* **Root Mean Squared Error (RMSE):** 9.77
* **R² Score:** 0.73 (The model explains 73% of the variance in the exam scores)

## 🚀 Installation & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/NazmulHudaNabil/students-exam-score-prediction-projects.git
