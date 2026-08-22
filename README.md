# 🏠 House Price Prediction using Machine Learning

A machine learning regression project that predicts residential house prices using the Ames Housing dataset. The project covers data preprocessing, exploratory data analysis, feature engineering, model comparison, and hyperparameter tuning.

# 📌 Project Overview

Predicting house prices is a common regression problem where multiple property characteristics influence the final sale price.

In this project, different machine learning regression models are trained and evaluated to determine which approach performs best for predicting house prices.

Objectives
Perform exploratory data analysis on the housing dataset
Handle missing values and categorical variables
Identify important features affecting house prices
Apply feature engineering and data preprocessing
Train and compare multiple regression models
Tune model hyperparameters using cross-validation
Evaluate models using RMSE and R²
Select the most suitable model for house price prediction
📊 Dataset

The project uses the Ames Housing dataset, which contains information about residential properties and their sale prices.

The dataset contains numerous numerical and categorical features describing properties, including:

Overall quality
Living area
Garage information
Basement area
Number of rooms
Year built
Neighborhood
Overall condition
And many other property characteristics

The training data used in this project contains approximately 1,168 rows and 81 columns after the relevant dataset preparation.

🔍 Exploratory Data Analysis

The dataset was explored to understand:

Distribution of house prices
Relationships between numerical features and house prices
Missing values
Feature distributions and skewness
Potential outliers
Correlations between important variables

Visualizations were used to identify patterns and understand which features could be useful for prediction.

Example analyses
Sale Price distribution
Correlation analysis
Feature vs. Sale Price relationships
Distribution of important numerical features
Outlier analysis
🛠️ Data Preprocessing

Several preprocessing steps were performed before training the models:

Handling missing values
Separating numerical and categorical features
Encoding categorical variables
Feature transformation where appropriate
Handling skewed variables
Preparing training and testing datasets

These steps help ensure that the machine learning models receive clean and usable input data.

⚙️ Feature Engineering

Feature engineering was performed to create more meaningful representations of the original variables.

The purpose was to help the models capture relationships between property characteristics and their final sale prices more effectively.

Examples include combining relevant property-area information and transforming variables where necessary.

🤖 Machine Learning Models

The following regression models were implemented and compared:

Linear Regression
Decision Tree Regressor
Random Forest Regressor
Gradient Boosting Regressor
XGBoost Regressor

The models were evaluated using the same prepared dataset to make their performance comparable.

📈 Model Evaluation

The main evaluation metrics used were:

RMSE

Root Mean Squared Error measures the average magnitude of prediction errors, with larger errors receiving greater weight.

Lower RMSE indicates better performance.

R² Score

R² measures how much of the variation in house prices is explained by the model.

Higher R² indicates better performance.

Model Comparison
Model	RMSE	R²
Linear Regression	—	—
Decision Tree	—	—
Random Forest	—	—
Gradient Boosting	0.1478	0.8633
XGBoost	—	—

The values above should be updated with the exact final results from the notebook if the experiments are rerun.

🔧 Hyperparameter Tuning

After comparing the initial models, hyperparameter tuning was performed using RandomizedSearchCV with 5-fold cross-validation.

The purpose of tuning was to find a better combination of model parameters while reducing the risk of relying on a single train/test split.

The tuned Gradient Boosting model achieved:

RMSE: 0.1501
R²: 0.8589

Interestingly, the untuned Gradient Boosting model achieved:

RMSE: 0.1478
R²: 0.8633

This demonstrates an important practical observation: hyperparameter tuning does not always improve performance on a particular test set.

📌 Key Findings

Some important observations from the project include:

House prices are influenced by multiple interacting property characteristics.
Property quality and size-related features play an important role in prediction.
Tree-based ensemble models can capture nonlinear relationships that simpler linear models may not capture effectively.
Gradient Boosting provided strong predictive performance among the tested models.
Hyperparameter tuning should be evaluated carefully rather than assuming that tuning will always improve the final test score.
💻 Technologies Used
Python
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
XGBoost
Jupyter Notebook
📁 Project Structure
House-Price-Prediction-using-Machine-Learning/
│
├── House Price Prediction using Machine Learning.ipynb
├── README.md
└── .gitignore
🚀 How to Run
1. Clone the repository
git clone https://github.com/sakshamsharma0407/House-Price-Prediction-using-Machine-Learning.git
2. Navigate to the project
cd House-Price-Prediction-using-Machine-Learning
3. Install the required libraries
pip install numpy pandas matplotlib seaborn scikit-learn xgboost jupyter
4. Launch Jupyter Notebook
jupyter notebook

Open the project notebook and run the cells sequentially.

🎯 Future Improvements

Possible improvements include:

Build a Streamlit web application
Add predicted-vs-actual visualizations
Perform detailed residual/error analysis
Add feature-importance visualizations
Experiment with additional ensemble models
Improve the project structure by separating preprocessing, training, and prediction code
Deploy the trained model for online predictions
👨‍💻 Author

Saksham Sharma

B.Tech Computer Science Engineering Student

Interested in Machine Learning, Data Science, and Software Development.

📜 License

This project is intended for educational and portfolio purposes.
