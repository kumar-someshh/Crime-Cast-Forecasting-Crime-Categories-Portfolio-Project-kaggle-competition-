# Crime-Cast: Forecasting Crime Categories (Portfolio Project) (Kaggle-competition)

# Steps involved:
## Look at the big picture

- My first question will be what exactly the business objective is? I am asked to build a model to really understand which algorithm to choose, and which performance measure to use I need to understand How does the company expect to use and benefit from this model.
- The second question would be is there any current solution? That could be my reference for performance.
By leveraging machine learning techniques, I need to analyze this rich dataset to predict crime categories, enhance law enforcement strategies, and bolster public safety measures.
-  What kind of training supervision the model will need: is it a supervised, unsupervised, semi-supervised, self-supervised or reinforcement learning task.
  Here we have a target variable that has certain categories so its a supervised learning and classification task. -> It's a batch learning task.

## Get The data 
## Exploratory data analysis (EDA)

- Key insights from EDA
- Location: contains string values, needs TF-IDF type encoding
- Cross_Street: close to 82% of values are missing, dropping the column seems the right approach here
- Latitude and Longitude: correlated to each other, needs encoding
- Date_reported, Date_occured, Time_occured: right now dtype is float, need to convert to datetime and extract features out of it like day, month etc.
- Area_Id: 21 distinct values, correlated with Area_name and Reporting_dist_number
- Area_Name: 21 distinct values(string)
- Reporting_district_number: 1120 unique numeric values highly correlated with Area_Id
- Part1-2: only two values 1 and 2
- Modus_operandi: a bunch of integer codes, don't know what to do with them
- Victim_Age: some absurd values are there like 0
- Victim_Sex: 4 categories, some missing values
- Victim_Discent: 17 categories coded with alphabets(string) and some missing values.
- Premise_code: real numbers 217
- Premsise_description: string description
- Weapon_used_code: real number, 63% missing values, imbalance
- Weapon_description: string, lot of missing values 63%
- Status and Status_description: categories of 5, one category is highly dominating, imbalanced, and highly correlated to each other.

## Data preprocessing
- Missing values (Imputation)
- Addressed outliers in data
- Encoding of features
- Feature Scaling

  ## Data splitting (training | validation)
  ## Feature selection
  ## Baseline model
  ## Model training
  ## Hyperparameter tuning (HPT)
  ## Testing on the test data
  

