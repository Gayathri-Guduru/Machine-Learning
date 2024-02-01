# Machine-Learning project on Autism Spectrum Disorder Screening

The goal of the Autism Screening and Assessment Clinic is to provide identification of Autism Spectrum Disorder (ASD) to inform intensive behavioral treatment, while addressing specific skill deficits and enhancing community inclusion.

Objective is to predict the likelihood of a person having autism using survey and demographic variables. The target variable is Class_ASD. It is a classification problem. Number of Instances (records in the data set): 704 (rows) Number of Attributes (fields within each record): 21 (columns)

I divided the provided data into scaled and unscaled categories for this dataset using PCA, a feature engineering technique, and I tested each category’s performance. Prior to performing PCA, I first removed the target column. Once the PCA was scaled, two graphs were drawn, with the first principle component explaining 4.9% of the variance and the second principle component explaining 2.6%. First principle component accounts for 89.6% of the variance in the unscaled PCA plot, while second principle component accounts for 6.5% of the variance. The overall variance was 96.1%. We can conclude that unscaled PCA perform better than scaled PCA at reducing the dimensions of the data.

The main idea of the project is to predict the likelihood of a person having autism using survey and demographic variables. The target variable is Class_ASD.
There are 20 predictor variables. 10 are behavioral features (AQ-10-Adult) plus 10 are individual characteristics. Therefore, the idea of the project is to predict ASD cases based on these 20 features. Hence, it is a binary classification problem I.e, to predict patient has ASD” or “patient does not have ASD”.  

I divided the provided data into scaled and unscaled categories for this dataset using PCA, a feature engineering technique, and I tested each category's performance. Prior to performing PCA, I first removed the target column. Once the PCA was scaled, two graphs were drawn, with the first principle component explaining 4.9% of the variance and the second principle component explaining 2.6%. First principle component accounts for 89.6% of the variance in the unscaled PCA plot, while second principle component accounts for 6.5% of the variance. The overall variance was 96.1%. We can conclude that scaled and unscaled PCA both perform better than scaled PCA at reducing the dimensions of the data.

Binary classification- Binary classification problem with the goal of being able to classify new instances like we have a new adult patient with certain characteristics which are similar to the cases of autism patients. So I would want to predict what level of probability that individual has of getting autism. None of the machine learning algorithms that we use make assumptions of normality. So we will apply min max Normalization on the dataset.

I intend to employ the confusion matrix, AUC, precision, recall, F1-score and ensemble method to evaluate a classification model. I will assess each model using a selected metric, and I may then work on boosting the grade by tuning (hyperparameters).

The models I intend to perform this task is  : 
SVM - SVM is used for classification and Regression. Create Bayes line or decision boundaries aka hyperplane and segregate end dimension spaces into classes. Its useful in putting new data points in the correct category in the future for analysis.

Decision Trees- Decision Trees are useful supervised Machine learning algorithms that have the ability to perform both regression and classification tasks. We have internal nodes that represent dataset features and branches that represent decision rule and each leaf node represent outcomes.

Logistic Regression - It predicts the outcome of categorical dependant variables. The outcome must be a discrete value. So it gives either a yes or no and provides values between 0 and 1. This describes if the patient has ASD or not.

ANN- Artificial Neural Networks (ANN) are algorithms based on brain function and are used to model complicated patterns and forecast issues. This mimics human neural network pattern.

Except for the decision tree, the entire model was successful. Both 1 normal person and 1 ASD patient were incorrectly classified as being ASD patients (false positive) (false negative). In order to build the decision tree model, I used k-fold cross validation and 10 fold cross validation. The entire set of data is passed to the train function, which splits the tests. In the end, k-fold cross validation yielded an accuracy of 0.9914475 at cp= 0.489418.

Using random sampling and row replacement, I divided the dataset into training and testing sets. 80% of the data is used as the training set, and 20% as the validation set.


