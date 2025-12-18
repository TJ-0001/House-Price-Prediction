# House Price Prediction

## Objective
The goal is to predict house prices using the available property features, applying regression model such as **Linear Regression**
## Dataset
The dataset used for this project is the **House Price Prediction Dataset** available on Kaggle. It contains 2000 entries with the following columns:
- **Name:** House Price Prediction Dataset
- **Source:** [Kaggle](https://www.kaggle.com)  
- **Features (10 columns):**
  - `Id`          – Unique identifier for each house
  - `Area`        – Square footage of the house
  - `Bedrooms`    – Number of bedrooms
  - `Bathrooms`   – Number of bathrooms
  - `Floors`      – Number of floors
  - `YearBuilt`   – Year the house was built
  - `Location`    – Categorical location
  - `Condition`   – Condition of the house
  - `Garage`      – Garage availability
  - `Price`       – Target variable (house price) 

---

## Features
- **Numerical Features:** Area, Bedrooms, Bathrooms, Floors, YearBuilt  
- **Categorical Features:** Location, Condition, Garage

---

## Methodology
1. Load and explore the dataset.
2. Preprocess features:
   - Handle categorical variables using **One-Hot Encoding**
   - Scale numeric features for Linear Regression
3. Split dataset into training and testing sets.
4. Train regression models:
   - **Linear Regression** (baseline model)
5. Evaluate models using:
   - **Mean Absolute Error (MAE)**
   - **Root Mean Squared Error (RMSE)**
6. Visualize predicted vs actual prices and residuals.

---

## Model Evaluation
| Model                   | MAE        | RMSE       |
| ----------------------- | ---------- | ---------- |
| Linear Regression       | 243241.98    | [279859.73]    |


---

## Visualization
- **Actual vs Predicted Prices:** Shows model accuracy.  
- **Residuals Distribution:** Helps check error patterns.  
- **Residuals vs Predicted Values:** Checks for any systematic bias in predictions.

---
## Insights and Conclusion

### Insights
1. **Feature Importance**
   - Larger houses (higher `Area`) generally have higher prices.
   - Number of `Bedrooms` and `Bathrooms` moderately influence price.
   - `Location` significantly affects house price; some areas are more expensive than others.
   - Houses with a `Garage` or better `Condition` tend to have higher prices.
   - Older houses (low `YearBuilt`) sometimes have lower prices unless in prime locations.

2. **Model Performance**
   - **Linear Regression** provides a good baseline, capturing general trends but sometimes underestimates or overestimates in extreme price ranges.
  
3. **Residual Analysis**
   - Residuals for Linear Regression are roughly centered around zero but show some variance for very high-priced houses.
   
---

### Conclusion
- Predicting house prices depends on a combination of numeric features (area, bedrooms, bathrooms) and categorical features (location, condition, garage).
- Preprocessing, such as encoding categorical variables and scaling numeric ones, is crucial for model performance.
- Visualizations such as predicted vs actual plots and residual plots are effective for evaluating model accuracy and identifying areas for improvement.
- The model can be further improved by incorporating additional features like neighborhood amenities, proximity to schools, or market trends.

> Overall, this project demonstrates a complete workflow for house price prediction using linear regression model, from data preprocessing to evaluation and visualization.


## Files Included
- **House_Price_Prediction.ipynb** — Jupyter Notebook containing all code, visualizations, and outputs.
- **House Price Prediction Dataset.csv** — Dataset used for analysis and visual exploration.
---
## References
- Heart Disease UCI Dataset: [Kaggle link](https://www.kaggle.com/datasets/zafarali27/house-price-prediction-dataset)  
