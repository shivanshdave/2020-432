# 432 Spring 2020 Class 13: 2020-03-03

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 13 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class13/432_2020_slides13.pdf) | [Class 13 Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class13/432_2020_slides13.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Key Topic

Details to come.

## Today's Announcements

### About the Class

1. Quiz 1 results should **appear by class time, I hope**.
2. I expect to post instructions for Homework 4 **by class time**. It is due at 5 PM on 2020-03-23.
3. Homework 3 grades were posted on 2020-02-27 to http://bit.ly/432-2020-grades. 
    - We built a [Google Doc containing several of the essays we really enjoyed in response to Question 6](https://docs.google.com/document/d/1krZRnMTniOKfU0EqlE-dnJjqP4n7hBgFB7JSPN-x8mQ/edit?usp=sharing).
4. *Homework Regrades*. A reminder...
    - If we've added your points up incorrectly on a Homework, send an email to Dr. Love at any time before 5 PM 2020-04-30.
    - To request a Homework regrade for any other reason, fill out the Form at http://bit.ly/432-2020-homework-regrade-requests  any time before 5 PM on 2020-04-30. Dr. Love will review all of those requests in a batch then. [See the Grading Errors section here](https://github.com/THOMASELOVE/2020-432/blob/master/homework/README.md#grading-errors) for a little more detail.
5. Minute Paper after Class 12 feedback is available at http://bit.ly/432-2020-minute12-feedback.
6. Project 2 instructions will appear on 2020-03-17 by 1 PM. The answer to all of the complicated questions I've heard so far about Project 2 is "I'm not sure. It depends on how Project 1 goes."

### Other Things

1. [Biostats4You](https://biostats4you.umn.edu/) from the University of Minnesota may be of interest to you. 
    > (The site) was developed to serve medical and public health researchers and professionals who wish to learn more about biostatistics. The site contains carefully selected and vetted training materials especially suited for a non-statistician audience.

## A few comments on non-linearity and the Spearman rho-squared plot

The main reason we use a Spearman rho-squared plot is as follows:

1. We know what variables we want to include in our model, but don't have a clear sense in advance of how we want to incorporate non-linear predictor terms (for instance, we don't have a prior clear understanding of which variables should interact with each other, or which variables will have a non-linear relationship with our outcome, after adjusting for all other variables.)
2. We want to avoid the possibility of using the data in such a way as to bias our eventual prediction model towards over-optimism about the significance of our coefficients, which essentially means that we cannot look directly at the X-Y relationship to see if it appears non-linear, because if we do this, we will include things we probably shouldn't, overstate the significance of the coefficients that wind up in the model, understate the standard errors, and overstate the summary statistics (R-square, C statistic, etc.) associated with the final fitted model, although we can mitigate this risk (a little bit) by splitting the data into training and test samples and performing cross-validation.  

What we're trying very hard to avoid is fitting many, many models to the data, identifying which one fits best in the data, and then believing that the summary statistics and statistical tests developed using that same data are correct, because they won't be. Every time we fit a model we spend some of the information (as measured by degrees of freedom) that we have available in the data set. Even if we have enormous data sets, we try hard not to overstate the quality of fit of a model built not for scientific reasons but instead because of p values or AIC statistics, or whatever summary you choose.

So the idea is that looking at the Spearman correlation - the rank correlation - of X with Y is somewhat safe in that it provides some evidence that helps us think about non-linearity, but it doesn't bias us so badly. We build a plot that shows for each variable X, essentially, the adjusted R-squared computed on the ranks of X and Y (and actually also on the rank of X-squared. This absolutely does not identify which variables will most benefit from non-linear terms. Instead, it identifies (to some extent) which variables have higher and lower levels of potential predictive power for our outcome, in general. 

We then use the plot to help decide where to spend the degrees of freedom of non-linearity that we are willing to spend, but (a) if we have scientific reasons to fit non-linear terms, like splines or interactions, then those scientific reasons should be used instead of the plot and (b) the plot is by no means a guarantee that the non-linear terms we identify will wind up adding significant or substantial predictive value to the model.

## Reminders/Notes (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
----: | ---------------------------------------------------------------
03-06 | There will be a Minute Paper after Class 14, due at 2 PM.
03-09 | [Project 1 Posters/Portfolios](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) are due at 2 PM.
Break | No class and no TA office hours from 03-09 through 03-13. `431-help` will be open.
03-17 | [Project 2 Instructions](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project2) should be available by 1 PM.
03-20 | There will be a Minute Paper after Class 16, due at 2 PM.
03-23 | [Homework 4](https://github.com/THOMASELOVE/2020-432/tree/master/homework) due at 5 PM
03-26 | [Quiz 2](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) made available at 5 PM
03-30 | [Quiz 2](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) due at 2 PM
04-01 | [Project 2 Proposal](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project2) due at 2 PM

## One Last Thing
