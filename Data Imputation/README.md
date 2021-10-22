
# Data Imputation Techniques:

**Note:** Imputation was done for only `Age` featue.
## Dataset : 
  [Dataset link](https://www.kaggle.com/c/titanic) 
  
  
## Model :

   **Random Forest** model was used to test various imputation techniques.

## Results :


| # | Imputation_Method |Score |
| - | - | - |
| 0 | Median Imputation |  0.877778
| 1 | Most Frequent Imputation |  0.866667
| 2 | Mean Imputation |  0.811111 
| 3 | Deep Learning(Datawig) Imputation |  0.800000

## Conclusion

Although it shown the Median data imputation techniques works well.  There is no perfect way to impute a dataset. Each strategy can perform better for certain datasets and missing data types but may perform much worse on other types of datasets. It's entirely depends on the dataset. And Deep learnig based tend to perform well although here it performed worse. So what imputation technique that need to be used can only be decided after a through EDA(Exploratory Data Analysis).
