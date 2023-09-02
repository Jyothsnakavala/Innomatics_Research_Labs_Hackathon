# Innomatics_Research_Labs_Hackathon
This repository contains four distinct machine learning models designed to predict fare amounts for Uber rides using a comprehensive dataset. These models are implemented using Python and popular machine learning libraries.
**Linear Regression Model:**
Linear Regression is a straightforward and interpretable regression technique that aims to find a linear relationship between the input features and the target variable (fare amount, in this case). Here's how the Linear Regression model was built:

Data Preprocessing: The Uber dataset was loaded into a Pandas DataFrame. Missing values in the dataset were handled appropriately, and features like 'distance' were engineered using the Haversine formula to calculate distances based on latitude and longitude coordinates.

Feature Selection: The input features for the Linear Regression model were chosen as 'passenger_count,' 'distance,' and 'ride_week_day.' These features were considered relevant for predicting fare amounts.

Training and Testing Split: The dataset was split into a training set (70%) and a testing set (30%) to train and evaluate the model's performance.

Model Building: The Linear Regression model was instantiated and trained using the training data. It learned the relationship between the input features and fare amounts, adjusting linear coefficients to minimize the prediction error.

Model Evaluation: After training, the model was evaluated on the testing set. The evaluation metric used was R-squared, which measures how well the model fits the data. Adjusted R-squared was also calculated to account for the number of features.

**Random Forest Regression Model:**
Random Forest Regression is an ensemble learning technique that combines multiple decision trees to make robust predictions. Here's how the Random Forest Regression model was built:

Data Preprocessing: Similar to Linear Regression, data preprocessing included handling missing values, calculating distances, and extracting the day of the week from the 'pickup_datetime' feature.

Feature Selection: The same input features, 'passenger_count,' 'distance,' and 'ride_week_day,' were chosen for the Random Forest Regression model.

Training and Testing Split: The dataset was split into training and testing sets for model training and evaluation.

Model Building: A Random Forest Regression model with 100 decision trees was created. This ensemble technique improves predictive accuracy and generalization by aggregating multiple decision trees.

Model Evaluation: The model was evaluated on the testing set using R-squared. Adjusted R-squared was calculated to provide a measure of model performance while considering the number of features.

**Decision Tree Regression Model:**
Decision Tree Regression builds a regression model in the form of a decision tree. It's a simple yet powerful model that can capture nonlinear relationships. Here's how the Decision Tree Regression model was built:

Data Preprocessing: Data preprocessing steps, including handling missing values and feature engineering, were performed as with the other models.

Feature Selection: The same set of input features, 'passenger_count,' 'distance,' and 'ride_week_day,' were used for the Decision Tree Regression model.

Training and Testing Split: The dataset was divided into training and testing sets.

Model Building: A Decision Tree Regression model was created. This model makes splits in the data based on feature values to predict fare amounts.

Model Evaluation: The model's performance was evaluated using R-squared, a metric that measures how well the decision tree fits the data.

**K-Nearest Neighbors (KNN) Regression Model:**
K-Nearest Neighbors is typically used for classification but was adapted for regression in this case. KNN predicts fare amounts based on the proximity of similar rides in terms of input features. Here's how the KNN Regression model was built:

Data Preprocessing: Data preprocessing steps, including handling missing values and feature engineering, were carried out as with the other models.

Feature Selection: The same input features, 'passenger_count,' 'distance,' and 'ride_week_day,' were selected for KNN Regression.

Training and Testing Split: The dataset was split into training and testing sets as before.

Model Building: A K-Nearest Neighbors Regression model was created with a specified number of neighbors (e.g., 5). This model predicts fare amounts by finding the k-nearest rides with similar feature values.

Model Evaluation: The model was evaluated using R-squared, a metric that assesses how well the KNN Regression model fits the data. Adjusted R-squared was not calculated as it is more commonly used with linear regression models.

In summary, these four models were built using the same dataset with specific input features and variations in modeling techniques. Each model was trained and evaluated for its ability to predict Uber fare amounts, with R-squared (and adjusted R-squared for linear regression) used as the primary evaluation metric. This repository provides a comprehensive comparison of different regression models for predicting fare amounts in the context of Uber rides.




