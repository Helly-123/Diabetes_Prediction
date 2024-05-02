# Diabetes Prediction

## Introduction

This project aims to predict the likelihood of diabetes in individuals based on user-provided information such as pregnancy, age, and BMI (Body Mass Index). Please note that glucose levels have been intentionally excluded from the prediction model to emphasize the influence of other significant factors on diabetes risk assessment. This deliberate decision allows for a more focused analysis of easily accessible variables such as pregnancy, age, and BMI, providing users with a clearer understanding of their potential risk factors for diabetes. The prediction model utilizes the Random Forest algorithm, and the deployment is done using Flask, a Python web framework.

## Project Structure

- **model/diabetes.csv:** Dataset containing information on pregnancies, glucose levels, blood pressure, skin thickness, insulin levels, BMI, diabetes pedigree function, age, and diabetes outcome.
- **model/model.py:** Python script for training the Random Forest classifier and saving the model using pickle.
- **app.py:** Flask application for handling user input and making predictions.
- **templates/index.html:** HTML template for the user input form.
- **templates/result.html:** HTML template for displaying the prediction results.
- **model/diabetes_prediction.ipynb:** Jupyter notebook containing detailed worked-out process of diabetes prediction, including exploratory data analysis, data preprocessing, feature engineering, model development, and model optimization.

## Usage

1. Enter the number of pregnancies, age, and BMI into the input form.
2. Click the "Predict" button to submit the form.
3. View the prediction result displayed on the result page.

## Prediction Output

- If the prediction indicates 0, the user appears to be at low risk for diabetes, with a recommendation for maintaining a healthy lifestyle.
- If the prediction indicates 1, the user may be at risk of developing diabetes, with a recommendation to consult a doctor for further evaluation. Additionally, the probability of having diabetes is displayed.

## Conclusion

This project demonstrates the integration of a machine learning algorithm - Random Forest, with web development using Flask for deploying a diabetes prediction system. Users can input their health information, and the system provides personalized predictions and recommendations based on the input data.

