# SalaryPrediction Project

Introduction:

The goal of this project is to predict the salary of a new job posting with the help of job details like education,experience, seniority etc. The model is then later tested on a test data set to validate the accuracy of the model.

The three datasets used for this project are train , test and train salaries. The model is trained using train dataset which has the features jobid, companyid, jobtype, major, degree, industry and the train salaries dataset which has the features jobid and the target variable salary.

The tool used is Python 3 along with its libraries and packages such as numpy, pandas, matplotlib, seaborn and sklearn to do data manipulation, data visualization and building the predictive model.

## Data Cleaning:
The data was checked for missing and Duplicate values. There were five entries with salary <= 0. So a new dataframe was defined with salaries greater than 0.

## Exploratory data analysis(EDA):
Numerical and categorical varibles were identified and summarized separately. There are two numerical features - yearsExperience and milesFromMetropolis. The feature jobId and companyId was not used to build the model. The categorical features are jobType with 8 unique values, degree, major and industry with 5,9,7 unique values respectively.

### Visualizing Target(Salary) Variable:


