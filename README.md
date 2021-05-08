# Logistic Regression

## Classification Model to predict weather a passenger survived or not.

&nbsp; &nbsp; &nbsp; &nbsp;

## Table of Contents

1.	Introduction
2.	Python libraries
3.	The problem statement
4.	Logistic Regression
5.	Independent and dependent variable
6.      Logistic Regression Algorithm
7.	Decision boundary
8.	Exploratory data analysis
9.	Interpretation and Conclusion

&nbsp; &nbsp; &nbsp; &nbsp;

## 1.	Introduction

In this project, I build Classification model to study the relationship between passenger survival and different continous and discrete variables. I implemented this classification model in Python programming language using Scikit-learn,numpy,seaborn,matplotlib. 

&nbsp; &nbsp; &nbsp; &nbsp;

## 2.	Python libraries

 •	Numpy
 
 •	Pandas

 •	Matplotlib
 
 •	Seaborn
 
 •	Scikit-Learn

&nbsp; &nbsp; &nbsp; &nbsp;

## 3.	The problem statement

The main aim of this model is to predicting weather a passenger survived or not on the basis of different attributes. Finding relationship or dependency of Output on attrubutes like Age,Sex and other variables. 
The accuracy of the model is defined using accuracy_score, confusion_matrix, ROc Graph.

&nbsp; &nbsp; &nbsp; &nbsp;

## 4.	Logistic Regression

Logistic Regression is one of the basic and popular algorithm to solve a classification problem. It is named as ‘Logistic Regression’, because it’s underlying technique is quite the same as Linear Regression. The term “Logistic” is taken from the Logit function that is used in this method of classification.
We identify problem as classification problem when independent variables are continuous in nature and dependent variable is in categorical form i.e. in classes like positive class and negative class. The real life example of classification example would be, to categorize the mail as spam or not spam, to categorize the tumor as malignant or benign and to categorize the transaction as fraudulent or genuine. All these problem’s answers are in categorical form i.e. Yes or No. and that is why they are two class classification problems.

&nbsp; &nbsp; &nbsp; &nbsp;

## 5.   Independent and Dependent Variables

### Independent variable

Independent or Input variable (X) = Feature variable = Predictor variable 

The following are the independent variable:-

  1. PassengerId
  2. Pclass
  3. Name
  4. Sex
  5. Age
  6. SibSp
  7. Parch
  8. Ticket
  9. Fare
  10. Cabin
  11. Embarked

### Dependent variable

Dependent or Output variable (y) = Target variable = Response variable

The following is the dependent variable:-
 
  1. Survived

&nbsp; &nbsp; &nbsp; &nbsp;

## 6.	Logistic Regression Algorithm

	Logistic Regression uses Sigmoid function.
	An explanation of logistic regression can begin with an explanation of the standard logistic function. The logistic function is a Sigmoid function, which takes any real value between zero and one. It is defined as
				
			f(t) = e^t / e^t + 1

			f(t) = 1 / 1 + e^-t
	Let’s consider t as linear function in a univariate regression model.
			
			t = a0 + a1*x

	So the Logistic Equation will become

			p(x) = 1 / 1 + e^-(a0+a1*x)

&nbsp; &nbsp; &nbsp; &nbsp;

## 7.	Decision boundary


The sigmoid function returns a probability value between 0 and 1. This probability value is then mapped to a discrete class which is either “0” or “1”. In order to map this probability value to a discrete class (pass/fail, yes/no, true/false), we select a threshold value. This threshold value is called **Decision boundary**. Above this threshold value, we will map the probability values into class 1 and below which we will map values into class 0.

Mathematically, it can be expressed as follows:-

	p ≥ 0.5 => class = 1
		
	p < 0.5 => class = 0 
	
Generally, the decision boundary is set to 0.5. So, if the probability value is 0.8 (> 0.5), we will map this observation to class 1.  Similarly, if the probability value is 0.2 (< 0.5), we will map this observation to class 0.

&nbsp; &nbsp; &nbsp; &nbsp;

## 8.	Exploratory data analysis

To summarize the main characteristics of data I analysed it using Data Visualization by ploting graphs like histogrames, and distribution plot between the dependent and various independent variables.
It help me in finding the good attributes and bad attributes for training my model as graph clearly shows us the reationship between the variables. 	 

&nbsp; &nbsp; &nbsp; &nbsp;

## 9.	Interpretation and Conclusion

	Accuracy Score : 0.7865168539325843
	
	Classification Report:
		precision : 0.80
		recall : 0.80
		f1-score : 0.80
		support : 268

According to the classification model the Survival of a pessenger depends on their passenger class, age, sex, single or with family.