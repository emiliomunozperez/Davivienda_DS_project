# Davivienda_DS_project

A brief story about my current role and the ongoing project:

Not so long ago I change a job in finance for the opportunity to work in one of the most promising new areas of my company, Marketing Intelligence. Its goal is to understand clients through data and experimental practices. As a beginner in analytics, this project is an opportunity to materialize some of my learnings and use the tools given by Udacity to bring up data solutions for a current business problem.

One of the components that is needed in order to forecast the effect of a campaign is the average email open rate. Since everything it’s as hard as it can be, there are many clients that doesn’t have this metric in our data bases. Therefore the object of this project is to build a linear regression model based on what’s taught in the course to try and forecast this metric for clients that doesn’t have it. The project outline based on the CRISP methodology is as follows:

1.	Business understanding:
The understanding of the importance of the open rate is directly related with the formula used to forecast a campaign success. This is why it’s really relevant for the business. 
The formula used is: 
Campaign success = Clients base x open rate x expected campaign effect. 

2.	Data understanding:
For this case I used different groups of features that could describe our client more holistically and extracted the data based on this approach. The groups and variables I used are the following:

   Demographic: Gender, age and income.

   Psychographic: transactional forecasted affinities.

   Business related: savings and investments products.

   Behavioral: Digital affinity, saving behavior, spending behavior and credit behavior, credit score.

   Geographical: City.

3.	Data preparation: 
As the data gathered came from different locations it needed a lot of cleaning, which was achived with codes learned in the course. You can find the specifics in the data_cleaning.py file.

4.	The model
The model used was a multiple regression learned at the course using the same packages. You can find the code at the model.py file.

5.	Evaluation
In order to evaluate the model I used the r squared metric that allow us to identify how much of the independence variable is explained by the dependent ones.

Sadly in this case after all this work the r squared method was extremely low, letting us identify that the variables chosen doesn’t necessarily relate with the open rate. Therefore we need to try a search for new variables that could let us build a more accurate model or use a different kind of approach with a different model.
	 
