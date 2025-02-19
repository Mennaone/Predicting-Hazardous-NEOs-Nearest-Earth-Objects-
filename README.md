# Predicting-Hazardous-NEOs-Nearest-Earth-Objects-
## Abstract
This project aims to predict whether a Near-Earth Object (NEO) is hazardous or not using machine learning models. By leveraging a dataset sourced from NASA, which contains information about NEOs from 1910 to 2024, we developed a comprehensive pattern recognition system. The primary goal is to enhance the accuracy and speed of identifying potentially hazardous NEOs, providing valuable insights for planetary defense initiatives. This documentation outlines the methodology, implementation, and evaluation of the developed system, demonstrating its potential to contribute significantly to space safety efforts.

## Introduction
Near-Earth Objects (NEOs) are asteroids and comets with orbits that bring them close to Earth's orbit. While most NEOs are harmless, some have the potential to cause significant damage if they were to collide with Earth. Identifying and classifying these hazardous NEOs is crucial for planetary defense and mitigating potential threats.

This project focuses on building a machine learning-based pattern recognition system to classify NEOs as hazardous or non-hazardous. The system utilizes a dataset provided by NASA, which includes various features such as the object's absolute magnitude, estimated diameter, relative velocity, and miss distance. By applying advanced machine learning algorithms, the system aims to accurately predict the hazard status of NEOs, thereby aiding in early detection and risk assessment.

The objectives of this project are as follows:
- To preprocess and analyze the NEO dataset to extract meaningful features relevant to hazard classification.
- To design and implement machine learning models capable of accurately classifying NEOs based on the extracted features.
- To evaluate the performance of the models using standard metrics such as accuracy, precision, recall, and F1 score.

## Dataset Information
The dataset used in this project is sourced from NASA and contains information about NEOs from 1910 to 2024. The dataset includes various features that describe the physical and orbital characteristics of the NEOs. Here are some key details about the dataset:

### Features:
- **neo_id**: Unique identifier for the NEO.
- **name**: Name of the NEO.
- **absolute_magnitude**: The absolute magnitude (brightness) of the NEO.
- **estimated_diameter_min**: The minimum estimated diameter of the NEO (in kilometers).
- **estimated_diameter_max**: The maximum estimated diameter of the NEO (in kilometers).
- **relative_velocity**: The relative velocity of the NEO with respect to Earth (in kilometers per second).
- **miss_distance**: The closest distance by which the NEO will pass Earth (in kilometers).
- **orbiting_body**: The celestial body that the NEO orbits (e.g., Earth, Mars).
- **is_hazardous**: A binary indicator of whether the NEO is considered hazardous (true) or not (false).

### Data Cleaning and Preprocessing:
- **Handling Missing Values**: Missing values in numerical columns were filled with the mean.
- **Checking for Duplicates**: Duplicate values were checked and handled.
- **Encoding Categorical Variables**: The 'orbiting_body' column was encoded using LabelEncoder.
- **Handling Imbalanced Classes**: SMOTE (Synthetic Minority Over-sampling Technique) was used to handle class imbalance.
- **Standardizing Numerical Features**: Numerical features were standardized using StandardScaler.

## Model Training and Evaluation
### Logistic Regression
The Logistic Regression model was trained on the preprocessed dataset. It achieved a certain level of accuracy, precision, recall, and F1 score. However, while it performed reasonably well, there was room for improvement in its ability to correctly classify hazardous NEOs.

### Decision Tree
The Decision Tree model was also trained on the preprocessed dataset. This model provided a clear and interpretable decision-making process, but its performance was slightly lower than that of the Random Forest model. The Decision Tree model achieved a certain level of accuracy, precision, recall, and F1 score, making it a useful model for understanding the decision paths.

### Random Forest
The Random Forest model was trained on the preprocessed dataset. This model outperformed both the Logistic Regression and Decision Tree models in terms of accuracy, precision, recall, and F1 score. The Random Forest model demonstrated a higher capability in correctly identifying hazardous NEOs, making it a more reliable choice for this classification task.

### Model Comparison
Upon comparing the three models, it was evident that the Random Forest model achieved the highest accuracy score compared to the Logistic Regression and Decision Tree models. The Random Forest model's superior performance in precision, recall, and F1 score further solidified its position as the best-performing model for predicting hazardous NEOs.

### Best Model
The Random Forest model emerged as the best model with the highest accuracy score, making it the most effective model for predicting hazardous NEOs in this project.

## Findings and Insights
- The Random Forest model performed the best with the highest accuracy score.
- The model can be further improved by tuning hyperparameters and exploring additional features.

### Conclusion
This project demonstrates the process of predicting hazardous NEOs using machine learning. The Random Forest model achieved the best performance, and further improvements can be made by tuning hyperparameters and exploring additional features.
