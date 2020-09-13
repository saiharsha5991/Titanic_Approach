# Titanic_Approach
In this kernal Iam going to explain the famous Titanic Challenge. The challenge is to use machine learning to create a model that predicts which passengers survived the Titanic shipwreck I have tried out 2 approches, one explained in this notebook, the other approach exaplained in another notebooks with title 'Titanic_Approach-2_Part-II' &amp; 'Titanic_Approach-2_Part-II'

***Preprocessing steps we are going to explained***
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
