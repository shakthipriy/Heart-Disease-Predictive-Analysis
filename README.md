# Heart-Disease-Prediction

# About the Project
Heart disease prediction is a crucial aspect of preventive healthcare that involves the comprehensive analysis of diverse data points to evaluate an individual's susceptibility to cardiovascular diseases. This process integrates demographic details like age and gender with critical clinical information, including medical and family histories, lifestyle choices, and existing health conditions such as hypertension or diabetes. By examining biomarkers like blood pressure, cholesterol levels, and blood sugar, alongside results from medical tests and imaging studies, predictive models can identify patterns and trends indicative of potential heart issues. Machine learning algorithms play a pivotal role in processing this information, helping stratify individuals into risk categories. The ultimate goal is to enable timely interventions and personalized preventive strategies, empowering individuals to make lifestyle adjustments that can mitigate the risk of heart-related events like heart attacks or strokes. Continuous monitoring and updating of predictive models ensure ongoing accuracy and effectiveness in supporting proactive heart health management.

# About the Dataset
This dataset gives information related to heart disease. The dataset contains 303 rows × 14 columns, target is the class variable which is affected by the other. Here the aim is to classify the target variable to (disease\non disease) using different machine learning algorithms and find out which algorithm is suitable for this dataset.

# Attributes:
1. Age
2. Gender
3. Chest pain type          
4. Resting blood pressure in mm Hg
5. Serum Cholesterol in  mg/dl
6. Fasting Blood Sugar 
7. Resting electrocardiographic results  
8. Maximum heart rate achieved during a stress test
9. Exercise-induced angina
10. oldpeak -ST depression induced by exercise relative to rest   
11. Slope of the Peak Exercise ST Segment
12. Number of major vessels (0-4) colored by fluoroscopy  
13. Thalium stress test result
14. Target

# Built With
* Pandas
* Numpy
* Scikit-Learn
* Seaborn
* Matplotlib
* boxcox
* Pipline


# Getting Started
This will help you understand how you may give instructions on setting up your project locally. To get a local copy up and running follow these simple example steps.
 
# Installation Steps
Follow these steps to install and set up the project directly from the GitHub repository:

1. Clone the Repository

* Open your terminal or command prompt.
* Navigate to the directory where you want to install the project.
* Run the following command to clone the GitHub repository:

https://github.com/shakthipriy/Heart-Disease-Predictive-Analysis.git
 
2. Create a Virtual Environment (Optional but recommended)

It's a good practice to create a virtual environment to manage project dependencies. Run the following command:

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from matplotlib.colors import ListedColormap
from sklearn.model_selection import train_test_split
from scipy.stats import boxcox
from sklearn.pipeline import Pipeline
from sklearn.preprocessing import StandardScaler
from sklearn.neighbors import KNeighborsClassifier
from sklearn.svm import SVC
from sklearn.model_selection import GridSearchCV, StratifiedKFold
from sklearn.metrics import classification_report, accuracy_score
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier

3. To Read the dataset

df = pd.read_csv('heart.csv')
df
#  Dataset Description:
Variable	Description
* age	Age of the patient in years
* sex	Gender of the patient (0 = male, 1 = female)
* cp	Chest pain type:
0: Typical angina
1: Atypical angina
2: Non-anginal pain
3: Asymptomatic
* trestbps	Resting blood pressure in mm Hg
* chol	Serum cholesterol in mg/dl
* fbs	Fasting blood sugar level, categorized as above 120 mg/dl (1 = true, 0 = false)
* restecg	Resting electrocardiographic results:
0: Normal
1: Having ST-T wave abnormality
2: Showing probable or definite left ventricular hypertrophy
* thalach	Maximum heart rate achieved during a stress test
* exang	Exercise-induced angina (1 = yes, 0 = no)
* oldpeak	ST depression induced by exercise relative to rest
* slope	Slope of the peak exercise ST segment:
0: Upsloping
1: Flat
2: Downsloping
* ca	Number of major vessels (0-4) colored by fluoroscopy
* thal	Thalium stress test result:
0: Normal
1: Fixed defect
2: Reversible defect
3: Not described
* target	Heart disease status (0 = no disease, 1 = presence of disease)

# Dataset Basic Information

df.info()

5. Activate the Virtual Environment (Optional)

 # Google colab <Environment_Name>
 

Activate the virtual environment based on your operating system:

# Contributing
We welcome contributions from the community! If you have any ideas or suggestions for improving the project, please feel free to create an issue or submit a pull request.

# Acknowledgements
This project was inspired by the Kaggle dataset on Heart disease  Prediction and the corresponding competition. We also acknowledge the open-source Python libraries used in this project and their contributors.   
