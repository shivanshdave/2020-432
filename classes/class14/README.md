# 432 Spring 2020 Class 14: 2020-03-05

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 14 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class14/432_2020_slides14.pdf) | [Class 14 Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class14/432_2020_slides14.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Key Topic

Dealing with Aggregated Data in Logistic Regression, Probit Regression 
- These materials are discussed in the [Course Notes](https://thomaselove.github.io/2020-432-book/) in Chapter 18

## Today's Announcements

1. There is a [Minute Paper after Class 14](http://bit.ly/432-2020-minute-14), due at 2 PM on Friday 2020-03-06.
2. The [Course Notes](https://thomaselove.github.io/2020-432-book/) have been updated to include Chapters 16, 18, and 21-24, along with placeholders for 17, 19 and 20.
3. For Project 2, I specified [some data sources I'd be pleased to see used more](https://github.com/THOMASELOVE/2020-432/blob/master/projects/project2/README.md#suggested-data-sources). 
4. Enjoy Spring Break! Our next class will be Tuesday 2020-03-17.

## Some Project 1 Tips

1. My note on back-transformation in nomograms for linear and logistic regression is available [in R Markdown](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class14/class14_nomogram_note.Rmd) or [as a PDF](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class14/class14_nomogram_note.pdf).

2. Some of you may have a logistic regression model that won't run, or that produces explosive results, with extremely large or small coefficients or standard errors. If that's the case, check to see that your binary outcome occurs at least a few times (and doesn't occur at least a few times) at every level of each of your categorical predictors. If, for example, you have a factor with levels A, B, C and D, and your outcome is always 1 (and never 0) for subjects in level D, you have a problem. The simplest solution is to recast the logistic regression model as a model for the sample including only subjects from levels A, B and C.

3. If you have a quantitative predictor or outcome in your project 1 data that could be represented by either a proportion (number between 0 and 1) or a percentage (number between 0 and 100), I suggest you use a percentage, multiplying the proportion by 100 if necessary.

4. If your predictors are on wildly different scales, for instance, most of your predictors are between 0 and 100 or are categorical, but one of your predictors (say, `cost`) is on a much wider scale (say from 1,000 to 10,000,000) then I strongly suggest either representing the costs with a base-10 logarithm or dividing by, say, 1000 to represent the costs in thousands of dollars. This will reduce the chances of you having a very very small or very very large coefficient that you need to explain. 

5. For Project 1, I suggest that using simple imputation or complete cases is fine. We'd like to see multiple imputation in Project 2, but it's not something Dr. Love will be looking for in Project 1, *except* that it's an excellent thing to mention in the Discussion session as a likely next step for the work.

6. If you are comparing models A and B in Project 1 and they are very comparable in terms of validation statistics (perhaps the R-square is within 1 percentage point of each other, and the RMSE and MAE disagree) then if both models' residual plots look OK, I would probably pick the main effects model, personally. (If model A's residuals look fine, but model B's don't, then you'd clearly choose model A.) You can choose whatever model you feel is more justified base on the results you've built.

7. The Box-Cox procedure isn't going to provide useful information on transformation of a quantitative outcome if your outcome is (a) not all positive, (b) discrete with a ceiling and a floor and limited potential values or (c) if you have one or more predictors that essentially define the outcome value (for instance, everyone who smokes has a higher outcome value, or close to that, than everyone who doesn't smoke). Do not use the Box-Cox procedure to try to justify a transformation other than these five: inverse, log, square root, raw (untransformed) and square.  In fact, don't use any transformation other than those five.

## Reminders/Notes (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
----: | ---------------------------------------------------------------
03-06 | [Minute Paper after Class 14](http://bit.ly/432-2020-minute-14), due at 2 PM.
03-09 | [Project 1 Posters/Portfolios](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) are due at 2 PM.
Break | No class and no TA office hours from 03-09 through 03-13. `431-help` will be open.
03-17 | [Project 2 Instructions](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project2) should be available by 1 PM.
03-20 | There will be a Minute Paper after Class 16, due at 2 PM.
03-23 | [Homework 4](https://github.com/THOMASELOVE/2020-432/tree/master/homework) due at 5 PM
03-26 | [Quiz 2](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) made available at 5 PM
03-30 | [Quiz 2](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) due at 2 PM
04-01 | [Project 2 Proposal](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project2) due at 2 PM


## One Last Thing

The map below [appeared in an article on CNBC.com](https://www.cnbc.com/2020/02/26/people-skipping-medically-necessary-drugs-because-they-cost-too-much.html) on 2020-02-26.

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class13/figures/cnbc_map_original.PNG)

[Alyssa Keiko](https://twitter.com/alyssakeiko/status/1233092947987529728) tweeted it out, saying "I have a lot of questions about if anyone looked at this map before during or after its making"

Any thoughts as to what happened here?

.

.

.

.

.

[Sam Ventura on Twitter](https://twitter.com/stat_sam/status/1233191157053693953?s=11) has the answer, I think...

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class13/figures/sam_ventura_2020.PNG)

If you're concerned about Alabama, later in that thread, Sam reminds us that 

> Wyoming + 1 = Alabama, if you go 'round the corner.

By 2020-02-28, CNBC corrected the map, which now looks like this:

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class13/figures/cnbc_map_corrected.PNG)
