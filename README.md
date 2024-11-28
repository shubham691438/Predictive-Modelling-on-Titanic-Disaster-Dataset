# Titanic_dataset: Machine Learning from a Disaster
## Data Collection
Data used in this project is collected from Kaggle website. It consists of two csv files. One is training file and other is for testing pupose. Training file consists of 891 X 12 records where as Testing file consists of 418 X 12 records.

Kaggle Repository: https://www.kaggle.com/competitions/titanic
## Exploratory Data Analysis
In this phase we select the important features and use descriptive analytics to summarize the records. In this way we can perform feature selection. Important libraries used in this step are- matplotlib, seaborn (for data vizualization to analyze trends), pandas and numpy.
## Predictive Modelling (with the help of Pipeline)
In this phase we divided our data into 2 sets for training and validation using train_test_split. We then used various preprocessing steps like simple imputer, ordinal encoding , MinMaxScaling, etc. to preprocess the data before fitting it into our model. We combined all the preprocessing steps using ColumnTransformer and then integrated it with our model using pipeline. The selection of models was based on the scores of those models on the validation data. 
## Recoding the Output
We then used this model to predict target variable for given testing data. The resulted array was then converted into a dataframe with the respective PassengerIds and then stored into a seperate csv file named as submission.csv.
## Saving the model
Then I have used Joblib to save my model for future use. After saving it I have again tested it on validation data to check if it is saved properly and can work as expected or not.
