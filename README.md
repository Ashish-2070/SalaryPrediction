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

![Target Variable](https://user-images.githubusercontent.com/63967431/88532182-c2dd4280-d021-11ea-866d-2f5b5b8265e3.JPG)

In the target variable's plot there were some suspicious potential outliers. 1.5 IQR rule was used to find the upper and lower bound of suspected outliers. There are 20 Junior positions with salary above the upper bound 220.5. But later after more examination of the data, it was clear that those data should be good as those entries had atleast 18 years of experience and almost most of them has masters or doctoral degree.

### Relationship between Target and Input Variable:

#### Degree VS Salary
<img width="334" alt="Degree VS Salary" src="https://user-images.githubusercontent.com/63967431/88532398-27989d00-d022-11ea-9ae0-f0bcc9a5344c.PNG">

#### Industry VS Salary
<img width="318" alt="Industry VS Salary" src="https://user-images.githubusercontent.com/63967431/88532514-5ca4ef80-d022-11ea-88bd-91407653da72.PNG">



