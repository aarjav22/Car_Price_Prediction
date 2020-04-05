# Car Price Prediction

## Regression model to predict the Price of the Car
&nbsp; &nbsp; &nbsp; &nbsp;

## Table of Contents

1.	Introduction
2.	Python libraries
3.	The problem statement
4.	Linear Regression
5.	Independent and dependent variable
6.	Multiple Linear Regression (MLR)
7.	About the dataset
8.	Exploratory data analysis
9.	Interpretation and conclusion


&nbsp; &nbsp; &nbsp; &nbsp;

## 1.	Introduction

In this project, I build Regression model to study the relationship between Price of a car and different continous and discrete variables. I implemented this regression model in Python programming language using Scikit-learn,numpy,seaborn,matplotlib. 

&nbsp; &nbsp; &nbsp; &nbsp;

## 2.	Python libraries

 •	Numpy
 
 •	Pandas

 •	Matplotlib
 
 •	Seaborn
 
 •	Scikit-Learn

&nbsp; &nbsp; &nbsp; &nbsp;

## 3.	The problem statement

The main aim of this model is to predicting the Price of a car using some continous and discrete variable data. Finding relationship or dependency of Price on attrubutes like Engine-Size , Horsepower and many continous and discrete variable data. 
The accuracy of the model is defined by RMS value and R2 Score.To improve the accuracy of the model I tried to Polynomial fit the data into the model.

&nbsp; &nbsp; &nbsp; &nbsp;

## 4.	Linear Regression

Linear Regression is a statistical technique which is used to find the linear relationship between dependent and one or more independent variables. This technique is applicable for Supervised Learning Regression problems where we try to predict a continuous variable.
Linear Regression can be further classified into two types – Simple and Multiple Linear Regression. In this project, I employ Multiple Polynomial Regression technique where I have Multiple independent and one dependent variable.

&nbsp; &nbsp; &nbsp; &nbsp;

## 5.	Independent and Dependent Variables

### Independent variable

Independent or Input variable (X) = Feature variable = Predictor variable 

The following are the independent variable:-

  1. symboling:                -3, -2, -1, 0, 1, 2, 3.
  2. normalized-losses:        continuous from 65 to 256.
  3. make:                     alfa-romero, audi, bmw, chevrolet, dodge, honda,
                               isuzu, jaguar, mazda, mercedes-benz, mercury,
                               mitsubishi, nissan, peugot, plymouth, porsche,
                               renault, saab, subaru, toyota, volkswagen, volvo
  4. fuel-type:                diesel, gas.
  5. aspiration:               std, turbo.
  6. num-of-doors:             four, two.
  7. body-style:               hardtop, wagon, sedan, hatchback, convertible.
  8. drive-wheels:             4wd, fwd, rwd.
  9. engine-location:          front, rear.
 10. wheel-base:               continuous from 86.6 120.9.
 11. length:                   continuous from 141.1 to 208.1.
 12. width:                    continuous from 60.3 to 72.3.
 13. height:                   continuous from 47.8 to 59.8.
 14. curb-weight:              continuous from 1488 to 4066.
 15. engine-type:              dohc, dohcv, l, ohc, ohcf, ohcv, rotor.
 16. num-of-cylinders:         eight, five, four, six, three, twelve, two.
 17. engine-size:              continuous from 61 to 326.
 18. fuel-system:              1bbl, 2bbl, 4bbl, idi, mfi, mpfi, spdi, spfi.
 19. bore:                     continuous from 2.54 to 3.94.
 20. stroke:                   continuous from 2.07 to 4.17.
 21. compression-ratio:        continuous from 7 to 23.
 22. horsepower:               continuous from 48 to 288.
 23. peak-rpm:                 continuous from 4150 to 6600.
 24. city-mpg:                 continuous from 13 to 49.
 25. highway-mpg:              continuous from 16 to 54.

### Dependent variable

Dependent or Output variable (y) = Target variable = Response variable

The following is the dependent variable:-
 
  1. price:                    continuous from 5118 to 45400.


&nbsp; &nbsp; &nbsp; &nbsp;

## 6.	Multiple Linear Regression (MLR)

Multiple Linear Regression also known simply as multiple regression is a statistical technique that uses several explanatory variables to predict the outcome or the response variable.
The goal of multiple linear regression is to model the linear relationship between the explanatory variable (independent variable) and response variable.

The formula for Multiple Regression is:
	     		
		y = a0 + a1x1 + a2x2 + ...............

where
  y = dependent variable
  xi= independent variable
  a0= y-intercept
  ai= slope coefficients for each independent variable

&nbsp; &nbsp; &nbsp; &nbsp;

## 7.	About the dataset

    1. Title: 1985 Auto Imports Database

    2. Source Information:
        -- Creator/Donor: Jeffrey C. Schlimmer (Jeffrey.Schlimmer@a.gp.cs.cmu.edu)
        -- Date: 19 May 1987
   	-- Sources:
     		1) 1985 Model Import Car and Truck Specifications, 1985 Ward's
        	Automotive Yearbook.
     		2) Personal Auto Manuals, Insurance Services Office, 160 Water
        	Street, New York, NY 10038 
     		3) Insurance Collision Report, Insurance Institute for Highway
        	Safety, Watergate 600, Washington, DC 20037
    3. Relevant Information:
   	-- Description
      		This data set consists of three types of entities: (a) the
      		specification of an auto in terms of various characteristics, (b)
      		its assigned insurance risk rating, (c) its normalized losses in use
      		as compared to other cars.  The second rating corresponds to the
      		degree to which the auto is more risky than its price indicates.
      		Cars are initially assigned a risk factor symbol associated with its
      		price.   Then, if it is more risky (or less), this symbol is
      		adjusted by moving it up (or down) the scale.  Actuarians call this
      		process "symboling".  A value of +3 indicates that the auto is
      		risky, -3 that it is probably pretty safe.

	        The third factor is the relative average loss payment per insured
      	        vehicle year.  This value is normalized for all autos within a
      		particular size classification (two-door small, station wagons,
      		sports/speciality, etc...), and represents the average loss per car
      		per year.

&nbsp; &nbsp; &nbsp; &nbsp;

## 8.	Exploratory data analysis

To summarize the main characteristics of data I analysed it using Data Visualization by ploting graphs like regression plot ,box plot ,histogrames, and distribution plot between the dependent and various independent variables.
It help me in finding the good attributes and bad attributes for training my model as graph clearly shows us the reationship between the variables. 	 

&nbsp; &nbsp; &nbsp; &nbsp;

## 9.	Interpretation and Conclusion

Simple Linear Regression:
	
     RMSE value: 15446938.691334337
     
     R2 value : 0.6887892619732783

Multiple Linear Regression:
	
     RMSE value: 19637652.97310373
     
     R2 value : 0.7708377040905359

Polynomial Regression: 

     RMSE value: 5357185.720506018
     
     R2 value : 0.892068340844766

We can conclude by looking the Mean Squared value and R2 value that polynomial regression fit more perfect for the given car data as compaired to simple or multiple linear regression.
as Polynomial Regression gives almost 90 per accuracy and there is a huge difference in RMS value of multiple regression and polynomial regression.
&nbsp; &nbsp; &nbsp; &nbsp;