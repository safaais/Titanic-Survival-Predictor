# Titanic-Survival-Predictor

This Python code builds and evaluates two machine learning models – Logistic Regression and Random Forest – to predict passenger survival on the Titanic. It loads the Titanic dataset, cleans the data, prepares features, and splits the data for training and testing. The models are then trained, tested, and their performance is measured using metrics like accuracy, error rates, and training time. This code provides a basic example of how to use machine learning to analyze and predict outcomes from real-world data, Here are the detailed steps:






1. Import Libraries:

   
•	pandas (pd): Used for data manipulation and analysis.

•	time: Used to measure the training and prediction time of the models.

•	sklearn.model_selection: Used for splitting data into training and testing sets.

•	sklearn.preprocessing: Used for scaling features.

•	sklearn.linear_model: Contains the Logistic Regression model.

•	sklearn.ensemble: Contains the Random Forest Classifier model.

•	sklearn.metrics: Used for evaluating model performance.





2. Load Data:

   
•	Load the Titanic dataset from a CSV file named 'train.csv'.





3. Data Preprocessing:

   
•	Handling Missing Values:

•	Fills missing values in the 'Age' column with the median age.

•	Fills missing values in the 'Embarked' column with the most frequent embarkation point.

•	One-Hot Encoding:

•	Converts categorical features ('Sex' and 'Embarked') into numerical features using one-hot encoding. 





4. Feature Selection:

   
•	The code selects the following features as input for the models:

•	'Pclass' (Passenger Class)

•	'Age'

•	'SibSp' (Number of Siblings/Spouses Aboard)

•	'Parch' (Number of Parents/Children Aboard)

•	'Fare'

•	'Sex_male' (One-hot encoded male indicator)

•	'Embarked_Q' (One-hot encoded indicator for Queenstown embarkation)

•	'Embarked_S' (One-hot encoded indicator for Southampton embarkation)

•	The target variable is 'Survived' (whether the passenger survived or not).




5. Data Splitting:

   
•	The data is split into training and testing sets using 'train_test_split' to allow the models to be trained on a portion of the data and evaluated on unseen data.






6. Feature Scaling:

   
•	The code uses StandardScaler to standardize the features to help to ensure that all features have a similar scale, which can improve the performance of some algorithms.





7. Model Training and Evaluation:
   
   
•	Logistic Regression:

•	A logistic regression model is trained on the training data.

•	Predictions are made on the test data.

•	The model's performance is evaluated using metrics such as accuracy, mean absolute error (MAE), mean squared error (MSE), R² score, and explained variance.

•	The training/prediction time is also recorded.

•	Random Forest Classifier:

•	The same process is repeated for a Random Forest Classifier model.



8. The Output:


  https://github.com/safaais/Titanic-Survival-Predictor/blob/cec7e4c654f16d15bc549496cd90d606a317f1b8/Screenshot%202024-08-12%20082208.png

