Traffic Accident Severity Prediction and
Hotspot Analysis in the United States
Overview
This project aims to develop a machine learning-based predictive model for
determining the severity of traffic accidents in the United States. Leveraging the US
Accidents Dataset (2016–2023), the analysis incorporates environmental, temporal,
and location-based features to improve public safety and emergency response
strategies. The project also includes spatial hotspot detection to identify high-risk
regions.
Objectives
• Predict the severity level of traffic accidents using machine learning.
• Analyze environmental and temporal features impacting accident severity.
• Identify accident hotspots using geospatial data visualization.
• Evaluate and compare the performance of multiple ML models.
Dataset
• Source: US Accidents Dataset (Kaggle.com)
• Duration: February 2016 to March 2023
• Coverage: 49 U.S. states
• Records: Over 7.7 million
• Features Used: Temperature, Humidity, Weather Condition, Start Time, End
Time, Latitude, Longitude, Wind Speed, Visibility, etc.
• Target Variable: Severity
Technologies Used
• Python
• Pandas, NumPy, Matplotlib, Seaborn
• Scikit-learn, XGBoost
• Google Colab
Preprocessing
• Handled missing values using median, mean, and mode.
• Encoded categorical features using LabelEncoder.
• Normalized numerical features using StandardScaler.
Models Used
• Random Forest
• Support Vector Machine (SVM)
• XGBoost
Evaluation Metrics
• Accuracy
• Precision
• Recall
• F1-score
• Support
Model Training & Testing
• Data Split: 80% Training, 20% Testing
• GridSearchCV used for hyperparameter tuning
Results Summary
Model Accuracy
Random Forest 81.67%
SVM 79.54%
XGBoost 83.13%
XGBoost (after
tunning)
83.21%
Accident Hotspot Visualization
• A folium-based heatmap is used to identify accident-prone zones.
• High-density regions include:
California, Texas, Florida
Key Insights
• XGBoost outperformed other models across all metrics.
• Most accidents occurred during peak hours (7–9 AM and 4–6 PM).
• Weather and visibility conditions moderately impact severity.
• Hyperparameter tuning significantly enhanced XGBoost performance.
Cloning the Repository
git clone https://github.com/yogesherla2/DataScienceProject-23032935.git
cd DataScienceProject-23032935
