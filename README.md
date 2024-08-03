# Unmess the Mess: Food Waste Reduction with Machine Learning
## Data Exploration & Preparation:

The code delves into the provided sample data, which includes:

  * Mess Menu.xlsx: Contains the hostel's food schedule.
  * MessSample.xlsx: Provides sample data on food items served over two days (Breakfast and Lunch).
  * Encoding Sheets (food_id.xlsx, day_encoding.xlsx, time_encoding.xlsx): Encode categorical variables for modeling.

### Explorations involve:

  * Visualizing leftover patterns with scatterplots.
  * Creating a pairplot for visualizing relationships between variables.
  * Encoding categorical features (day, time, and food_id) for numerical representation.
  * Deriving a new feature, "consumption," by subtracting leftovers from total quantity.

## Machine Learning Model:

  * Linear Regression: Chosen for initial exploration due to its simplicity and interpretability.
  * Training/Testing Split: The data is divided into training and testing sets using train_test_split for model training and evaluation.
  * Feature Scaling (Optional): Consider scaling numerical features if necessary using preprocessing.StandardScaler for better model performance.
  * Model Fitting: The model is trained on the training data using model.fit(X_train, y_train).
  * Prediction: New consumption values are predicted on the testing data using model.predict(X_test). 
  * Evaluation: Mean Squared Error (MSE) and Mean Absolute Error (MAE) are calculated using mean_squared_error and mean_absolute_error to assess model performance.

## Future Enhancements:

  * Explore alternative machine learning models (e.g., Random Forest, Gradient Boosting) for potentially better performance.
  * Integrate the model into a real-world system for meal planning optimization.
  * Incorporate additional data sources (e.g., weather, student surveys) to enrich the model's understanding of food waste patterns.
