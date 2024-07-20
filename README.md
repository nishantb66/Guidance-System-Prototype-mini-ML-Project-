
# SUV Car Purchasing Prediction

## Project Overview

This project aims to predict whether a customer will purchase an SUV car based on their age and salary. The prediction is made using a logistic regression model. The project includes a web application built with Streamlit to allow users to input age and salary values and receive a prediction.

## Project Structure

The project consists of the following files:

1. **Model_LR.ipynb**: Jupyter notebook containing the code for data preprocessing, model training, and evaluation.
2. **app.py**: Streamlit application for interacting with the model.
3. **mahindra.jpeg**: Image used in the Streamlit application.
4. **suv_data.csv**: Dataset containing user information, including age, salary, and whether they purchased the SUV.

## Data Description

The dataset `suv_data.csv` contains the following columns:
- User ID
- Gender
- Age
- EstimatedSalary
- Purchased (0 or 1)

## Steps in the Notebook

The Jupyter notebook `Model_LR.ipynb` follows these steps:

1. **Data Preprocessing**:
   - Load the dataset.
   - Extract independent (Age, Salary) and dependent (Purchased) variables.
   - Split the data into training and testing sets.
   - Scale the features using `StandardScaler`.

2. **Model Training**:
   - Train a logistic regression model on the training set.

3. **Model Evaluation**:
   - Make predictions on the test set.
   - Calculate the accuracy of the model on both training and test sets.
   - Generate a confusion matrix and visualize it using a heatmap.

## Streamlit Application

The `app.py` file contains the code for the Streamlit application. The application performs the following tasks:

1. **Loads the trained model and data scaler**.
2. **Displays an image (`mahindra.jpeg`)**.
3. **Collects user input**:
   - Age (using a slider).
   - Salary (using a slider).

4. **Makes predictions** based on the input.
5. **Displays the prediction result**.

## How to Run the Project

1. **Install the required packages**:
   ```bash
   pip install streamlit pandas scikit-learn
   ```

2. **Run the Streamlit application**:
   ```bash
   streamlit run app.py
   ```

3. **Interact with the application**:
   - Adjust the age and salary sliders to see if the user is predicted to purchase an SUV.

## Conclusion

This project demonstrates how to build and deploy a machine learning model using logistic regression. It provides a user-friendly interface for making predictions based on age and salary.
