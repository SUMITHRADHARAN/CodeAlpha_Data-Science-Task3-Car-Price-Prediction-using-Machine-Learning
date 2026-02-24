# 🚗 Car Price Prediction with Machine Learning
This project implements a machine learning model to predict the selling price of used cars. It leverages various car attributes such as kilometers driven, fuel type, selling type, transmission, and the age of the car to build a robust prediction model using the Random Forest Regressor. And this project builds a machine learning model to predict used car prices based on features such as brand goodwill, year of manufacture, fuel type, transmission, mileage and more.

# 🚗 Car Price Prediction Project 📈

Welcome to the Car Price Prediction project repository! In this project, I aim to predict car prices using various machine learning algorithms and techniques. I have gone through a rigorous process of data cleaning, exploratory data analysis (EDA), feature engineering, data preprocessing, model development, and evaluation to arrive at my best-performing model, the Random Forest Regressor.

![car](https://github.com/RoshankumarS14/Car-Price-Prediction/assets/123869873/ecc02265-d770-4ee1-b50f-ca06963d799b)

## Project Overview 🌟

In this project, I've accomplished the following steps:

1. **Data Cleaning**: I started by cleaning and preparing the dataset to remove any inconsistencies and missing values.

2. **EDA**: Extensive Exploratory Data Analysis was conducted, including univariate, bivariate, statistical testing, and multivariate analysis to gain insights into the data.

3. **Feature Engineering**: I employed feature engineering techniques to create new features and enhance the predictive power of my models.

4. **PCA (Principal Component Analysis)**: Dimensionality reduction through PCA was explored to reduce complexity and improve model performance.

5. **Data Preprocessing**: Encoding categorical variables and scaling numerical features was carried out to prepare the data for modeling.

6. **Model Development**: I developed several regression models, including Linear Regression, Decision Tree, AdaBoost, Gradient Boosting, and Random Forest Regressor.

7. **Model Evaluation**: Thorough model evaluation was performed, and various metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared were used to compare and select the best-performing model.


 
## 📌 Project Steps
- **Data Loading & Exploration**: Load car data, inspect missing values and unique features.
- **Data Preprocessing**: Convert categorical features (Fuel_Type, Selling_type, Transmission) into numeric form, derive `Age` from `Year`.
- **Feature Engineering**: Drop unnecessary columns, one-hot encode categorical variables.
- **Model Training**: Train a regression model (Random Forest Regressor) on the processed data.
- **Evaluation**: Use R² Score and RMSE to evaluate model performance.
- **Prediction**: Predict selling price of a new car given its attributes.
- **Visualization**: Scatter plot of actual vs. predicted prices to check model accuracy.


## 🛠️ Tech Stack
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

📊 Dataset
The model requires car data.csv in the root directory. Key columns include:
Year: Manufacturing year.
Present_Price: Current ex-showroom price (Target reference).
Driven_kms: Total mileage.
Fuel_Type: Petrol, Diesel, or CNG.
Selling_type: Dealer or Individual.
Transmission: Manual or Automatic.
Target Variable: Selling_Price (The price at which the car is sold).

📂 Project Structure
.
├── car data.csv               # Input dataset
├── car_price_prediction.py    # Main script
├── README.md                  # Project documentation
├── correlation_matrix.png     # Heatmap visualization
├── actual_vs_predicted.png    # Prediction accuracy plot
└── feature_importances.png    # Most influential features plot


## 🌟 Features

- **Data Loading & Exploration:** Initial inspection of `car data.csv` and summary statistics.
- **Feature Engineering:** 
  - Calculated `Car_Age` from manufacturing year (Base year: 2025).
  - Categorical encoding via **One-Hot Encoding** with `drop_first=True` to avoid the dummy variable trap.
- **Exploratory Data Analysis (EDA):** Statistical summaries and a **Correlation Heatmap** to identify relationships.
- **Model Training:** Utilizes a `RandomForestRegressor` (100 estimators) with an 80/20 train-test split.
- **Comprehensive Evaluation:** Reports MAE, MSE, RMSE, and R² scores.
- **Visual Insights:** 
  - Actual vs. Predicted Price scatter plots.
  - Feature Importance analysis to identify top price drivers.

## Best Model 🏆
After evaluating all the models, the **Random Forest Regressor** emerged as the top performer, demonstrating excellent generalization capabilities.

## 🛠️ Installation
1. Clone: git clone https://github.com/AliHasnainAbro/CodeAlpha_Car-Price-Prediction-with-Machine-Learning.git
2. Setup Venv: python -m venv venv
3. Activate:
   - Windows: .\venv\Scripts\activate
   - Mac/Linux: source venv/bin/activate
4. Install: pip install pandas scikit-learn matplotlib numpy seaborn

## How to Run 🏃‍♀️🏃‍♂️

1. Clone this repository to your local machine.
2. Create a virtual environment and install the required packages using `pip install -r requirements.txt`.
3. Navigate to the `notebooks/` or `scripts/` directory to run the code for various project stages.
4. Follow the step-by-step instructions in the Jupyter notebooks or Python scripts.


--- OUTPUTS ---
The script will output performance metrics to the console and save three images:
- correlation_matrix.png
- actual_vs_predicted_selling_price.png
- feature_importances.png

--- USAGE ---
Run the script using: python car_price_prediction.py

📈 Results & Visualizations
Upon execution, the script generates the following insights:
Correlation Heatmap: Visualizes multicollinearity.
Actual vs. Predicted Plot: A scatter plot with a 45-degree reference line showing how closely predictions align with reality.
Feature Importance: A bar chart showing that Present_Price and Car_Age typically have the highest impact.











