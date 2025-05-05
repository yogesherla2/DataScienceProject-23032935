Traffic Accident Severity Prediction and Hotspot Analysis (U.S.)

Overview
This project uses machine learning to predict the severity of traffic accidents in the U.S. and identifies high-risk accident areas using geospatial analysis. The goal is to improve public safety and emergency response planning.

Objectives
* Predict accident severity using machine learning.
* Analyze how weather, time, and location affect severity.
* Visualize accident hotspots using maps.
* Compare different machine learning models.

Dataset
* Source: US Accidents Dataset (Kaggle)
* Duration: Feb 2016 – Mar 2023
* Coverage: 49 U.S. states
* Records: ~7.7 million
* Main Features Used:
    * Weather: Temperature, Humidity, Wind Speed, Visibility, Condition
    * Time: Start Time, End Time
    * Location: Latitude, Longitude
* Target: Severity (4 levels)

Tools & Technologies
* Language: Python (Google Colab)
* Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Folium

Data Preprocessing
* Handled missing values (mean/median/mode)
* Encoded categories using LabelEncoder
* Normalized numerical features with StandardScaler

Machine Learning Models
1. Random Forest
2. Support Vector Machine (SVM)
3. XGBoost
4. XGBoost (after tuning)

Training & Evaluation
* Data Split: 80% training / 20% testing
* Tuning: Used GridSearchCV
* Metrics Used: Accuracy, Precision, Recall, F1-score, Support
Model Performance (Accuracy)
Model	Accuracy
Random Forest	81.67%
SVM	79.54%
XGBoost	83.13%
XGBoost (Tuned)	83.21%
Model Performance (Accuracy)
Model	Accuracy
Random Forest	81.67%
SVM	79.54%
XGBoost	83.13%
XGBoost (Tuned)	83.21%
Hotspot Visualization
* Used Folium to create an interactive heatmap
* High accident zones:
    * California
    * Texas
    * Florida

Key Findings
* XGBoost was the best-performing model.
* Most accidents occurred during rush hours (7–9 AM, 4–6 PM).
* Weather and visibility had a moderate impact on severity.
* Hyperparameter tuning improved XGBoost accuracy.


