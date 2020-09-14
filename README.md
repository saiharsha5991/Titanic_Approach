# Titanic_Approach
In this kernal Iam going to explain the famous Titanic Challenge. The challenge is to use machine learning to create a model that predicts which passengers survived the Titanic shipwreck I have tried out 2 approches, one explained in this notebook, the other approach exaplained in another notebooks with title 'Titanic_Approach-2_Part-II' &amp; 'Titanic_Approach-2_Part-II'

Kaggle Notebook Link :https://www.kaggle.com/saiharsha1234/titanic-approach1-harsha

Kaggle Notebook Link :https://www.kaggle.com/saiharsha1234/titanic-approach2-part1 

Kaggle Notebook Link :https://www.kaggle.com/saiharsha1234/titanic-approach2-part2 .

Programing language used : Python 

Libraries used : pandas, numpy, seaborn, sklearn 

Concepts : Imputation

Machine Learning Algorithms : Random Forest,Decision Tree,Logistic Regression,KNN,Support Vector Machines,Naive Bayes,Stochastic Gradient Decent

***Preprocessing steps we are going to explained on 'Titanic_Approach-1'***

*)Extracted 'NAME' column from both train and test datasets. A column 'Title' is created and the extracted names are put in that column .For each title checked for 'SEX' column if a name is male or female

IN THIS I FILLED THE NULL VALUES OF 'AGE' COLUMN IN TWO DIFFERENT TYPES

**METHOD II**

*)filled the null values of the 'Age' column with entire mean of the 'Age' column

**METHOD I**

*)split the table with reference to the Title column which has 5 values that are mr,mrs,miss,master,rare resulting into 5 tables

*)Then filled the NAN values column with mean() of the respective tables(mr,mrs,miss,master,rare)

*)After filling, 5 tables(mr,mrs,miss,master,rare) are joined

*)Removed the columns which had duplicates and less correlation with dependent variable

*)created the new columns to get the maximum survival rate

*)Assigned the LabelEncoder and OneHotEncoder to the categorical varibles

*)Fit few machine learning algorithms(Random Forest,Decision Tree,Logistic Regression,KNN,Support Vector Machines,Naive Bayes,Stochastic Gradient Decent) on the data

***comparing the scores of different models obtained using 2 methods in this notebook***

|  ***Model	               | Method I Score	   |    Method II Score*** |
|--------------------------|-------------------|-----------------------|
|Random Forest	            | **83.21**    	    |       **77.99**       |
|Decision Tree	            |   83.21	          |         77.99         |
|Support Vector Machines	  |   78.36	          |         77.24         |
|Logistic Regression	      |   78.36	          |         76.12         |
|Naive Bayes	              |   77.99	          |         74.63         |
|Stochastic Gradient Decent|	  69.40	          |         74.63         |
|KNN	                      |   54.48	          |         69.03         |




***Preprocessing steps we are going to explained on 'Titanic_Approach-2'***


*) Then filled the NAN values with mean() for the respective tables(mr,mrs,miss,master,rare)

*)After filling,the 5 tables(mr,mrs,miss,master,rare) were joined

*)Removed the columns which had duplicates and less correlation with dependent variable

*)converted the 'Age' column and the 'Fare' column into categorical

*)created the new columns like 'relatives','not-alone','Fare_per_person' trying to get the maximum survival rate.

*)Assigned the LabelEncoder and OneHotEncoder to the categorical varibles

*)Fit few machine learning algorithms(Random Forest,Decision Tree,Logistic Regression,KNN,Support Vector Machines,Naive Bayes,Stochastic Gradient Decent) on the data



### comparing the scores of different models obtained from Part I & Part II
| Model                       | Score-I | Score-II |
| --------------------------- | ------- | -------- |
| Random Forest               |  83.21  | **84.33**|
| Decision Tree               |  83.21  |   82.84  |
| Support Vector Machines     |  78.36  |   80.97  |
| Logistic Regression         |  78.36  |   80.22  |
| Naive Bayes                 |  77.99  |   78.36  |
| Stochastic Gradient Decent  |  73.51  |   75.37  |
| KNN                         |  54.48  |   67.91  |
