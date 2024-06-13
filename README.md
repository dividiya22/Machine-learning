Machine Learning model:
Classification model:

Introduction:
Classification is used when the output variable is a category or class. The goal is to assign input data into one of several predefined categories. Classification problems can be binary (two classes) or multiclass (more than two classes).

Data set used:
classifying liver cirrhosis stages
https://www.kaggle.com/datasets/aadarshvelu/liver-cirrhosis-stage-classification
Describing the Dataset
1.	N_Days: Number of days the patient has been monitored.
2.	Status: The status of the patient (1: Alive, 0: Dead).
3.	Drug: Type of drug administered to the patient.
4.	Age: Age of the patient.
5.	Sex: Gender of the patient (1: Male, 0: Female).
6.	Ascites: Presence of ascites (1: Yes, 0: No).
7.	Hepatomegaly: Presence of hepatomegaly (1: Yes, 0: No).
8.	Spiders: Presence of spider nevi (1: Yes, 0: No).
9.	Edema: Presence of edema (0: No, 1: Yes but no diuretics, 2: Yes with diuretics).
10.	Bilirubin: Level of bilirubin in the blood.
11.	Cholesterol: Level of cholesterol in the blood.
12.	Albumin: Level of albumin in the blood.
13.	Copper: Level of copper in the blood.
14.	Alk_Phos: Level of alkaline phosphatase in the blood.
15.	SGOT: Level of serum glutamic-oxaloacetic transaminase in the blood.
16.	Tryglicerides: Level of triglycerides in the blood.
17.	Platelets: Number of platelets in the blood.
18.	Prothrombin: Prothrombin time in seconds.
19.	Stage: Stage of liver disease (1-4)
Steps Performed:
1.	Import the libraries and load the dataset liver cirrhosis.
2.	Perform some pandas functions like isnull , describe, info.
3.	Clean the Dataset especially objects column using replace,fill and map as per need.
4.	Visualise the data for classification correlation matrix, heatmap,pair plot.
5.	Then train and test the model and find the accuracy of the classification models.
CLASSIFICATION MODEL USED:
1.	Logistic Regression: Despite its name, it is used for binary classification problems.
2.	Decision Trees: Splits data into branches to classify instances.
3.	Random Forest: An ensemble of decision trees.
4.	Support Vector Machines (SVM): Finds the hyperplane that best separates different classes.
5.	K-Nearest Neighbors (KNN): Classifies instances based on the majority class among the nearest neighbours.
6.	AdaBoost: An ensemble learning method that combines multiple weak classifiers to create a strong classifier. It focuses on instances that were previously misclassified by increasing their weights, forcing subsequent classifiers to pay more attention to these difficult cases.
7.	XGBoost: An advanced implementation of gradient boosting designed for speed and performance. It incorporates regularisation to reduce overfitting and uses second-order derivatives to optimise the loss function, resulting in highly efficient and scalable models.
8.	CatBoost: A gradient boosting algorithm that handles categorical features natively, providing superior performance without extensive preprocessing. It efficiently processes categorical data and incorporates techniques to reduce overfitting, making it robust and effective for a variety of tasks.

 Conclusion:

●	XGBoost achieved the highest accuracy (0.9942), followed closely by CatBoost (0.9926). Both models are highly effective, benefiting from advanced gradient boosting techniques and efficient handling of various data types, especially categorical data in the case of CatBoost.
●	Random Forest (0.988) and Decision Trees (0.9804) also show excellent performance. Random Forest, an ensemble of decision trees, provides robustness and reduces the risk of overfitting compared to a single decision tree.
●	Support Vector Machines (SVM) (0.925) demonstrates strong accuracy, particularly suitable for high-dimensional spaces.

Regression model:

Introduction:
Regression is used when the output variable is a continuous value. The goal is to predict a numerical value based on input data. Regression problems focus on modelling the relationship between the input features and the continuous output variable.

Data set used:
Predicting district wise rainfall normal
https://www.kaggle.com/datasets/rajanand/rainfall-in-india

Describing the Dataset:
●	STATE_UT_NAME: The state or union territory name.
●	DISTRICT: The district within the state or union territory.
●	JAN, FEB, MAR, … DEC: The average monthly rainfall (in centimetres) for each month of the year.
●	ANNUAL: The total annual rainfall received in that district.
●	Jan-Feb, Mar-May, Jun-Sep, and Oct-: These represent cumulative rainfall for specific periods (e.g., Jan-Feb, Mar-May, etc.).

Steps Performed:
1.	Import the libraries and load the dataset Predicting district wise rainfall normal.
2.	Perform some pandas functions like isnull , describe, info.
3.	Clean the Dataset especially objects column using replace,fill and map as per need.
4.	Visualise the data for regression residual plot,line plot,pair plot.
5.	Then train and test the model and find the accuracy of the regression models.
REGRESSION MODEL USED:
1.	Linear Regression: Models the relationship between two variables by fitting a linear equation.
2.	Ridge Regression: A variant of linear regression that includes L2 regularisation. It penalises the sum of the squared coefficients, shrinking them towards zero to prevent overfitting.
3.	Lasso Regression: A variant of linear regression that includes L1 regularisation. It penalises the sum of the absolute values of the coefficients, which can shrink some coefficients to exactly zero, effectively performing feature selection.
4.	Elastic Net: A regularised regression method that combines both L1 (Lasso) and L2 (Ridge) regularisation. It balances the benefits of both methods, providing a more flexible approach to regularisation by controlling the balance with a mixing parameter.

Conclusion:

Ridge Regression is Very close to perfect with a score of 0.9999999999709915. Ridge regression includes L2 regularisation which can help reduce overfitting by penalising large coefficients. The extremely high score suggests it performs nearly as well as linear regression, with added robustness against overfitting.

