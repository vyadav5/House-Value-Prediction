# California-House-Value-Prediction (Data Science Project)

## Table of contents 
1. Aim   
2. Libraries 
3. Project Pipleline

## Objective: 
I created this project because I wanted to learn the process of building a machine learning model in data science. This includes selection, prediction and 
interpretation. The goal for this project is to predict the sale prices for houses in California. I used a dataset from Kaggle which I split into two parts
training and testing using train_test_split method. The dataset has 20640 rows and 10 columns with the target variable as median_house_value and features
as the other columns in the dataset. I used the training dataset to teach our models and the next step was to run the best test data. 

## Libraries used: 
1. Pandas: To handle structured data 
2. Scikit Learn: For Machine learning 
3. NumPy: Solved the purpose for linear algebra and mathematics
4. Seaborn: For data visualization

## Project Pipeline: 
#### Data Cleaning: 
Since Kaggle doesn't provide us with a clean data I managed to do it handling missing values and checking for NaN values as it causes problem in the models.
I tried droppping the ocean_proximity column from the dataset as it is a string value which could further cause issues in our models and dropped null values.

#### Exploratory Data Analysis (EDA):
This is mostly where we use our data visualization techniques. I began with building a histogram of the training data. The distribution of the house prices
were right skewed which means that few of the houses were comparetively expensive. Additionaly, I plotted a heatmap with respect to the correlation of the 
features with the target variable. 

#### Data pre-processing and Feature Engineering:
I performed pre-processing by applying a log transform to house prices to compress outliers for a normal distribution. I also implemented feature engineering
to apply transformations to convert the categories into numbers. I used panda's get_dummies for one hot encoding to convert the ocean_proximity column in 
a binary format of 0s and 1s. 

#### Machine Learning:
Now that we have cleaned, explored and visualized our data. The next step is to build our model for house prices. I have used linear regression and random 
forest to find the best accuracy and precision. To tune the hyperparameters I have used the K-cross validation with GridSearchCV to come up with the best
algorithm and practices. 
