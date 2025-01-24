# classification-challenge
Model 13 Challenge - Email Spam Detector

## Summary
Model 13 Supervised Learning - Classification introduces the different classification  models.  It begins with linear models such as logistic regression, then advances to nonlinear models and ensemble methods.<BR>

In this challege, the task is to classify emails to spam and not-spam with supervised ML models.  This is a real-world challenge that ISP and email providers are facing due to the staggering volume of emails.  Two classification models, a logistic regression model and a random forest model, are used to train with the provided dataset.  The accuracy of the mmodels are compared in a preliminary evlauation.

## Data Source
The data is located at [https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv)

Dataset Source: [UCI Machine Learning Library](https://archive.ics.uci.edu/dataset/94/spambase)

## Step 1. Split the data into training and testing sets
The "spam" column in the dataset contains the lables.  The rest of the columns are the features.  Create the features as X and labels as y.  Split them into training and testing sets.

## Step 2. Scale the features.
Use the StandardScaler to scale the split features sets, X_train and X_test to X_train_scaled and X_test_scaled.

## Step 3. Create a logistic regression model.
Create a logistic regression (LR) model, fit it with training data.  Make predictions with the testing data, and obtain the LR model's accuracy score.

## Step 4. Create a random forest model.
Create a random forest (RF) classifier, fit it with training data.  Make predictions with the testing data, and obtain the RF model's accuracy score.

## Step 5. Evaluate the models.
Compute the difference between the LR model's traning accuracy and testing accuracy, and that of the RF classifier.<BR>

Evaluate the performance of the 2 models from their accuracy scores.

    In terms of accuracy, the Random Forest Classifier performs better than the Logistic Regression model in both training and test.  On the other hand, the difference between training and test accuracy is larger for Random Forest Classifier than for Logistic Regression (RF_Diff : LR_Diff = 0.041 : 0.003).  The Random Forest Classifier has a higher variance than Logistic Regression.  This is contrary to the reasoning of my educated guess.<BR>

    After all, I will still choose the Random Forest Classifier for this task over the Logistic Regression which indicates a higher bias in its predictions.