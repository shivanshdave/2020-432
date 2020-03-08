# 432 Spring 2020 Class 15: 2020-03-17

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 15 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class15/432_2020_slides15.pdf) | [Class 15 Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class15/432_2020_slides15.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Announcements

1. Feedback on the Minute Paper after Class 14 will appear at http://bit.ly/432-2020-minute14-feedback.
2. Here's the logistic regression example ([in R Markdown](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class15/logistic_example_2020-03-06.Rmd) and [in PDF](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class15/logistic_example_2020-03-06.pdf)) that I built to demonstrate some things for Project 1, using the `lind` data from Quiz 1.
    - If you have trouble fitting a logistic regression model, check that your binary outcome is a numeric variable in R, with 1 and 0 its only possible values. That seems to lead to the fewest downstream problems, cleaner than having it be a factor or character variable, for example. To check the type of variable, I would use `str(datasetname)` to look at each of the variable types, and I would use `datasetname %>% tabyl(outcomename)` to check to see that the outcome's two values are in fact 0 and 1.
3. At some point in your life, you won't have 431-help any more, and you'll need to figure out how to debug on your own - consider googling any error messages you don't understand, and see if that might at least help you identify where your problem might be. If you are asking us a question at `431-help` about an R issue, I implore you to please send:
    - your complete R Markdown file
    - AND a clear indication of the problem you are having, such as a screenshot of the error and a clear indication of where in the code you are having a problem
    - AND either your original raw .csv file that you load at the top of your R Markdown file or a tidied Rds file of your data after cleaning. Don't send a tidied csv since that loses any work you've done to create factors, etc. For most problems where the answer isn't obvious, we need to be able to exactly duplicate your problem in order to fix it.

## In The News

1. [COVID-19 Epidemiology with R](https://rviews.rstudio.com/2020/03/05/covid-19-epidemiology-with-r/) by Tim Churches 2020-03-05. 
    - The [`coronavirus` package] provides a daily summary of the Coronavirus (COVID-19) cases by state/province. Data source: [Johns Hopkins University Center for Systems Science and Engineering](https://systems.jhu.edu/research/public-health/ncov/)
2. [How Working-Class Life Is Killing Americans, in Charts](https://www.nytimes.com/interactive/2020/03/06/opinion/working-class-death-rate.html) by David Leonhardt and Stuart A. Thompson, *NY Times* 2020-03-06.
3. [R Studio 1.3 is out in preview](https://rstudio.com/products/rstudio/download/preview/). This is a major new release with some [appealing new features](https://rstudio.com/products/rstudio/download/preview-release-notes/). I wouldn't recommend switching over this semester to anyone who isn't comfortable with dealing with less-well-tested software, and I certainly wouldn't do it in the middle of working on anything important, but I'm experimenting with it a bit.
4. [ggplot2 version 3.3.0 is now available on CRAN](https://www.tidyverse.org/blog/2020/03/ggplot2-3-3-0/). There are some useful new features in this release, and I wouldn't expect anything to break in your current code.
5. You might be interested in this new paper: [Development and Reporting of Prediction Models](https://journals.lww.com/ccmjournal/Abstract/onlinefirst/Development_and_Reporting_of_Prediction_Models_.95713.aspx) from 2020-03-04 in *Critical Care Medicine*, subtitled Guidance for Authors From Editors of Respiratory, Sleep, and Critical Care Journals. 
    > Key topics include considerations for selecting predictor variables, operationalizing variables, dealing with missing data, the importance of appropriate validation, model performance measures and their interpretation, and good reporting practices.... Additional best practices can be found in the Transparent Reporting of a multivariable prediction model for Individual Prognosis Or Diagnosis (TRIPOD) guidelines.
    - The [TRIPOD guidelines may be found here](https://www.equator-network.org/reporting-guidelines/tripod-statement/), along with links to guidelines for randomized trials reporting (CONSORT) and reporting on observational studies (STROBE), among other things.
6. If you like that guidance, consider reading [Control of Confounding and Reporting of Results in Causal Inference Studies](https://www.atsjournals.org/doi/full/10.1513/AnnalsATS.201808-564PS) from 2018, which is also very helpful in terms of framing a lot of these issues.

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
