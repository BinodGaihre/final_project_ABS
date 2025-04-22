# final_project_ABS

# **Optimizing Global Freight: Machine Learning Predictions for LCL Transit Times**

## Overview

This project is about building a machine learning model to predict the **Total Actual Days** it takes for the shipment to arrive for a company that one of our team member works in. we have used the dataset for the past three weeks, done some feature engineering (including calculating geo distance between the ports) and Random Forest Regression in this model to helps improve **Delivery Day Window**  for logistics operations.

## Highlights

- Focused on three major tradelanes "TPEB","FEWB", and "TAWB" (covers 90% of the shipments)
- Real operational LCL shipping data was used (only past three weeks dataset)
- Isolation Forest and Local Outlier Factor to removal of the outliers
- Feature engineering calculations as follows:
    1. geo-distance(ocean distance) 
    2. weight-to-volume ratio 
    3. total distance (land distance)
- Random Forest model to predict actual shipment days
- Evaluates the model with **MAE** and **R² Score**
- Visualizes feature importances, actual vs predicted, and residual errors


## Outcomes
- For "TPEB" (55% of the shipments)
    - As per the dataset delivery day window approx. 10 days
    From the model
    - **Mean Absolute Error (MAE):** 5.72 days (Delivery Day Window)  
    - **R² Score:** 0.7583

- For "FEWB" (25% of the shipments)
    - As per the dataset delivery day window approx. 12 days
    From the model
    - **Mean Absolute Error (MAE):** 6.48 days (Delivery Day Window) 
    - **R² Score:** 0.6081

- For "TAWB" (10% of the shipments)
    - As per the dataset delivery day window approx. 11 days
    From the model
    - **Mean Absolute Error (MAE):** 8.31 days (Delivery Day Window)  
    - **R² Score:** 0.6330



## 📁 Project Structure

