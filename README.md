# Davivienda_DS_project

## Project motivation

A brief story about my current role and the ongoing project:
Not so long ago I change a job in finance for the opportunity to work in one of the most promising new areas of my company, Marketing Intelligence. Its goal is to understand clients through data and experimental practices. As a beginner in analytics, this project is an opportunity to materialize some of my learnings and use the tools given by Udacity to bring up data solutions for a current business problem.

One of the components that is needed in order to forecast the effect of a campaign is the average email open rate. Since everything it’s as hard as it can be, there are many clients that doesn’t have this metric in our data bases. Therefore the object of this project is to build a linear regression model based on what’s taught in the course to try and forecast this metric for clients that doesn’t have it. The business questions needed to complete the project are:

  1. Which are the most relevant client’s traits and how can they be group to get a better understanding of them? 
  2. How does the open rate of emails behave in young clients, 18 to 30 years old?
  3. Can a multivariate regression model based on the variables identified before an acceptable model to predict open rate of clients missing this information? 

The project outline based on the CRISP methodology is as follows:
  1. Business understanding: The understanding of the importance of the open rate is directly related with the formula used to forecast a campaign success. This is why it’s really relevant for the business. The formula used is: Campaign success = Clients base x open rate x expected campaign effect.
  2. Data understanding: For this case I used different groups of features that could describe our client more holistically and extracted the data based on this approach. The groups and variables I used are the following:
 
- Demographic: Gender, age and income.
- Psychographic: transactional forecasted affinities.
- Business related: savings and investments products.
- Behavioral: Digital affinity, saving behavior, spending behavior and credit behavior, credit score.
- Geographical: City.
	
   3. Data preparation: As the data gathered came from different locations it needed a lot of cleaning, which was achived with codes learned in the course. You can find the specifics in the data_cleaning.py file.

   5. The model The model used was a multiple regression learned at the course using the same packages. You can find the code at the model.py file.
   6. Evaluation In order to evaluate the model I used the r squared metric that allow us to identify how much of the independence variable is explained by the dependent ones.
Sadly in this case after all this work the r squared method was extremely low, letting us identify that the variables chosen doesn’t necessarily relate with the open rate. Therefore we need to try a search for new variables that could let us build a more accurate model or use a different kind of approach with a different model.


## Libraries used

- numpy
- pandas
- matplotlib
- sklearn
- seaborn
- Udacity Alltogether code


## Files in repository

I. readme file -> Describres the project and its framework.

II. Juypter notebook -> The programing and execution of the project outline.

III. Df_ds -> data used for the project.

IV. Alltogether -> library shown in Audacity course, .py file.

## Results

This was an excelent project to get inmerse in the workflow of a Data Science, and the results to the business questions briefly explained are the following:

1. Which are the most relevant client’s traits and how can they be group to get a better understanding of them?
Demographic: Gender, age and income. 
Psychographic: transactional forecasted affinities. 
Business related: savings and investments products. 
Behavioral: Digital affinity, saving behavior, spending behavior and credit behavior, credit score. 
Geographical: City.

2.  How does the open rate of emails behave in young clients, 18 to 30 years old?
The open rate in young clients have a left skewed distribution, its mean is 9% but it has a considerable standard devation of 18%.

3. Is a multivariate regression model based on the variables identified an acceptable model to predict open rate?
The r^2 is too low to use this type of model in production.
Therefore it's recomended to look for other models in order to get a better fit, random forest is a suggestion that should be evaluated.

Readers can check a blog post in the following link:
https://medium.com/@emilio.m16/attempt-to-forecast-email-openings-7a35d4d34d7a

## Acknowledgments

This project is based on Udacity nano degree for Data Science, and most of its content might be reviewed there.
Also their reviewers made a great contributino to this project by correcting its content.

