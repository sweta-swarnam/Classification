## Problem statement
Using a simple data set classifier to distinguish between different types of fruits, I have four types of fruits in the dataset Apple, Mandarin, Orange Lemon few dozen oranges, lemons and apples of different varieties. Try to find accuracy on the basis of 3 types of classification process randomly.
•	Support Vector Machine
•	Decision Tree
•	Logistic regression
 
## Data understanding
In this fruit data types, we have four types of fruits in the dataset few dozen oranges, lemons and apples of different varieties, and recorded their measurements in a table. Each row of the dataset represents one piece of the fruit as represented by several features .We have 59 pieces of fruits and 7 features in the dataset.
•	Fruit label
•	Fruit name
•	Fruit subtype
•	Mass
•	Width
•	Height
•	Color score
The data is pretty balanced except mandarin. There was missing value in the column of color score and in height column total no of missing value is 43.Box plot for each numeric variable will give us a clearer idea of the distribution of the input variables. Some pairs of attributes are correlated (mass and width). This suggests a high correlation and a predictable relationship. We can see that the numerical values do not have the same scale. We will need to apply scaling to the test set that we computed for the training set.


## Data prepressing

Data Cleaning: The data can have many irrelevant and missing parts. To handle this part, data cleaning is done in this data in height column there are missing value from index 0 to 2, 8 to 12,18 to 27 and 33 to 58.In color score all the value are missing.
Missing Data:
This situation arises when some data is missing in the data. It can be handled in various ways.
1.	Ignore the tuples: This approach is suitable only when the dataset we have is quite large and multiple values are missing within a tuple. In this data set we cannot use this techniques because this dataset is not so large.
2.	Fill the Missing values: There are various ways to do this task. We can choose to fill the missing values manually, by attribute mean or the most probable value. In this data set I used most probable value to fill the missing value.
 
## Model building
•	In this classification techniques I used mainly three techniques to classify the data set.
•	Those are Support Vector Machine, Decision Tree and Logistic regression.
Support Vector Machine-
Support vector machines are supervised learning models with associated learning algorithms that analyze data used for classification and regression analysis. SVMs are used in text categorization, image classification, handwriting recognition and in the sciences.
In this scenario support Vector Machine use to find out the classification among 4 types of fruits those are Apple, Mandarin, Orange and Lemon. Here, used to find out classification in Fruits.
This classification called as a text categorization.
Decision Tree-
A decision tree is a decision support tool that uses a tree-like graph or model of decisions and their possible consequences, including chance event outcomes, resource costs, and utility. It is one way to display an algorithm that only contains conditional control statements.
In this scenario decision tree use to find out the classification among 4 types of fruits those are
Apple, Mandarin, Orange and Lemon. Logistic regression-
Logistic regression is a statistical analysis method used to predict a data value based on prior observations of a data set. A logistic regression model predicts a dependent data variable by analyzing the relationship between one or more existing independent variables.
Logistic regression mainly use to find classification among less no of class. In this scenario we are finding classification among 4 types of fruits those are Apple, Mandarin, Orange and Lemon.


## Model Evaluations

Model evaluation metrics are required to quantify model performance. The choice of evaluation metrics depends on a given machine learning task (such as classification, regression, ranking, clustering, topic modeling, among others). Some metrics, such as precision Recall are useful for multiple tasks. Supervised learning tasks such as classification and regression constitutes a majority of machine learning applications. In this article, we focus on metrics for these two supervised learning models.
 
Evaluations Matrix-
In this section we will review some of the metrics used in classification problems, namely:
•	Classification Accuracy
•	Confusion matrix
•	Logarithmic Loss
•	Area under curve (AUC)
•	F-Measure
For simplicity of the project, I have utilized precision based accuracy score for model evaluation.

## Result

Classifier	Value of training	Value of test
Decision Tree	1.00	0.67
Support Vector Machine	0.61	0.33
Logistic Regression	0.70	0.40
According to classifier, if we are comparing out of these 3 techniques Decision tree, Support vector and Logistic Regression for classification Decision Tree (67% accuracy on test data) is giving better output as compare to other 2 techniques. Hence we are using Decision Tree classifier for this problem statement.

## Problem solved

In the basis of 7 Features we are able to successfully classify the given sample into respective fruit classes those are Apple, Man
