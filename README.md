# Effectiveness-of-STD-Drug
It is a comptetion project participated on HackerEarth platform. 

# Problem Statement
A new pharmaceutical startup is recently acquired by one of the world's largest MNCs. For the acquisition process, the startup is required to tabulate all drugs that they have sold and account for each drug's effectiveness. A dedicated team has been assigned the task to analyze all the data. This data has been collected over the years and it contains data points such as the drug's name, reviews by customers, popularity and use cases of the drug, and so on. Members of this team are by the noise present in the data.

# Project Description
This is a type of regresssion problem where
my task is to make a sophisticated NLP-based Machine Learning model that has the mentioned features as the input. Also, use the input to predict the base score of a certain drug in a provided case.

# Dataset Description

The dataset has the following columns:

 Variable Name			Description

- patient_id		->	ID of patients
- name _of_drug		->	Name of the drug prescribed
- use_case_fro_drug	->	Purpose of the drug
- review_by_patient	->	Review by patient
- drug_approved_by_UIC		Date of approval of the drug by UIC
- number_of_times_prescribed  ->	Number of times the drug is prescribed
- effectiveness_rating	    ->	Effectiveness of drug
- base_score		    ->	Generated score(Target Variable)

# Approach

When I saw the data and sumbission sample then I came to know that it some kind of problem that is predicting the drug score from the above features to know that how much the drug is effective to the patient by getting the review from patient about the drug.That's why I accepted this problem as regression problem. I can solve this by some of the regression models.

# Data Wrangling
I have check all the column to know is there any null values present in the dataset. But I did not get any null values.

## Main Challenge that I faced the in the data set
The main problem in the dataset is that it have some text data that is review given by patient and drug name as well.
So,In regresion model we can't train the categorical data instead it should be a numerical data. 
 
So the solution for the problem is Called Featuring engineering and Label Encoding 

# Feature Engineering
I created heatmap to get the clear view about the dataset columns to know that how they are related with others column.
I came to know that only few are related with others but If I remove all the columns then it will not give a good result. 
So, I have choosen every feature of train set except Target Variable(base_score).

# Label Encoding
I did label encoding on the dataset columns which are categorical to get a numerical value for traing purpose.

# Tools used
- Python
- Seaborn
- Numpy
- Pandas
- Sci-kit Learn

# Model Building
I used different regression models to train the train dataset.I predicted with all the models.According to the result I came to know that Random Forest Regressor and Decision Tree Regressor are producing same result. 

# Evaluation of Model
I saved 4 subission file of each model.Then I submitted the submission file to the hackerearth platform and I got good score(73.8) with Random Forest Regressor.


# Result
I predicted the base socre with trained model and I saved a submission file as csv file having two column as "patient_id" and "base_score".

***My rank was 156 out of 3712 participants feel free to [check here](https://www.hackerearth.com/challenges/competitive/hackerearth-machine-learning-challenge-std-drug-effectiveness/leaderboard/effectiveness-of-std-drugs-cc3e4cc9/page/4/#)
Happy Learning!***








