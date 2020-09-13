# Titanic_Approach
In this kernal Iam going to explain the famous Titanic Challenge. The challenge is to use machine learning to create a model that predicts which passengers survived the Titanic shipwreck I have tried out 2 approches, one explained in this notebook, the other approach exaplained in another notebooks with title 'Titanic_Approach-2_Part-II' &amp; 'Titanic_Approach-2_Part-II'

***Preprocessing steps we are going to explained on 'Titanic_Approach-1'***

1)Import libraries

2)checked the data types

3)Extracted 'NAME' column from both train and test datasets. A column 'Title' is created and the extracted names are put in that column .For each title checked for 'SEX' column if a name is male or female

IN THIS I FILLED THE NULL VALUES OF 'AGE' COLUMN IN TWO DIFFERENT TYPES

**METHOD I**

4)split the table with reference to the Title column which has 5 values that are mr,mrs,miss,master,rare resulting into 5 tables

5)Then filled the NAN values column with mean() of the respective tables(mr,mrs,miss,master,rare)

6)After filling, 5 tables(mr,mrs,miss,master,rare) are joined

**METHOD II**

7)filled the null values of the 'Age' column with entire mean of the 'Age' column

8)Removed the columns which had duplicates and less correlation with dependent variable

9)created the new columns to get the maximum survival rate

10)Assigned the LabelEncoder and OneHotEncoder to the categorical varibles

11)Fit few machine learning algorithms(Random Forest,Decision Tree,Logistic Regression,KNN,Support Vector Machines,Naive Bayes,Stochastic Gradient Decent) on the data

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




***Preprocessing steps we are going to explained on 'Titanic_Approach-2 of part-1 and part-2'***

   ***PART-1***
   
1)Imported libraries

2)Checked the data types

3)Extracted 'NAME' column from both train and test datasets. A column 'Title' is created and the extracted names are put in that column. For each title checked for 'SEX' column if a name is male or female

4)Split the table with reference to the Title column which has 5 values that are mr,mrs,miss,master,rare resulting into 5 tables

5)Then filled the NAN values with mean() for the respective tables(mr,mrs,miss,master,rare)

6)After filling,the 5 tables(mr,mrs,miss,master,rare) were joined

7)Removed the columns which had duplicates and less correlation with dependent variable

8)Uploaded the file to csv for the continuation of part-2

9)Assigned the LabelEncoder and OneHotEncoder to the categorical varibles

10)Ran few machine learning algorithms(Random Forest,Decision Tree,Logistic Regression,KNN,Support Vector Machines,Naive Bayes,Stochastic Gradient Decent) on the data


 ***PART-2***
   
  This notebook is the continuation of part 1

1) Imported libraries

2) Loaded the part 1 data

3)In this I converted the 'Age' column and the 'Fare' column into categorical

4)created the new columns like 'relatives','not-alone','Fare_per_person' trying to get the maximum survival rate.

5)Assigned the LabelEncoder and OneHotEncoder to the categorical varibles

6)Fit few machine learning algorithms(Random Forest,Decision Tree,Logistic Regression,KNN,Support Vector Machines,Naive Bayes,Stochastic Gradient Decent) on the data



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
