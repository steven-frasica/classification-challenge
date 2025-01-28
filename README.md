# classification-challenge

This repo analyzes an email filtering system provided by an Internet Service Provider (ISP). As an employee at this ISP, we are tasked with developing a supervised machine learning (ML) model that will accurately detect spam emails and filter them out of customers' inboxes.  

First, we'll split our data into training and testing sets (`X_train, X_test, y_train, y_test`) using `train_test_split`. Value 0 means the email message is not spam, 1 means the message is spam. 

We use `StandardScaler` to scale the features and use the training data to fit our instance of `StandardScaler`.

Prior to building the models, we can make a prediction that the Random Forest Classifier will yield a higher `accuracy_score` than the Logistic Regression model. 

Next, we create the Logistic Regression model and fit it with scaled training data. We use the scaled testing data to create predictions with our model. We also evaluate the performance using the `accuracy_score` and get a score of 0.928.

Afterwards, we create a Random Forest model and fit it as well. We create predictions and calculate an `accuracy_score` of 0.967. 

Our results show that the Random Forest model yields a higher `accuracy_score` than the Logistic Regression model by 0.039, matching the initial prediction. It's a high score, but does not indicate that the model is overfit, so the model appears to be a successful one.

<b>Sources</b></br>
Module-13-Classification/Class-1/Activities/02-Stu_Logistic_Regression/Unsolved/predicting_malware.ipynb - Logistic Regression example </br>
Module-13-Classification/Class-2/Activities/06-Stu_Random_Forest/Unsolved/predict_malware_random_forest.ipynb - Random Forest Example </br>
https://www.geeksforgeeks.org/logistic-regression-vs-random-forest-classifier/ - Further reading on Logistic Regression and Random Forest Classifier </br>

