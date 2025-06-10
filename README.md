# Flight Price Prediction using Multiple Linear Regression

This project demonstrates how to build a Multiple Linear Regression (MLR) model to predict flight ticket prices based on various features extracted from a dataset. The project involves data preprocessing, exploratory data analysis (EDA), model training, evaluation, and interpretation.

## Dataset Overview

The dataset contains historical flight ticket data, with features like:
- Flight Duration
- Number of Stops
- Airline Class
- Distance
- Booking Time
- And more...

The target variable is:
- **`flightprice`**: The final ticket price paid by customers.

## Exploratory Data Analysis (EDA)

EDA was conducted to understand the data distribution and relationships among variables. Key steps included:
- Viewing dataset structure using `.head()` and `.info()`
- Descriptive statistics using `.describe()`
- Correlation heatmap to identify strongly correlated features with `flightprice`

## Model Building

### Preprocessing
- Categorical variables were converted into numeric format using `pd.get_dummies()`
- Three features most correlated with `flightprice` were selected as predictors

### Training
- The dataset was split into training and testing sets using `train_test_split()`
- A Multiple Linear Regression model was trained using `LinearRegression()` from `sklearn`

### Evaluation
- Performance metrics:
  - R² Score
  - RMSE (Root Mean Squared Error)
- Visual inspection of residuals and predictions

## Results

The MLR model provided a baseline understanding of how flight prices are influenced by a few key variables. The residuals were reasonably distributed, indicating a decent model fit.

## 🛠Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn (for visualization)
- Scikit-learn (for model training and evaluation)
