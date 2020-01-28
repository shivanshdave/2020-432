# 432 Spring 2020 Class 06: 2020-01-30

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Week 3 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class06/432_2020_week03.pdf) | [Week 3 .Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class06/432_2020_week03.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Announcements

1. A reminder that I've added some new packages, including `caret` and `tidymodels` to the [software packages list](https://github.com/THOMASELOVE/2020-432/blob/master/software.md). Please update your packages in RStudio, and add these new ones.
2. The [Minute Paper after Class 06](http://bit.ly/432-2020-minute-06) is due at 2 PM tomorrow.
3. More to come.

## What does it mean to have your data for Project 1 in hand?

I think you will be much happier if you have data for Project 1 by 2020-02-05 than if you don't, because I think you need to spend meaningful time with the data in R before you turn in your proposal on 2020-02-14.

By *data in hand*, I mean:

1. Your data meets all the standards posted in the [What Makes an Acceptable Data Set](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1#what-makes-an-acceptable-data-set) section of the Project 1 instructions.
    a. Availability to All
    b. Size (n = 100 to 1000)
    c. Outcomes (one quantitative and one binary) for your planned models
    d. Inputs (somewhere between 4 and 4 + (n-100)/100 inputs are required) for your planned models
2. The original source of the data (files, hyperlinks, etc.) and the raw data you used to create the analytic data are in your possession.
    a. The raw data should be in one or more .csv files.
    b. You should have a recipe for how you went from the raw data to the analytic tibble.
3. Your analytic data is in the form of a tidied rectangle (rows indicate subjects/observations and columns are variables) and already exists as a tibble in R, and is stored as a .csv (and perhaps also as an .Rds) file, using `write_csv` (and perhaps `saveRDS`, too.)
4. Your analytic tibble contains *only* the observations and variables you intend to use in your work, and a subject identifier.
5. In the analytic tibble, every characteristic/measure you gather is obtained at the level of the subject (no hierarchical data.)
6. In the tibble, all variable names are meaningful to you and use an appropriate naming style consistently - please run `clean_names()`.
7. You can clearly specify the units for all quantities and the potential levels for all categorical variables that are in your tibble.
8. Missing observations are consistently indicated with NA in R and with blanks in your CSV file.

If you are unsure whether your raw data or analytic tibble meets one or more of these standards, then please email us at 431-help as soon as possible with specific questions, and we'll try to provide confirmation.

## What is Wrong with This Picture?

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class06/Futier_2020_FLASH_JAMA_visual_abstract.png)

## Next Few Deliverables (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
---------: | -----------------------------------------------------------------------
**Tomorrow** | [Minute Paper after Class 06](http://bit.ly/432-2020-minute-06) is due at 2 PM.
2020-02-04 | [Homework 2](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw02) due at 5 PM.
2020-02-05 | You should have your data for [Project 1](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) in hand.
2020-02-06 | Read *The Art of Statistics* Chapter 7 (Estimates and Intervals)
2020-02-11 | [Homework 3](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw03) due at 5 PM. (Note that HW 3 was revised 2020-01-27)
2020-02-13 | Read *The Art of Statistics* Chapter 8 (Probability)
2020-02-14 | [Project 1 Proposal](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) due at 2 PM.

## One Last Thing

To come.
