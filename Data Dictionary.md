# Week 15 - Datasets Dictionary

This folder contains all the synthetic datasets required for completing the Week 15 assignments on Advanced Regression Techniques (Polynomial Regression, Support Vector Regression, and Decision Tree Regression).

## Folder Structure

```
Week-15 (Regression-2)/
│
├── Task-Datasets/
│   ├── task1_polynomial_data.csv
│   ├── task2_svr_data.csv
│   └── task3_decision_tree_data.csv
│
├── Assignment-Dataset/
│   ├── assignment1_salary_prediction.csv
│   ├── assignment2_energy_efficiency.csv
│   └── assignment3_stock_prices.csv
│
└── Assessment-Dataset/
    └── car_price_prediction.csv
```


## Task Datasets

### 1. task1_polynomial_data.csv
**Purpose**: Practice building and comparing Linear vs Polynomial Regression models

**Columns**:
- `Experience_Years` (numeric): Years of work experience (1-15)
- `Salary` (numeric): Annual salary in thousands of dollars (30-150)

**Records**: 15 rows  
**Pattern**: Non-linear relationship between experience and salary

**Use Case**: Compare performance of Linear Regression vs Polynomial Regression (degrees 2, 3, 4)


### 2. task2_svr_data.csv
**Purpose**: Practice implementing Support Vector Regression with feature scaling

**Columns**:
- `Temperature` (numeric): Temperature in Celsius (15-35°C)
- `Ice_Cream_Sales` (numeric): Daily ice cream sales in units (150-850)

**Records**: 20 rows
**Pattern**: Non-linear relationship with some outliers

**Use Case**: Apply SVR with RBF kernel and compare with Linear Regression. Requires feature scaling.


### 3. task3_decision_tree_data.csv
**Purpose**: Implement Decision Tree Regression and visualize splits

**Columns**:
- `Hours_Studied` (numeric): Study hours per week (5-40)
- `Exam_Score` (numeric): Exam score percentage (45-98)

**Records**: 25 rows
**Pattern**: Non-continuous relationship with plateaus

**Use Case**: Build Decision Tree Regressor, visualize with high resolution, compare with Linear Regression



## Assignment Datasets

### 1. assignment1_salary_prediction.csv
**Purpose**: Comprehensive comparison of all three regression techniques

**Columns**:
- `Position_Level` (numeric): Job position level (1-10)
- `Salary` (numeric): Annual salary in dollars (40,000-1,000,000)

**Records**: 10 rows
**Pattern**: Exponential growth pattern

**Use Case**: Build and compare:
- Linear Regression
- Polynomial Regression (multiple degrees)
- Support Vector Regression
- Decision Tree Regression

Evaluate which model best captures the salary progression pattern.


### 2. assignment2_energy_efficiency.csv
**Purpose**: Multi-feature non-linear regression problem

**Columns**:
- `Temperature` (numeric): Outside temperature (5-35°C)
- `Humidity` (numeric): Humidity percentage (30-80%)
- `Wind_Speed` (numeric): Wind speed in km/h (0-25)
- `Solar_Radiation` (numeric): Solar radiation in W/m² (100-900)
- `Energy_Consumption` (numeric): Energy consumption in kWh (50-450) - **Target variable**

**Records**: 100 rows
**Pattern**: Complex non-linear interactions

**Use Case**: Build SVR and Decision Tree models with multiple features. Compare performance and analyze feature importance.


### 3. assignment3_stock_prices.csv
**Purpose**: Time-series prediction with polynomial features

**Columns**:
- `Day` (numeric): Trading day number (1-90)
- `Opening_Price` (numeric): Stock opening price
- `High_Price` (numeric): Daily high price
- `Low_Price` (numeric): Daily low price
- `Volume` (numeric): Trading volume
- `Closing_Price` (numeric): Stock closing price - **Target variable**

**Records**: 90 rows
**Pattern**: Trending with volatility

**Use Case**: Predict stock closing prices using:
- Polynomial Regression with engineered features
- Decision Tree Regression for capturing non-linear patterns
Compare model performance and discuss limitations for financial prediction.



## Assessment Dataset

### assessment_car_price_prediction.csv
**Purpose**: Comprehensive regression project using all learned techniques

**Columns**:
- `Brand` (categorical): Car brand (Toyota, Honda, Ford, BMW, Audi, Mercedes)
- `Year` (numeric): Manufacturing year (2010-2023)
- `Mileage` (numeric): Mileage in kilometers (5,000-200,000)
- `Engine_Size` (numeric): Engine size in liters (1.0-5.0)
- `Horsepower` (numeric): Engine horsepower (70-450)
- `Fuel_Type` (categorical): Fuel type (Petrol, Diesel, Electric, Hybrid)
- `Transmission` (categorical): Transmission type (Manual, Automatic)
- `Previous_Owners` (numeric): Number of previous owners (0-5)
- `Accident_History` (categorical): Accident history (Yes/No)
- `Service_Records` (categorical): Complete service records (Yes/No)
- `Price` (numeric): Car price in dollars (8,000-95,000) - **Target variable**

**Records**: 200 rows
**Pattern**: Complex non-linear relationships with categorical features

**Use Case**: 
Complete end-to-end machine learning project:
1. Data preprocessing (encoding, scaling)
2. Build and compare all regression models:
   - Multiple Linear Regression (baseline)
   - Polynomial Regression
   - Support Vector Regression
   - Decision Tree Regression
3. Hyperparameter tuning for best model
4. Model evaluation and selection
5. Business insights and recommendations

**Complexity**: Advanced - requires integration of Week 14 preprocessing techniques with Week 15 advanced regression models.



## Data Quality Notes

- Missing values are intentionally NOT included to focus on regression techniques
- Datasets are designed to demonstrate specific regression method strengths
- Outliers in SVR dataset are intentional to demonstrate robustness
- Feature scaling is required for SVR datasets
- Decision Tree datasets contain non-continuous patterns to highlight tree-based advantages


## Usage Guidelines

1. **Tasks**: Focus on implementing one technique at a time, understanding hyperparameters
2. **Assignments**: Compare multiple techniques, analyze when each works best
3. **Assessment**: Integrate all knowledge from Weeks 14-15 for complete ML pipeline


**Note**: Refer to this Data Dictionary when working on any Week 15 assignments. Each dataset is specifically designed to highlight the strengths of particular regression techniques covered in the week.
