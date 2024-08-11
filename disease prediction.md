diseases prdiction based on symptoms made by Eman Sarfraz
Certainly! Here's a concise breakdown of the steps:

1. **Data Loading**
   - **Objective**: Load the medical dataset.
   - **Action**: Imported the dataset using `pandas`.
 2. **Data Preprocessing**
   - **Objective**: Prepare the data for modeling.
   - **Actions**:
     - Extracted `risk_percentage` from `risk level`.
     - Converted categorical features to numerical format.
     - Imputed missing `risk_percentage` values with the column's mean.

 3. **Feature Selection**
   - **Objective**: Identify relevant features for the model.
   - **Actions**:
     - Selected numerical features, excluding non-numeric columns like `disease` and `cures`.
     - Set `risk_percentage` as the target variable (`y`).

 4. **Data Splitting**
   - **Objective**: Split data into training and testing sets.
   - **Action**: Used `train_test_split` to create an 80/20 train-test split.

 5. **Feature Scaling**
   - **Objective**: Normalize feature values.
   - **Action**: Applied `StandardScaler` to standardize the features.

 6. **Model Training**
   - **Objective**: Train the SVM model.
   - **Action**: Trained an SVM with an RBF kernel on the training data.

 7. **Prediction**
   - **Objective**: Predict risk percentages on test data.
   - **Action**: Used the trained SVM model to make predictions.

8. **Evaluation**
   - **Objective**: Evaluate model performance.
   - **Actions**:
     - Calculated Mean Squared Error (MSE).
     - Calculated R² score.

This process led to the development and evaluation of a predictive model for disease risk using SVM.
