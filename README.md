# Bank_Marketing_Prediction

Find the best strategies to improve for the next marketing campaign. How can the financial institution have a greater effectiveness for future marketing campaigns? In order to answer this, we have to analyze the last marketing campaign the bank performed and identify the patterns that will help us find conclusions in order to develop future strategies.

## Data:

The data used for that project was loaded from Kaggle [Bank Marketing Dataset](https://www.kaggle.com/janiobachmann/bank-marketing-dataset).

## Target value (Deposit Suscriptions):

![alt text](https://github.com/bmd94/Bank_Marketing_Prediction/blob/main/newplot.png)

## Data Preprocessing:

* Outlier Handling: Replace outlier values with median.
* One-Hot-Encoding: Encode Nominal variables describe categories that do not have a specific order to them.
* Mutual information (MI): Measures the dependency between the variables and choose the higher values mean higher dependency.
* Normalize data with StandardScaler.
* Data Augmentation with SMOTE of imblearn.over_sampling
* Split data Train Test (80%, 20%).

## Classification Models:

* ANN (Artificial Neural Network)
* LogisticRegression
* XGBClassifier

##Results:

1. ANN:

| Models        |  Accuracy  | precision  | recall     | f1-score   |
| ------------- |:----------:| ----------:| ----------:| ----------:|
|      no       |    0.90    |    0.89    |    0.92    |    0.90    |      
|      yes      |    0.90    |    0.92    |    0.88    |    0.90    |
|   macro avg   |    0.90    |    0.90    |    0.90    |    0.90    |
| weighted avg  |    0.90    |    0.90    |    0.90    |    0.90    |

2. XGBClassifier:

| Models        |  Accuracy  | precision  | recall     | f1-score   |
| ------------- |:----------:| ----------:| ----------:| ----------:|
|      no       |    0.90    |    0.88    |    0.92    |    0.90    |      
|      yes      |    0.90    |    0.91    |    0.87    |    0.89    |
|   macro avg   |    0.90    |    0.90    |    0.90    |    0.90    |
| weighted avg  |    0.90    |    0.90    |    0.90    |    0.90    |

3. LogisticRegression:

| Models        |  Accuracy  | precision  | recall     | f1-score   |
| ------------- |:----------:| ----------:| ----------:| ----------:|
|      no       |    0.89    |    0.87    |    0.93    |    0.90    |      
|      yes      |    0.92    |    0.92    |    0.86    |    0.89    |
|   macro avg   |    0.89    |    0.89    |    0.89    |    0.89    |
| weighted avg  |    0.89    |    0.89    |    0.89    |    0.89    |
