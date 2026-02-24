# CodeAlpha_Data-Science-Task3-Car-Price-Prediction-using-Machine-Learning
This project implements a machine learning model to predict the selling price of used cars. It leverages various car attributes such as kilometers driven, fuel type, selling type, transmission, and the age of the car to build a robust prediction model using the Random Forest Regressor.

# 🚗 Car Price Prediction with Machine Learning

This project implements a **Random Forest Regressor** to predict the selling price of used cars based on various features such as age, mileage, and fuel type.

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

## 🛠️ Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/AliHasnainAbro/CodeAlpha_Car-Price-Prediction-with-Machine-Learning.git
   cd car-price-prediction
   
2. Set Up Virtual Environment (Recommended):
python -m venv venv
# Windows:
.\venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

3. Install Dependencies:
pip install pandas scikit-learn matplotlib numpy seaborn

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

--- DESCRIPTION ---
A machine learning project using Random Forest Regressor to predict used car prices.

--- FEATURES ---
1. Data Preprocessing: Missing value checks and feature engineering (Car_Age).
2. Categorical Encoding: One-Hot Encoding for Fuel_Type, Selling_type, and Transmission.
3. EDA: Statistical summaries and correlation heatmaps.
4. Model: Random Forest Regressor (100 estimators).
5. Evaluation: Metrics include MAE, MSE, RMSE, and R-squared.

--- INSTALLATION ---
1. Clone: git clone https://github.com/AliHasnainAbro/CodeAlpha_Car-Price-Prediction-with-Machine-Learning.git
2. Setup Venv: python -m venv venv
3. Activate:
   - Windows: .\venv\Scripts\activate
   - Mac/Linux: source venv/bin/activate
4. Install: pip install pandas scikit-learn matplotlib numpy seaborn


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
