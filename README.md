
🚶 Traffic Tracks – Pedestrian Traffic Data Analysis Using Machine Learning

📌 Project Overview

This project, Traffic Tracks, focuses on analysing pedestrian traffic data and applying Machine Learning techniques to understand and predict patterns from pedestrian movement and traffic-related information.

The project uses the Pedestrians in Traffic Dataset from the UCI Machine Learning Repository (Dataset 536). The dataset contains information related to pedestrian positions, timestamps, body orientation, head orientation, and surrounding traffic agents.

The project was developed using Python in Jupyter Notebook and follows a complete Machine Learning workflow including data loading, data understanding, data cleaning, Exploratory Data Analysis (EDA), encoding, outlier analysis, skewness analysis, feature selection, data transformation, feature scaling, model training, and model evaluation.

The main goal is to prepare real-world pedestrian traffic data and develop a Machine Learning model for prediction using the processed features.


---

🎯 Objectives

To understand and analyse the pedestrian traffic dataset.

To perform data preprocessing and cleaning.

To perform Exploratory Data Analysis (EDA).

To analyse missing values and duplicate records.

To handle categorical features using encoding techniques.

To identify and analyse outliers.

To analyse skewness in numerical features.

To select important features using SelectKBest.

To transform skewed data using Power Transformation.

To scale the features using StandardScaler.

To build Machine Learning regression models.

To evaluate and compare model performance using regression metrics.



---

📊 Dataset

The dataset used in this project is the Pedestrians in Traffic Dataset (Dataset 536) from the UCI Machine Learning Repository.

The dataset contains pedestrian tracks collected from a vehicle driving in an urban environment. It includes information about pedestrian positions, timestamps, body orientation, head orientation, and information about other objects or agents present in the environment.

Dataset Source:
UCI Machine Learning Repository – Pedestrians in Traffic Dataset

[UCI Pedestrians in Traffic Dataset](https://archive.ics.uci.edu/dataset/536/pedestrian%2Bin%2Btraffic%2Bdataset?utm_source=chatgpt.com)

Important Features

oid – Object/Pedestrian identification

timestamp – Time information of the recorded track

x – X-coordinate of pedestrian position

y – Y-coordinate of pedestrian position

body_roll – Body roll orientation

body_pitch – Body pitch orientation

body_yaw – Body yaw orientation

head_roll – Head roll orientation

head_pitch – Head pitch orientation

head_yaw – Head yaw orientation

other_oid – Identification of another surrounding object

other_class – Class of the surrounding object

other_x – X-coordinate of the other object

other_y – Y-coordinate of the other object


The dataset contains 4,760 instances and 14 features.


---

🔄 Project Workflow

Dataset
   ↓
Data Loading
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Missing Value Analysis
   ↓
Duplicate Value Analysis
   ↓
Exploratory Data Analysis (EDA)
   ↓
Categorical Encoding
   ↓
Correlation Analysis
   ↓
Outlier Analysis
   ↓
Skewness Analysis
   ↓
Feature Selection
   ↓
Power Transformation
   ↓
Feature Scaling
   ↓
Train-Test Split
   ↓
Machine Learning Model
   ↓
Model Evaluation
   ↓
Performance Analysis


---

🔍 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the structure, distribution, and relationships between the features in the dataset.

The following EDA steps were performed:

1. Data Information

df.info() was used to understand the number of records, columns, data types, and non-null values in the dataset.

2. Statistical Analysis

df.describe() was used to obtain statistical information such as mean, standard deviation, minimum, maximum, and quartile values of numerical features.

3. Dataset Shape

df.shape was used to identify the number of rows and columns present in the dataset.

4. Column Analysis

df.columns was used to identify and understand the features available in the dataset.

5. Missing Value Analysis

Missing values were checked using:

df.isnull().sum()

This helped identify columns containing missing data and determine the required preprocessing steps.

6. Duplicate Value Analysis

Duplicate records were checked using:

df.duplicated().sum()

This helped identify repeated records in the dataset.

7. Correlation Analysis

Correlation analysis was performed to understand the relationship between numerical features.

8. Heatmap Visualization

A correlation heatmap was created using Seaborn to visually understand the strength and direction of relationships between features.

9. Box Plot Analysis

Box plots were used to analyse the distribution of numerical features and identify unusual observations.

10. Outlier Analysis

Potential outliers were identified from the numerical features using box plot analysis and statistical observations.

11. Skewness Analysis

Skewness was analysed to understand whether numerical features were normally distributed or highly skewed.


---

🛠️ Data Preprocessing

The dataset was prepared for Machine Learning using several preprocessing techniques.

Missing Values

The dataset was checked for missing values and the required preprocessing was performed before model development.

Duplicate Records

Duplicate records were identified and handled during the data cleaning process.

Categorical Encoding

Categorical/object features were converted into numerical form using Label Encoding, so that they could be used by Machine Learning algorithms.

Outlier Analysis

Numerical features were analysed using box plots to identify potential outliers.

Skewness Handling

Skewed numerical features were identified through skewness analysis.

Feature Selection

SelectKBest was used to select the most important features for the Machine Learning model.

Power Transformation

Power Transformation was applied to improve the distribution of skewed numerical features.

Feature Scaling

Finally, StandardScaler was applied to standardize the selected features and bring them to a common scale.


---

🤖 Machine Learning Algorithm

After completing the preprocessing and feature engineering steps, the processed dataset was divided into training and testing datasets using an 80:20 train-test split.

A Linear Regression model was implemented to perform prediction using the processed pedestrian traffic features.

Linear Regression

Linear Regression is a supervised Machine Learning algorithm used to predict a continuous numerical output based on one or more input features.

The model was trained using the training dataset and then used to predict values for the testing dataset.


---

📈 Model Evaluation

Since the project uses a regression approach, regression evaluation metrics were used to measure the performance of the model.

Mean Absolute Error (MAE)

MAE measures the average absolute difference between the actual values and predicted values.

A lower MAE indicates better prediction performance.

Mean Squared Error (MSE)

MSE calculates the average squared difference between actual and predicted values.

A lower MSE indicates better model performance.

R² Score

R² Score measures how well the model explains the variation in the target variable.

A value closer to 1 indicates better model performance.

The model was evaluated using:

MAE
MSE
R² Score


---

💻 Technologies Used

Python

Jupyter Notebook

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn




---


📌 Results

The Traffic Tracks project successfully follows a complete Machine Learning workflow for analysing pedestrian traffic data.

The dataset was explored and preprocessed through EDA, missing-value analysis, duplicate analysis, encoding, correlation analysis, outlier analysis, skewness analysis, feature selection, Power Transformation, and StandardScaler.

After preprocessing, the data was divided into training and testing sets and a Linear Regression model was developed.

The model performance was evaluated using MAE, MSE, and R² Score to understand the prediction accuracy of the regression model.


---

🎓 Conclusion

This project demonstrates how Machine Learning can be applied to real-world pedestrian traffic data.

The project covers the complete workflow, starting from data loading and understanding, followed by data cleaning, Exploratory Data Analysis, encoding, correlation analysis, outlier analysis, skewness analysis, feature selection, Power Transformation, and feature scaling.

Finally, a Linear Regression model was trained and evaluated using appropriate regression metrics.

Overall, the project provides practical experience in analysing real-world traffic data and applying Machine Learning techniques for predictive analysis.

