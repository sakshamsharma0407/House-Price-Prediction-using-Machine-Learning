# 🏠 House Price Prediction using Machine Learning

A machine learning regression project that predicts residential house prices using the **Ames Housing dataset**. The project covers data preprocessing, exploratory data analysis, feature engineering, model comparison, and hyperparameter tuning.

## 📌 Project Overview

Predicting house prices is a common regression problem where multiple property characteristics influence the final sale price.

### Objectives

- Perform exploratory data analysis
- Handle missing values and categorical variables
- Identify important features affecting house prices
- Apply feature engineering and preprocessing
- Train and compare multiple regression models
- Tune model hyperparameters using cross-validation
- Evaluate models using RMSE and R²
- Select a suitable model for house price prediction

## 📊 Dataset

The project uses the **Ames Housing dataset**, containing information about residential properties and their sale prices.

The dataset includes features related to:

- Overall quality
- Living area
- Garage
- Basement
- Number of rooms
- Year built
- Neighborhood
- Overall condition
- And many other property characteristics

## 🔍 Exploratory Data Analysis

The dataset was analyzed to understand:

- Distribution of house prices
- Relationships between features and house prices
- Missing values
- Feature distributions and skewness
- Outliers
- Correlations between important variables

## 🛠️ Data Preprocessing

The following preprocessing steps were performed:

- Handling missing values
- Separating numerical and categorical features
- Encoding categorical variables
- Feature transformation
- Handling skewed variables
- Preparing training and testing datasets

## ⚙️ Feature Engineering

Feature engineering was performed to create more meaningful representations of the original variables and help the models capture relationships between property characteristics and sale prices.

## 🤖 Machine Learning Models

The following regression models were implemented and compared:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor
5. XGBoost Regressor

## 📈 Model Evaluation

The main evaluation metrics were:

### RMSE

Root Mean Squared Error measures the magnitude of prediction errors.

**Lower RMSE indicates better performance.**

### R² Score

R² measures how much of the variation in house prices is explained by the model.

**Higher R² indicates better performance.**

### Model Results

| Model | RMSE | R² |
|---|---:|---:|
| Linear Regression |**0.128575** |**0.195192**|
| Decision Tree | **0.051708** | **0.827173**|
| Random Forest |**0.027610**| **0.827173**|
| Gradient Boosting | **0.1478** | **0.8633** |
| XGBoost | **0.022158** | **0.861303** |

## 🔧 Hyperparameter Tuning

Hyperparameter tuning was performed using **RandomizedSearchCV with 5-fold cross-validation**.

The tuned Gradient Boosting model achieved:

- **RMSE:** 0.1501
- **R²:** 0.8589

The original Gradient Boosting model achieved:

- **RMSE:** 0.1478
- **R²:** 0.8633

This demonstrates that hyperparameter tuning does not necessarily guarantee better performance on a particular test set.

## 📌 Key Findings

- House prices depend on multiple property characteristics.
- Quality and size-related features have an important influence on price.
- Tree-based ensemble models can capture nonlinear relationships effectively.
- Gradient Boosting produced strong predictive performance.
- Model tuning should be evaluated based on actual validation/test performance rather than assuming it will always improve results.

## 💻 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

## 📁 Project Structure
House-Price-Prediction-using-Machine-Learning/
│
├── House Price Prediction using Machine Learning.ipynb
├── README.md
└── .gitignore
## 🚀 How to Run
1. Clone the repository
git clone https://github.com/sakshamsharma0407/House-Price-Prediction-using-Machine-Learning.git
2. Navigate to the project
cd House-Price-Prediction-using-Machine-Learning
3. Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn xgboost jupyter
4. Launch Jupyter Notebook
jupyter notebook

Open the notebook and run the cells sequentially.

## 🎯 Future Improvements
Build a Streamlit web application

Add predicted-vs-actual visualizations

Perform detailed residual analysis

Add feature-importance visualizations

Experiment with additional ensemble models

Separate preprocessing, training, and prediction into Python modules

Deploy the model for online predictions

## 👨‍💻 Author

Saksham Sharma

B.Tech Computer Science Engineering Student

Interested in Machine Learning, Data Science, and Software Development.

## 📜 License

This project is intended for educational and portfolio purposes.
