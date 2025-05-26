# Rainfall Prediction Using Logistic Regression

__Mid Course Assessment__ - ML Case Study 
__Project Name__: Rainfall Prediction 
__Project Type__: Machine Learning - Logistic Regression 

Project Summary
The Rainfall Prediction project applies machine learning techniques to classify whether rainfall will occur ("Rainfall") or not ("No Rainfall") based on meteorological data. Using logistic regression, the model leverages key weather features like pressure, dew point, humidity, cloud cover, sunshine duration, wind direction, and wind speed.

This project aims to improve rainfall prediction accuracy, which is critical for agriculture, water resource management, urban planning, and disaster preparedness.

Problem Statement
Accurate and timely rainfall prediction is essential for various industries, yet it remains a challenging task due to the complexity and variability of weather patterns. This project seeks to address this challenge through machine learning classification techniques using logistic regression.

Dataset Description
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

Target Variable (Output)
Rainfall (Binary Classification)

Class 0 (No Rainfall) - The model predicts dry weather (0).

Class 1 (Rainfall) - The model predicts precipitation occurrence (1).

Model Performance Metrics
The model evaluation was performed on test data using precision, recall, F1-score, and accuracy metrics.

Performance on Class 0 (No Rainfall - Minority Class)
✅ Precision: 0.55 → 55% of predictions for Class 0 are correct. ✅ Recall: 0.48 → 48% of actual dry weather instances correctly classified. ✅ F1-Score: 0.51 → Balance between precision & recall. ✅ Support: 23 actual cases in the test set.

Performance on Class 1 (Rainfall - Majority Class)
✅ Precision: 0.78 → 78% of rainfall predictions are correct. ✅ Recall: 0.82 → 82% of actual rainfall occurrences correctly classified. ✅ F1-Score: 0.80 → Strong overall performance. ✅ Support: 51 actual cases in the test set.

Overall Model Accuracy & Averages
📈 Accuracy: 71.6% → Percentage of correctly classified instances. 📊 Macro Average: 0.66 → Average performance across both classes. 📊 Weighted Average: 0.71 → Accounts for class imbalance.

Making Predictions on New Data
The model can predict rainfall for unknown input data using standardized features:

python
# Standardize the input data
input_data = (1025.9, 19.1, 72, 99, 1, 9.3, 26.3)  # Sample data
input_df = pd.DataFrame([input_data], columns=['pressure', 'dewpoint', 'humidity', 'cloud', 'sunshine', 'winddirection', 'windspeed'])
input_data_standardized = scaler.transform(input_df)  # Apply feature scaling

# Make prediction
prediction = model.predict(input_data_standardized)

# Print prediction result
print(prediction[0])  # Output: Binary classification (0 = No Rainfall, 1 = Rainfall)
print("Prediction result:", "Rainfall" if prediction[0] == 1 else "No Rainfall")
Example Output:
1
Prediction result: Rainfall
Learning Resources
📖 Books:

Introduction to Machine Learning with Python – Andreas C. Müller & Sarah Guido

Pattern Recognition and Machine Learning – Christopher Bishop

Applied Predictive Modeling – Max Kuhn & Kjell Johnson

🎓 Courses:

MIT OpenCourseWare - Machine Learning

Stanford CS229 - Machine Learning

Machine Learning Specialization

📄 Documentation & Tutorials:

Scikit-Learn Documentation

NumPy and Pandas Guides

Kaggle - Weather Prediction Datasets

How to Use This Repository
1️⃣ Clone the Repository
bash
git clone https://github.com/RaviSharma1901/Module-6
cd "Module-6/Mid Course Summative Assessment"
2️⃣ Install Dependencies
bash
pip install -r requirements.txt
3️⃣ Run the Jupyter Notebook
Open the notebook in Jupyter and execute code cells for analysis:

bash
jupyter notebook Mid_Course_Assessment_ML_Case_Study_Ravi_Sahrma.ipynb
About
This repository showcases the Rainfall Prediction ML Case Study, using logistic regression to classify rainfall occurrence based on meteorological data. The project contributes to climate analytics, agricultural planning, and disaster preparedness through accurate weather forecasting techniques.

🎯 Objective: Improve rainfall prediction accuracy using machine learning while addressing weather complexity challenges.
