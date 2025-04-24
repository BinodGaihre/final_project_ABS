# final_project_ABS

# **Optimizing Global Freight: Machine Learning Predictions for LCL Transit Times**

## Overview

This project involves building a machine learning model to predict the **Total Actual Days** it takes for a shipment to arrive for a company where one of our team members works. We have used data from the past three weeks, performed feature engineering (including calculating the geographical distance between ports), and applied Random Forest Regression to help improve the Delivery Day Window for logistics operations.

## Folder Structure

- /Final_Project_ABS
    - /Final_Code             # Source code for all three tradelanes and the dataset 
    - /Test_Code              # Test codes and files to build the project
    - README.md               # Main documentation file
    - .gitignore              # Files/folders to ignore by Git
    - Final_Project_ABS       # Project Presentation

## Highlights

- Focused on three major tradelanes: TPEB, FEWB, and TAWB (covering 90% of the shipments)
- Utilized real operational LCL shipping data (past three weeks only)
- Applied Isolation Forest and Local Outlier Factor for outlier removal
- Performed feature engineering with the following calculations:
    1. Geo-distance (ocean distance)
    2. Weight-to-volume ratio
    3. Total distance (land distance)

- Used a Random Forest model to predict actual shipment days
- Evaluated the model using **MAE** and **R² Score**
- Visualized feature importance, actual vs. predicted values, and residual errors


## Key Steps

1. Data Cleaning, Feature Selection and Feature Engineering
2. Outlier Fraction Tuning
3. Encoding Categorical Variables
4. Training and Testing
5. Hyperparameter Tuning using Grid Search
6. Evaluation
7. Output Visualization

## Outcomes

- For "TPEB" (55% of the shipments):
    - According to the dataset, the delivery day window is approximately 10 days.
    - From the model:
        - **Mean Absolute Error (MAE)**: 5.72 days (Delivery Day Window)
        - **R² Score**: 0.7583

- For "FEWB" (25% of the shipments):
    - According to the dataset, the delivery day window is approximately 12 days.
    - From the model:
        - **Mean Absolute Error (MAE)**: 6.48 days (Delivery Day Window)
        - **R² Score**: 0.6081

- For "TAWB" (10% of the shipments):
    - According to the dataset, the delivery day window is approximately 11 days.
    - From the model:
        - **Mean Absolute Error (MAE)**: 8.31 days (Delivery Day Window)
        - **R² Score**: 0.6330
 
## Limitations and Future Improvements

- Only 13 weeks of data. The model may better predict with more data, reducing the mean absolute error.
- Unaccounted features that are outside of the dataset could cause potential issues in predictions. Incorporating them would yield better results.
- With the addition of missing and unaccounted features, gradient boosting would be a better option for capturing complex data relationships and is more effective on imbalanced datasets.

## Data Source 
- Provided by Flexport Freight Forwarding Company
