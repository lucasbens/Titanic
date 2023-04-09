# Kaggle Titanic Project - README

This is the README file for the [Kaggle Titanic project](https://www.kaggle.com/c/titanic), in which I achieved an [accuracy of 78.468%](https://www.kaggle.com/code/lucasbensaid/titanic-example-top-10) on the leaderboard (top 10%).

## Project Overview

The Kaggle Titanic project is a classification problem in which we are asked to predict the survival of passengers on the Titanic based on various features such as age, gender, class, and fare. The train dataset contains information on 891 passengers, of which we are provided with the survival outcome. The goal is to use this information to build a model that can predict the survival outcome for the 418 passengers of the test set. 

## Approach

My approach to solving this problem involved several steps:


1. **Import data:** Train dataset: 891 labeled passengers. Test set: 418 unlabeled passengers. 

2. **Exploratory Data Analysis (EDA):** I then performed EDA to gain insights into the data and understand the relationships between different variables. This helped us identify which variables were most important for predicting survival.

3. **Feature Engineering:** Based on our EDA, I created new features such as `connected_survival`, `FamilySize` and `Title` to capture additional information. I also cleaned the data by removing irrelevant columns and filling in missing values. 

4. **Model Selection:** I tested several models on the data using LazyPredict library. I selected the models with the best performance on the validation set. I tested also neural networks.

5. **Hyperparameter Tuning:** I fine-tuned the hyperparameters of our selected models, including logistic regression, decision trees, and random forests using grid search. Random forests had the best perfomance.

6. **Submission:** I submited the final predictions to the Kaggle competition achieving an [accuracy of 78.468%](https://www.kaggle.com/code/lucasbensaid/titanic-example-top-10) on the leaderboard (top 10%).


## Files in the Repository

This repository contains the following files:

- `train.csv` and `test.csv`: The original data provided by Kaggle.
- `Kaggle_Titanic.ipynb`: The Jupyter notebook containing our code for data cleaning, EDA, feature engineering, model selection, hyperparameter tuning, and ensemble methods.
- `submission.csv`: The final predictions submitted to the Kaggle leaderboard.

## Dependencies

To run the code in the Jupyter notebook, you will need the following libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`
- `lightgbm`
- `lazypredict`

You can install these libraries using `pip` or `conda`.

## Conclusion

I was able to achieve an [accuracy of 78.468%](https://www.kaggle.com/code/lucasbensaid/titanic-example-top-10) on the Kaggle Titanic leaderboard by using a combination of data cleaning, EDA, feature engineering, model selection and hyperparameter tuning. My approach was based on sound statistical principles and the latest techniques in machine learning. I hope that my code and methods will be useful for others working on this problem or similar classification problems in the future.
