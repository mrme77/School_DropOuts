
### Table of Contents 

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

The code should run with no issues using Python versions 3.*. Below are the libraries used for this project.
```
import numpy as np
import pandas as pd
from sklearn.linear_model import LogisticRegression
from scipy.stats import chi2_contingency
from sklearn.preprocessing import OneHotEncoder
from sklearn.compose import ColumnTransformer
import matplotlib.pyplot as plt
from sklearn.preprocessing import LabelEncoder
from sklearn.metrics import (
    classification_report,
    confusion_matrix,
    precision_recall_curve,
    auc,
    accuracy_score
)
from xgboost import XGBClassifier
from imblearn.over_sampling import SMOTE
from sklearn.model_selection import train_test_split
import xgboost as xgb
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import r2_score, mean_squared_error
import seaborn as sns

pd.set_option('display.max_columns', None)
import warnings

warnings.filterwarnings("ignore")

%matplotlib inline
```

## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using data gathered from Kaggle (https://www.kaggle.com/datasets/naveenkumar20bps1137/predict-students-dropout-and-academic-success?select=dataset.csv) to answer the following questions:

1. Does marital status contribute to student drop out rates?
2. Are international students less or more likely of dropping-out?
3. Does parental education prevent drop-out?
4. How does gender relate to student drop-outt?
5. Can we fit a ML algorithm to predict students drop-out?

This project leverages the CRISP-DM framework which stands for Cross-Industry Standard Process for Data Mining, is an industry-proven way to guide your data mining efforts. As a methodology, it includes six steps:
1. Business understanding
2. Data understanding
3. Data preparation
4. Modeling
5. Evaluation
6. Deployment
## File Descriptions <a name="files"></a>

There is 1 jupyter notebook available here to showcase work related to the above questions. It is exploratory in searching through the data pertaining to the questions.  Markdown cells were used to assist in walking through the thought process for individual steps.
Here’s a table explaining each of the fields from the dataset (dataset.csv)

| Feature                                   | Description                                                                 |
|-------------------------------------------|-----------------------------------------------------------------------------|
| **Marital Status**                        | The marital status of the student. (Categorical)                           |
| **Application Mode**                      | The method of application used by the student. (Categorical)               |
| **Application Order**                     | The order in which the student applied. (Numerical)                        |
| **Course**                                | The course taken by the student. (Categorical)                             |
| **Daytime/Evening Attendance**           | Whether the student attends classes during the day or in the evening. (Categorical) |
| **Previous Qualification**                | The qualification obtained by the student before enrolling in higher education. (Categorical) |
| **Nationality**                           | The nationality of the student. (Categorical)                              |
| **Mother's Qualification**                | The qualification of the student's mother. (Categorical)                   |
| **Father's Qualification**                | The qualification of the student's father. (Categorical)                   |
| **Mother's Occupation**                   | The occupation of the student's mother. (Categorical)                      |
| **Father's Occupation**                   | The occupation of the student's father. (Categorical)                      |
| **Displaced**                             | Whether the student is a displaced person. (Categorical)                   |
| **Educational Special Needs**             | Whether the student has any special educational needs. (Categorical)       |
| **Debtor**                                | Whether the student is a debtor. (Categorical)                            |
| **Tuition Fees Up to Date**               | Whether the student's tuition fees are up to date. (Categorical)           |
| **Gender**                                | The gender of the student. (Categorical)                                   |
| **Scholarship Holder**                    | Whether the student is a scholarship holder. (Categorical)                 |
| **Age at Enrollment**                     | The age of the student at the time of enrollment. (Numerical)             |
| **International**                         | Whether the student is an international student. (Categorical)            |
| **Curricular Units 1st Sem (Credited)**  | The number of curricular units credited by the student in the first semester. (Numerical) |
| **Curricular Units 1st Sem (Enrolled)**  | The number of curricular units enrolled by the student in the first semester. (Numerical) |
| **Curricular Units 1st Sem (Evaluations)**| The number of curricular units evaluated by the student in the first semester. (Numerical) |
| **Curricular Units 1st Sem (Approved)**  | The number of curricular units approved by the student in the first semester. (Numerical) |
 |

This table should help understanding each field's role and what kind of data it contains.
T

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@josh_2774/how-do-you-become-a-developer-5ef1c1c68711).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Greatest shot-out to Gernerative AI such as ChatGPT and Gemini to help with some doc strings and documentation. Full credit to Kaggle for the data.  You can find the Licensing for the data and other descriptive information at the Kaggle link available [Kaggle](https://www.kaggle.com/datasets/naveenkumar20bps1137/predict-students-dropout-and-academic-success?select=dataset.csv).  Otherwise, feel free to use the code here as you would like! 

