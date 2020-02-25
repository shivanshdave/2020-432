# 432 Spring 2020 Class 12: 2020-02-25

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 12 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class12/432_2020_slides12.pdf) | [Class 12 Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class12/432_2020_slides12.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Key Topic

Today, we'll be talking about multiple imputation and cross-validation approaches when fitting a linear regression model with `lm` and when fitting a logistic regression model with `glm`, in each case without using `aregImpute` or the `Hmisc` package.

### A Few References on Multiple Imputation

- Thomas Leeper's [Tutorial](https://thomasleeper.com/Rcourse/Tutorials/mi.html) which covers methods using `mice`, but also the `Amelia` and `mi` packages.
- Sterne JAC, White IR, Carlin JB, Spratt M, Royston P, Kenward MG, Wood AM, and Carpenter JR [Multiple imputation for missing data in epidemiological and clinical research: potential and pitfalls](https://www.bmj.com/content/338/bmj.b2393) BMJ 2009;338:b2393
- Stef van Buuren and Karin Groothuis-Oudshoorn [mice: Multivariate Imputation by Chained Equations in R](https://www.jstatsoft.org/article/view/v045i03) *J Statistical Software* 2011, 45:3.
- UCLA Statistical Consulting R FAQ: [How do I perform multiple imputation using predictive mean matching in R?]( https://stats.idre.ucla.edu/r/faq/how-do-i-perform-multiple-imputation-using-predictive-mean-matching-in-r/)

## Today's Announcements

1. Please remember that we don't have class this Thursday 2020-02-27. 
2. There will be a **Minute Paper after Class 12**, which will be due at 2 PM Wednesday.
3. The [Answer Sketch for Homework 3](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw03) is available. We anticipate **grades** appearing at http://bit.ly/432-2020-grades by 5 PM on 2020-02-25.
4. **Project 1 Proposal Status**
    - Let's take a look at [where we are](https://github.com/THOMASELOVE/2020-432/blob/master/projects/project1/approved_proposals.md).
5. Since we last met, there have been several updates to the [Project 1 Instructions](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1).
    - This includes [a set of portfolio templates](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1/templates) which can be very helpful to you in terms of getting the formatting to work well. Switching between these three templates is simply a matter of swapping out the YAML code at the start of the R Markdown document.
    - The newest arrival is a [posterdown template](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1/templates) which we'll talk about today, and which I'm expecting you to use in preparing your poster.
6. Quiz 1 covers materials through the first 11 classes, and Chapters 1-5 and 7-8 of Spiegelhalter's *Art of Statistics*. It will have **either 14 or 15** questions. It **will be available** at 5 PM Wednesday 2020-02-26.
7. The next meeting of [the Cleveland R Users Group](https://www.meetup.com/Cleveland-UseR-Group) is Wednesday evening (2020-02-26). I've been to a few of the meetings in the past (though I won't be at this one) and found them useful/interesting.

## Next Few Deliverables (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
----: | ---------------------------------------------------------------
02-26 | If necessary, the third version of your [Project 1 Proposal](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1#new-some-additional-thoughts-after-reviewing-the-proposal-drafts) will be due at 9 AM.
02-26 | Minute Paper after Class 12 will be due at 2 PM.
02-26 | [Quiz 1](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) will be made available at 5 PM.
03-02 | [Quiz 1](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) is due at 9 AM.
03-09 | [Project 1 Posters/Portfolios](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) are due at 2 PM.

## One Last Thing

**To come**.
