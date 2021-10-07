Heart Disease Prediction -
Classification [Supervised Learning]

Notebook link-
https://colab.research.google.com/drive/1eInQFQ124yX0yJsuGDHDAS3YNiQRrnPf?usp=sharing

Dataset: 
https://www.kaggle.com/dileep070/heart-disease-prediction-using-logistic-regression

EDA :
Histogram , countplot, pairplots and distplot are used for exploratory Data Analysis.Pairplot plots pairwise relationship between features of the dataset.Distplot shows the spread of the data and also shows the skewness present in totchol feature of the dataset.Countplot gives value count of people with or without heart disease.Histogram provides distribution of each feature with feature value on x-axis and frequency on y-axis.

Classification Models Applied on Heart Disease Prediction Dataset:
1.Logistic Regression

There are a total of 15 feature out of which 1 feature("education" ) was excluded because it wasn't a useful feature in determining wheter a preson has heart disease or not.I have used single Logistic Regression Algorithm to predict the probability of a person having heart disease or not.I have scaled the features to between 0 to 1 before applying the model to get bettter results.

Results:
Accuracy on testing data  - 87.066%
