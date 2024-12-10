# Phone Price Prediction Analysis

## Project Overview

This project explores the prediction of mobile phone prices using machine learning techniques. By analyzing various features of mobile phones, we aim to develop a robust model that can accurately estimate phone prices based on their specifications.

## Dataset

The dataset contains information about mobile phones with the following features:
- Sale volume
- Weight
- Screen resolution
- Pixels per inch (PPI)
- CPU cores
- Internal memory
- RAM
- Rear camera resolution
- Front camera resolution
- Battery capacity
- Phone thickness

## Methodology

### Data Preprocessing
- Imported necessary libraries (pandas, numpy, scikit-learn)
- Checked for null values and duplicates
- Performed feature selection using SelectKBest with chi-squared scoring
- Split data into training and testing sets
- Applied standard scaling to normalize features

### Machine Learning Models

Three regression models were explored to predict phone prices:

1. **Linear Regression**
   - Simple baseline model
   - Provides a linear relationship between features and price

2. **Random Forest Regressor**
   - Ensemble method using multiple decision trees
   - Hyperparameter tuning with GridSearchCV
   - Best parameters:
     - Number of estimators: 50
     - Max depth: None
     - Minimum samples split: 2

3. **Support Vector Regression (SVR)**
   - Non-linear regression technique
   - Hyperparameter tuning with GridSearchCV
   - Best parameters:
     - Regularization parameter (C): 3
     - Kernel: Linear
     - Degree: 1

## Model Evaluation

Models were evaluated using the following metrics:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R-squared (R²)

### Performance Comparison

| Model | MSE | MAE | R² |
|-------|-----|-----|-----|
| Linear Regression | 48,766.21 | 183.94 | 0.881 |
| Random Forest | 34,211.06 | 146.53 | 0.916 |
| Support Vector Regression | 30,456.51 | 144.37 | 0.926 |

## Key Insights

- Support Vector Regression (SVR) demonstrated the best predictive performance
- Random Forest showed more stable residuals, indicating good generalization
- The chosen features effectively capture the factors influencing phone prices

## Recommendations

1. For precise price prediction, use the Support Vector Regression model
2. For a more robust and generalizable model, consider the Random Forest approach
3. Potential future work could involve ensemble methods combining multiple models

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## How to Use

1. Clone the repository
2. Install required libraries
3. Run the Jupyter notebook or Python script
4. Explore the analysis and model predictions

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the issues page if you want to contribute.

## License

[Specify your license here]

## Contact

[Your contact information or GitHub profile]
