# Global Earthquake Analysis and Tsunami Prediction

This project focuses on analyzing global earthquake data and predicting the occurrence of tsunamis using machine learning techniques. The dataset used is sourced from [Kaggle](https://www.kaggle.com/) and includes historical earthquake and tsunami records.


## Project Overview

The goal of this project is to:

1. Analyze global earthquake data and identify patterns.  
2. Visualize earthquake occurrences using plots and geospatial maps.  
3. Handle outliers and scale numerical features for better model performance.  
4. Predict the occurrence of tsunamis (`tsunami` as target feature) using K-Nearest Neighbors (KNN) and Random Forest classifiers.  
5. Evaluate model performance and compare results.

---

## Dataset

- Source: Kaggle (`earthquake-tsunami` dataset)  
- Features include earthquake magnitude, depth, location (latitude & longitude), and tsunami occurrence.  
- Target variable: `tsunami` (0 = no tsunami, 1 = tsunami)  

---

## Data Preprocessing

- Handled missing values.  
- Scaled numerical features for better model performance.  
- Detected and handled outliers to improve accuracy.  
- Encoded categorical features if needed.  

---

## Exploratory Data Analysis (EDA)

- Visualized key features using **bar plots** and **scatter plots**.  
- Used **GeoPandas** to create geospatial maps to show earthquake occurrences worldwide.  

---

## Feature Engineering and Scaling

- Standardized numerical features.  
- Created new features if necessary to improve model prediction.  

---

## Modeling

Two machine learning algorithms were used to predict tsunami occurrence:

1. **K-Nearest Neighbors (KNN)**  
2. **Random Forest Classifier**  

### KNN Performance

Train Score: 1.0
Test Score: 0.8958

Classification Report:
precision recall f1-score support
0 0.94 0.91 0.92 64
1 0.82 0.88 0.85 32

Accuracy: 0.90

### Random Forest Performance
Train Score: 0.9738
Test Score: 0.9479

Classification Report:
precision recall f1-score support
0 1.00 0.92 0.96 64
1 0.86 1.00 0.93 32

Accuracy: 0.95


---

## Results

- **Random Forest** outperformed KNN with higher test accuracy and better balance between precision and recall.  
- Visualizations highlighted high-risk earthquake zones.  
- Scaling and outlier handling improved model robustness.  

---

## Conclusion

- Random Forest is a reliable model for predicting tsunami occurrence based on earthquake features.  
- The project demonstrates how geospatial analysis and machine learning can be combined to study natural disasters.  
- Future improvements: Include temporal features and larger datasets for better generalization.  
















