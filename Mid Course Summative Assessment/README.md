# Rainfall Prediction Using Logistic Regression

__Mid Course Assessment__ - ML Case Study 
__Project Name__: Rainfall Prediction 
__Project Type__: Machine Learning - Logistic Regression 

Project Summary
The Rainfall Prediction project applies machine learning techniques to classify whether rainfall will occur ("Rainfall") or not ("No Rainfall") based on meteorological data. Using logistic regression, the model leverages key weather features like pressure, dew point, humidity, cloud cover, sunshine duration, wind direction, and wind speed.

This project aims to improve rainfall prediction accuracy, which is critical for agriculture, water resource management, urban planning, and disaster preparedness.

__Problem Statement__
Accurate and timely rainfall prediction is essential for various industries, yet it remains a challenging task due to the complexity and variability of weather patterns. This project seeks to address this challenge through machine learning classification techniques using logistic regression.

__Dataset Description__
The dataset contains historical meteorological parameters that influence rainfall. Below are the input features used in the model:

(Variables in the Dataset)
day: The specific day or date of observation.

pressure: Atmospheric pressure (measured in hPa or mmHg).

maxtemp: Maximum temperature recorded during the day.

temperature: Average temperature for the day.

mintemp: Minimum temperature recorded during the day.

dewpoint: Temperature at which condensation begins (linked to humidity).

humidity: Moisture percentage present in the air.

cloud: Cloud cover percentage in the sky.

rainfall: Amount of rainfall (measured in mm).

sunshine: Duration or intensity of sunlight during the day.

winddirection: Wind direction (measured in degrees or compass direction).

windspeed: Wind speed (measured in m/s or km/h).

__Target Variable (Output)__
- Rainfall (Binary Classification)
  - Class 0 (No Rainfall) - The model predicts dry weather (0).
  - Class 1 (Rainfall) - The model predicts precipitation occurrence (1).

__Model Performance Metrics__    
The model evaluation was performed on test data using precision, recall, F1-score, and accuracy metrics.

__Performance on Class 0 (No Rainfall - Minority Class)__
- __Precision__: 0.55 → 55% of predictions for Class 0 are correct.
- __Recall__: 0.48 → 48% of actual dry weather instances correctly classified.
- __F1-Score__: 0.51 → Balance between precision & recall. 
- __Support__: 23 actual cases in the test set.

__Performance on Class 1 (Rainfall - Majority Class)__
- __Precision__: 0.78 → 78% of rainfall predictions are correct. 
-  __Recall__: 0.82 → 82% of actual rainfall occurrences correctly classified. 
- __F1-Score__: 0.80 → Strong overall performance.
- __Support__: 51 actual cases in the test set.

__Overall Model Accuracy & Averages__
- __Accuracy: 71.6% →__ Percentage of correctly classified instances.
- __Macro Average: 0.66 →__ Average performance across both classes.
- __Weighted Average: 0.71 →__ Accounts for class imbalance.

Making Predictions on New Data
The model can predict rainfall for unknown input data using standardized features:

- __Standardize the input data__
# Standardize the input data
    input_data = (1025.9, 19.1, 72, 99, 1, 9.3, 26.3)  # Sample data
    input_df = pd.DataFrame([input_data], columns=['pressure', 'dewpoint', 'humidity', 'cloud', 'sunshine', 'winddirection', 'windspeed'])
    input_data_standardized = scaler.transform(input_df)  # Apply feature scaling
    
    # Make prediction
    prediction = model.predict(input_data_standardized)
    
    # Print prediction result
    print(prediction[0])  # Output: Binary classification (0 = No Rainfall, 1 = Rainfall)
    print("Prediction result:", "Rainfall" if prediction[0] == 1 else "No Rainfall")

    _Example Output:_
    1
    Prediction result: Rainfall

__Documentation & Tutorials:__
- Scikit-Learn Documentation
- NumPy and Pandas Guides
- Kaggle - Weather Prediction Datasets

__How to Use This Repository__
- Clone the Repository

      git clone https://github.com/RaviSharma1901/Module-6
  
      cd "Module-6/Mid Course Summative Assessment"      (Linux/macOS)
  
      cd "Module-6\Mid Course Summative Assessment"      (Windows)
- Install Dependencies
  
      pip install -r requirements.txt
- Run the Jupyter Notebook
   - Open the notebook in Jupyter and execute code cells for analysis:

          jupyter notebook Mid_Course_Assessment_ML_Case_Study_Ravi_Sahrma.ipynb
     
__About__    
This repository showcases the Rainfall Prediction ML Case Study, using logistic regression to classify rainfall occurrence based on meteorological data. The project contributes to climate analytics, agricultural planning, and disaster preparedness through accurate weather forecasting techniques.

__Objective__: Improve rainfall prediction accuracy using machine learning while addressing weather complexity challenges.
