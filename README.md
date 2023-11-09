# Chennai-House-Price-Prediction-
Chennai Housing Price Prediction Report:

Data Loading and Cleaning:
The data is loaded from a CSV file into a Pandas dataframe. Several cleaning steps are applied:
Fix typos and abbreviations in columns like AREA, STREET, BUILDTYPE etc.
Convert categorical features like PARK_FACIL to numeric values.
Handle missing values.
Convert DATE_SALE and DATE_BUILD to datetime format.

Exploratory Data Analysis:
Statistics like the correlation matrix, histogram and heatmap visualizations are generated to understand relationships between variables.
Total_Sales_Price is correlated with features like sqft area, number of rooms etc.

Feature Engineering:
The data is prepared for modeling by:
Dropping non-useful columns like IDs and text fields.
One-hot encoding the categorical AREA column.
Splitting into X (features) and y (target price).

Model Training:
Multiple regression models are trained and evaluated using cross-validation:
Linear regression, Lasso regression, decision tree regression
Tuned hyperparameters using grid search
Linear regression performed best with R^2 score of 0.72 on test set

Conclusion:
The linear regression model can effectively predict housing prices based on location, size, number of rooms etc. It could be improved further with more data.
The model can be productionized and integrated into a housing price estimator tool.
