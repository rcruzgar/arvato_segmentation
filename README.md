# Customer Segmentation and Acquisition - Bertelsmann Arvato

The objective of this project is to create a customer segmentation Report for Arvato Bertelsmann Financial Services, to predict and improve the customer acquisition process of a mail-order company.

## Software

The project has been produced using Python 3 in the Google Colab environment. The default versions of the libraries available in Colab are enough to reproduce the analysis. The basic libraries used are: numpy, pandas, matplotlib, seaborn, sklearn and imblearn.

## Summary

The notebook with the analysis can be found [here](https://github.com/rcruzgar/arvato_segmentation/blob/master/Arvato_Project.ipynb). The main steps of the analysis are:

1. **Data Cleaning and Visualization**: The data has to be processed to identify and clean missing values. An analysis on how many missing values are there per feature is performed to decide on which features to neglect. 
2. **Feature Engineering**: Determining the required number of features that can amount for maximum variance in the dataset using a dimensionality reduction technique like PCA.
3. **Modelling**: First step is to identify the customer segments using unsupervised learning algorithms. A K-means clustering algorithm is used to segment the data into desired number of clusters. In the second step, different supervised algorithms are trained and evaluated in the context of predicting whether a person will be our next customer or not. Algorithms like Logistic Regression, Random Forest, Ada Boosting and Extra Trees are used to make predictions. A hyperparameter tuning algorithm like Grid Search is used to determine the best set of hyper parameters. The previously proposed evaluation metrics is used to determine the best model in this step.
4. **Predictions on test data**: Finally, the best model is used to make predictions on the test data and the predictions are submitted on the Kaggle competition page.

## Data

The project makes use of four datasets:

- *Udacity_AZDIAS_052018.csv*: Demographics data for the general population of
Germany; 891 211 people (rows) x 366 features (columns).
- *Udacity_CUSTOMERS_052018.csv*: Demographics data for customers of a mail order
company; 191 652 people (rows) x 369 features (columns).
- *Udacity_MAILOUT_052018_TRAIN.csv*: Demographics data for individuals who
were targets of a marketing campaign; 42 982 people (rows) x 367 (columns). This is the only dataset with the target variable, which is highly unbalanced (people hiring the services are the minority class).
- *Udacity_MAILOUT_052018_TEST.csv*: Demographics data for individuals who were
targets of a marketing campaign; 42 833 people (rows) x 366 (columns).

I am not allowed to publish the data provided by Arvato Financial Services due to the terms and conditions. However, a description of the different features can be found [here](<https://github.com/rcruzgar/arvato_segmentation/blob/master/DIAS Information Levels - Attributes 2017.xlsx>).















