
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
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import r2_score, mean_squared_error
import AllTogether as t
import seaborn as sns
%matplotlib inline
```

## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using syintethic data inspired from a Kaggle dataset to accomplish the following:
1. What Family Factors Contribute to Student Dropout Rates?
2. Do Extracurricular Activities Reduce the Likelihood of Dropping Out?
3. Does Access to Educational Support Systems Help Prevent Dropout?
4. How Does Alcohol Consumption Relate to Student Dropout?
5. What ML model can we use to predicate DropOuts?

## File Descriptions <a name="files"></a>

There are 1 jupyter notebook available here to showcase work related to the above questions. It is exploratory in searching through the data pertaining to the questions.  Markdown cells were used to assist in walking through the thought process for individual steps.  
Here’s a table explaining each of the fields from the dataset (student_data.csv)

| Field                           | Description                                                                                  | Example                                      |
|---------------------------------|----------------------------------------------------------------------------------------------|----------------------------------------------|
| **Name_of_the_school_attended** | Name of the school the student is attending.                                                | MS                                           |
| **Gender**                      | Gender of the student.                                                                       | M (Male), F (Female)                        |
| **Age**                         | Age of the student.                                                                         | 15                                           |
| **Address**                     | Type of residence: urban or rural.                                                           | U (Urban), R (Rural)                        |
| **Family_Size**                 | Size of the family: greater than 3 or less than or equal to 3.                              | GT3 (Greater than 3), LE3 (Less than or equal to 3) |
| **Parental_Status**             | Living arrangement of the parents.                                                            | A (Living together), T (Living apart)       |
| **Mother_Education**            | Education level of the mother on a scale from 0 to 4.                                         | 2                                            |
| **Father_Education**            | Education level of the father on a scale from 0 to 4.                                         | 3                                            |
| **Mother_Job**                  | Type of job held by the mother.                                                               | Teacher, Nurse                               |
| **Father_Job**                  | Type of job held by the father.                                                               | Engineer, Driver                             |
| **Reason_for_Choosing_School**  | Reason for selecting the school.                                                               | Course, Location, Reputation                |
| **Guardian**                    | Guardian of the student.                                                                     | Mother, Father                               |
| **Travel_Time**                 | Time taken to travel to school in minutes.                                                   | 30                                           |
| **Study_Time**                  | Weekly study hours on a scale from 1 to 4.                                                    | 2                                            |
| **Number_of_Failures**          | Number of past class failures.                                                                | 1                                            |
| **School_Support**              | Whether the student receives extra educational support.                                       | Yes, No                                      |
| **Family_Support**              | Whether the family provides educational support.                                              | Yes, No                                      |
| **Extra_Paid_Class**            | Participation in extra paid classes.                                                          | Yes, No                                      |
| **Extra_Curricular_Activities** | Involvement in extracurricular activities.                                                    | Yes, No                                      |
| **Attended_Nursery**            | Attendance in nursery school.                                                                 | Yes, No                                      |
| **Wants_Higher_Education**      | Desire to pursue higher education.                                                            | Yes, No                                      |
| **Internet_Access**             | Availability of internet at home.                                                             | Yes, No                                      |
| **In_Relationship**             | Romantic relationship status.                                                                  | Yes, No                                      |
| **Family_Relationship**         | Quality of family relationships on a scale from 1 to 5.                                       | 4                                            |
| **Free_Time**                   | Amount of free time after school on a scale from 1 to 5.                                      | 3                                            |
| **Going_Out**                   | Frequency of going out with friends on a scale from 1 to 5.                                   | 2                                            |
| **Weekend_Alcohol_Consumption** | Alcohol consumption on weekends on a scale from 1 to 5.                                      | 1                                            |
| **Weekday_Alcohol_Consumption** | Alcohol consumption on weekdays on a scale from 1 to 5.                                      | 2                                            |
| **Health_Status**               | Health rating of the student on a scale from 1 to 5.                                          | 3                                            |
| **Number_of_Absences**          | Total number of absences from school.                                                         | 10                                           |
| **Grade_1**                     | Grade received in the first assessment.                                                       | 14                                           |
| **Grade_2**                     | Grade received in the second assessment.                                                      | 15                                           |
| **Final_Grade**                 | Final grade received, typically the end-of-year grade (G3).                                   | 16                                           |
| **Dropped_Out**                 | Indicator of whether the student has dropped out of school.                                   | True, False                                  |

This table should help you understand each field's role and what kind of data it contains.
There is an additional `.py` file that runs the necessary code to obtain the final model used to predict salary.

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@josh_2774/how-do-you-become-a-developer-5ef1c1c68711).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to Stack Overflow for the data.  You can find the Licensing for the data and other descriptive information at the Kaggle link available [here](https://www.kaggle.com/stackoverflow/so-survey-2017/data).  Otherwise, feel free to use the code here as you would like! 

