# Assignment3
Q4.(a) Write your own random forest classifier (this should be relatively easy, given you have
written your own decision tree code) to apply to the Spam dataset [data, information].
Use 30% of the provided data as test data and the remaining for training. Compare
your results in terms of accuracy and time taken with Scikitlearn’s built-in random
forest classifier. (Note that you can’t use in-built decision tree functions to implement
your code. You can modify your decision tree code of the Assignment 1, or code a new
one, to implement a random forest. You can however use the inbuilt train test split of
sklearn to divide the data into train and test.)
(b) Explore the sensitivity of Random Forests to the parameter m (the number of features
used for best split).
(c) Plot the OOB (out-of-bag) error (you have to find what this is, and read about it!) and
the test error against a suitably chosen range of values for m. (Use your implementation
of random forest to perform this analysis.)

Q5.In this question, we will explore the use of
pre-processing methods and Gradient Boosting on the popular Lending Club dataset. You
are provided with two files: loan train.csv and loan test.csv. The dataset is almost as
provided by the the original source, and you may have to make the necessary changes to make
it suitable for applying ML algorithms. (If required, you can further divide loan train.csv
into a validation set for model selection.) Your efforts will be to pre-process the data appro-
priately, and then apply gradient boosting to classify whether a customer should be given
a loan or not. The target attribute is in the column loan status, which has values “Fully
Paid” for which you can assign +1 to, and “Charged off” for which you can assign -1 to. The
other records with loan status values “Current” (in both train and test) are not relevant
to this problem. You can see this link to know more about the different attributes on the
dataset (but please use the provided data, there are several versions of the dataset online.)
Your tasks are to do the following:
(a) Pre-process the data as needed to apply the classifier to the training data (you are free
to use pandas or other relevant libraries. Note that test data should not be used for
pre-processing in any way, but the same pre-processing steps can be used on test data.
Some steps to consider:
• Check for missing values, and how you want to handle them (you can delete the
records, or replace the missing value with mean/median of the attribute - this is
a decision you must make. Please document your decisions/choices in the final
submitted report.)
• Check whether you really need all the provided attributes, and choose the necessary
attributes. (You can employ feature selection methods, if you are familiar; if not,
you can eyeball.)
• Transform categorical data into binary features, and any other relevant columns to
suitable datatypes
• Any other steps that help you perform better
(b) Apply gradient boosting using the function sklearn.ensemble.GradientBoostingClassifier
for training the model. You will need to import sklearn, sklearn.ensemble, and
numpy. Your effort will be focused on predicting whether or not a loan is likely to
default.
