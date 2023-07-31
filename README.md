# Interview application predictions
This model must the people into 2 groups: who can enter the interview and who can't. We'll use 3 ML models to solve this classification task.

# Starting with imports
we'll use these libraries/modules

1. Pandas
2. Numpy
3. Scikit Learn
   
                 preprocessing (OrdinalEncoder , StandardScaler)
   
                 model_selection (train_test_split)

                 metrics (accuracy_score)

                 linear_model (LogisticRegression)

                 naive_bayes (GaussianNB)

                 kneighbors (KNeighborsClassifier)
5. matplotlib
6. seaborn
7. plotly

****
# Visualizing the data
We'll use .hist to see instances for understanding the distribution of numeric variables. Use Seaborn's pairplot to see how our feaatures are related to each other (if we see that the blue lines are fully upper than the secondary diagonal then we call the relations 'positive', otherwise 'negative')

Use .info() to see if there are any NONE value (we don't). 

Later we'll use seaborn's .heatmap() to see how much impact our features have to our result, as well use .corr() to see that as well.

****
# Working with data
at first we need to use StandardScaler() to do feature scaling with 'age', 'daily rate' and 'employee number'
then we need to use OrdinalEncoder for 'marial status', 'gender' and 'overtime'

now we have modified dataset and we can to use train_test_split to split our dataset into X_train, X_test, y_train, y_test

****
# Using the models
as it was required for the task we'll use LogisticRgression, Naive Bayes and KNearestClassifier
we will run for loop to fit each of them , then to predict results and check the accuracy for each of them and store them in the dictionaries: scores & predictions
