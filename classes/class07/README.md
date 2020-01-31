# 432 Spring 2020 Class 07: 2020-02-04

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 07 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class07/432_2020_slides07.pdf) | [Class 07 .Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class07/432_2020_slides07.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Announcements

1. I revised the Week 3 Slides ([PDF](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class06/432_2020_week03.pdf), [RMarkdown](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class06/432_2020_week03.Rmd)) to fix a typo in the denominator of Specificity in slide 39.
2. I added the [ModernDive example with interaction and parallel slope plots](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class06/modern_dive_example.md) that were missing in Class 6.
3. More to come.

## On Your Project, Sample Size and Logistic Regression Models

To fit a logistic regression model, we need a fairly considerable sample size. [This tweet](https://twitter.com/f2harrell/status/936230071219707913?lang=en) links to some details.

One set of "rules" that I like to use is as follows:

1. Select the number of predictors you want to study in your logistic regression (includes everything you plan to consider, regardless of whether it makes it into your final model) and call that P.
2. Denote the sample size as follows - if you have an outcome where you have N1 people with "1" and N0 people with "0" then let N = min(N0, N1).
3. To fit a logistic regression model with P+1 coefficients (adding one for the intercept) you need that N to be at least 96 + 8P, realistically, in order to get a margin of error of +/- 0.1 in estimating probabilities.

- So if you have a rare event that occurs less than 96 times, your logistic regression model will be so weak that even an intercept won't be reliably estimated.
- For the project, I'd operationalize this to say that if both "1" and "0" occur 200 times, they should be fine for our purposes for any sample size up to 1000.
- For people with fewer than 256 observations overall, their logistic regression models will be very weak, since even with just 4 predictors, you'd really want 128 "1" and 128 "0" results. 
- Since I've set the minimum sample size for Project 1 at 100, there will be some people in that setting. The rule I'll apply in future versions of the course will require at least 400 observations on all data, and at least 200 "1" and 200 "0" in their binary outcome. If you can meet that standard with the data set you plan to use, great. If not, prepare for your logistic regression model to be a little disappointing.

## Next Few Deliverables (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
---------: | -----------------------------------------------------------------------
Today | [Homework 2](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw02) due at 5 PM.
Tomorrow | You should have your data for [Project 1](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) in hand.
Thursday | Read *The Art of Statistics* Chapter 7 (Estimates and Intervals)
Friday | There will be a Minute Paper after Class 8 due at 2 PM. **Link to come.**
2020-02-11 | [Homework 3](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw03) due at 5 PM. 
2020-02-13 | Read *The Art of Statistics* Chapter 8 (Probability)
2020-02-14 | [Project 1 Proposal](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) due at 2 PM.


