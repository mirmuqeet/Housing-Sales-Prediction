**Housing Price Prediction Model**

This project involves building a housing price prediction model using machine learning techniques to predict house prices based on various features.

**Overview**

The dataset used in this project is Housing.csv, which includes the following features:

**price:** The price of the house (target variable).

**area:** The area of the house in square feet.

**bedrooms:** Number of bedrooms in the house.

**bathrooms:** Number of bathrooms in the house.

**stories:** Number of stories in the house.

**mainroad:** Whether the house is on the main road (yes or no).

**guestroom**: Whether the house has a guest room (yes or no).

**basement**: Whether the house has a basement (yes or no).

**hotwaterheating**: Whether the house has hot water heating (yes or no).

**airconditioning**: Whether the house has air conditioning (yes or no).

**parking**: Number of parking spaces.

**prefarea**: Whether the house is in a preferred area (yes or no).

**furnishingstatus**: The furnishing status of the house (furnished, semi-furnished, unfurnished).

**Steps**

**Data Loading**: Loaded the dataset and performed an initial exploration to understand its structure and contents.

**Data Cleaning**: Verified that there were no missing values in the dataset.

**Feature Engineering**:

Converted categorical variables into binary format using encoding techniques.

Created dummy variables for the furnishingstatus feature.

**Feature Selection**:

Used Recursive Feature Elimination (RFE) with a Linear Regression model to identify and select the most relevant features for predicting house prices.

Found that bedrooms was not a significant predictor in the presence of other variables and excluded it from the final model.

**Model Building:**

Built a linear regression model using selected features.

Evaluated the model’s performance using Ordinary Least Squares (OLS) regression.

**Model Evaluation:**

Assessed model performance through key metrics and examined feature importance.

**Results**
Model Performance Metrics:

R-squared: 0.676

Adjusted R-squared: 0.667

These metrics indicate that the model explains approximately 67.6% of the variance in housing prices.

**Key Features:**

area
bathrooms
stories
mainroad
guestroom
hotwaterheating
airconditioning
parking
prefarea
unfurnished

**Feature Insights:**

The area of the house is the most significant predictor of price.

Categorical features such as mainroad, guestroom, and airconditioning have a noticeable impact on pricing.
**
Requirements**
Python 3.x
Pandas
NumPy
Scikit-Learn
StatsModels
