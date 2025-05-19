
# Predicting Next-Day Rain in Australia 🌧️

This project uses real-world weather data from Australia to build a machine learning model that predicts whether it will rain the next day. The dataset comes from the Australian Bureau of Meteorology and is publicly available on Kaggle.

{ 

# 🧹 Data Cleaning & Preprocessing Tool
![Screenshot 2025-05-19 201752](https://github.com/user-attachments/assets/2ae9a3d5-f5fb-482b-b9df-b74ffe75a300)

This project is part of the SkillHIGH Minor Project for internship training, focusing on automating essential data preprocessing tasks to ensure datasets are clean, consistent, and ready for analysis or machine learning applications.

## 🔧 Features

* **Handling Missing Values**: Identify and address null values using strategies like mean, median, or mode imputation.
* **Duplicate Removal**: Detect and eliminate duplicate records to maintain data integrity.
* **Outlier Detection**: Utilize Z-score or Interquartile Range (IQR) methods to identify and handle outliers.
* **Data Normalization**: Apply techniques such as Min-Max Scaling to standardize data ranges.
* **Automated Reporting**: Generate visualizations and summaries to provide insights into the cleaning process.

## 🛠️ Technologies Used

* **Python**: Core programming language for implementation.
* **Pandas**: Data manipulation and analysis.
* **NumPy**: Numerical computations.
* **Matplotlib & Seaborn**: Data visualization.
* **Scikit-learn**: Preprocessing utilities and algorithms.([GitHub][1], [GitHub][2], [GitHub][3])


}
🔗 View Project Notebook on Kaggle
👉 [https://www.kaggle.com/code/krishnayadav456wrsty/predicting-next-day-rain](https://www.kaggle.com/code/krishnayadav456wrsty/predicting-next-day-rain)

---

## 🔍 Project Overview

Predicting rainfall is essential in agriculture, water management, and disaster prevention. This project performs:

* Data cleaning and preprocessing
* Feature selection
* Classification model training using Random Forest
* Model evaluation
* Visualization of predictions

---

## 🛠️ Technologies and Libraries

* Python
* Jupyter Notebook
* Pandas & NumPy
* Seaborn & Matplotlib
* Scikit-learn

---

## 🧹 Data Cleaning Steps

1. ✅ Handling Missing Values:

   * Columns with significant missing data were dropped.
   * Remaining missing values were imputed using mean, median, or mode depending on the feature type.

2. ✅ Duplicate Removal:

   * Duplicate rows were checked and removed to prevent skewed learning.

3. ✅ Outlier Detection:

   * Outliers were handled using the Interquartile Range (IQR) method to improve model robustness.

---

##  Model: Random Forest Classifier

* Target variable: RainTomorrow (Yes or No)
* Training/Test split: 80/20
* Evaluation metric: Accuracy, Precision, Recall, F1-score

---

## 📈 Model Performance

✔️ Accuracy: 88.17%

📊 Classification Report:

| Class       | Precision | Recall | F1-Score | Support |
| ----------- | --------- | ------ | -------- | ------- |
| No Rain (0) | 0.89      | 0.98   | 0.93     | 17,855  |
| Rain (1)    | 0.75      | 0.30   | 0.43     | 3,108   |

* Weighted Average F1-score: 0.86
* Macro Average F1-score: 0.68

---

## 🌦️ Prediction Distribution

| Label   | Count  | Percentage |
| ------- | ------ | ---------- |
| No Rain | 19,711 | 94.10%     |
| Rain    | 1,252  | 5.90%      |

📊 Bar chart visualizing prediction percentage was included to illustrate class imbalance.

![Screenshot 2025-05-10 095204](https://github.com/user-attachments/assets/437778ee-e6bd-43a7-94d0-8d966706a495)
![Screenshot 2025-05-10 095341](https://github.com/user-attachments/assets/ea92eb70-1a00-4b1e-ae68-7e9d5f94bd5e)

---

![Screenshot 2025-05-10 094713](https://github.com/user-attachments/assets/fb0497f1-41f7-4bc6-85d1-04c27f1f3417)

---

## 📌 Conclusion

This model demonstrates solid overall accuracy and strong performance on the majority class (No Rain). However, predicting rain events remains challenging due to class imbalance and requires further improvements like:

* SMOTE or other resampling techniques
* Ensemble or deep learning models
* Feature engineering and domain knowledge

