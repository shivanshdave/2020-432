# 432 Spring 2020 Class 12: 2020-02-25

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 12 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class12/432_2020_slides12.pdf) | [Class 12 Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class12/432_2020_slides12.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Key Topic

Today, we'll be talking about multiple imputation and cross-validation approaches when fitting a linear regression model with `lm` and when fitting a logistic regression model with `glm`, in each case without using `aregImpute` or the `Hmisc` package.

## Today's Announcements

1. Please remember that we don't have class this Thursday 2020-02-27. 
2. There will be a **Minute Paper after Class 12**, which will be due at 2 PM Wednesday.
3. The [Answer Sketch for Homework 3](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw03) is available. We anticipate **grades** appearing at http://bit.ly/432-2020-grades by 5 PM on 2020-02-25.
4. Since we last met, there have been several updates to the [Project 1 Instructions](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1).
    - This includes [a set of portfolio templates](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1/templates) which can be very helpful to you in terms of getting the formatting to work well. Switching between these three templates is simply a matter of swapping out the YAML code at the start of the R Markdown document.
    - **Additional updates** will appear by class time.
    - If Dr. Love has accepted your [Project 1 Proposal Revision](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1#new-some-additional-thoughts-after-reviewing-the-proposal-drafts) and given you a grade of 10 on Canvas, you'll be on the list below, and you should move on to building your actual Portfolio for the project.
    - If your grade on the Proposal is still below 10 after revision, then your next (and, we fervently hope, final) revision is due Wednesday 2020-02-26 at 9 AM to Canvas, in the same place where you've posted prior revisions.
5. Quiz 1 covers materials through the first 11 classes, and Chapters 1-5 and 7-8 of Spiegelhalter's *Art of Statistics*. It will have **either 14 or 15** questions. It **will be available** at 5 PM Wednesday 2020-02-26.
6. The next meeting of [the Cleveland R Users Group](https://www.meetup.com/Cleveland-UseR-Group) is tomorrow evening. I've been to a few of the meetings in the past (though I won't be at this one) and found them useful/interesting.

## Approved Project Proposals (of the 38 in total)

Code | Investigator(s) | Title
---: | :-------------: | -------------------------------------------------------------------------------------------
`01-P` | Hussam Alqahtani and Kimberly Noriega | Unnamed project using NHANES to study sleep, BMI and gum disease
`03-P` | Fatima Asad and Basma Dahash | Unnamed project using Chinese PCI data from DataDryad
`11-P` | Emily Hannon and Jasmine Olvany | Exploring the Connection between Human Population and Sea Otter Health
`12-S` | Logan Harper | Unnamed project on diabetes using the National Health Interview Survey
`18-S` | Noah Lorincz-Comi | Predicting Absenteeism at Work
`20-S` | Stephanie Merlino Barr | Unnamed project using County Health Rankings to study infant mortality
`21-S` | Anna Miller | Predicting Blood Pressure Medication Usage and Doctor Checkups from 500 Cities Data
`30-S` | Alena Sorensen | Unnamed project using BRFSS data to study poor mental health days or satisfaction with life


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