# 432 Spring 2020 Class 05: 2020-01-28

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Week 03 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class05/432_2020_week03.pdf) | [Week 03 .Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class05/432_2020_week03.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Next Few Deliverables (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
---------: | -----------------------------------------------------------------------
Today | [Homework 1](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw01) due at 5 PM.
2020-01-31 | Minute Paper after Class 06 (**link to come**) will be due at 2 PM.
2020-02-04 | [Homework 2](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw02) due at 5 PM.
2020-02-05 | You should have your data for [Project 1](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) in hand.
2020-02-06 | Read *The Art of Statistics* Chapter 7 (Estimates and Intervals)
2020-02-11 | [Homework 3](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw03) due at 5 PM.
2020-02-14 | [Project 1 Proposal](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) due at 2 PM.

## Today's Announcements

1. The [Class 03](https://github.com/THOMASELOVE/2020-432/tree/master/classes/class03) and [Class 04](https://github.com/THOMASELOVE/2020-432/tree/master/classes/class04) Slides have been edited to reflect what we actually discussed each day, and reposted accordingly.
2. Thank you for completing the [Minute Paper after Class 4](http://bit.ly/432-2020-minute-04). By now, I hope you've had the chance to [review the feedback I posted Friday](http://bit.ly/432-2020-minute-04-feedback). Our next Minute Paper will be after Class 6.
3. When sending us a request for help at **431-help** it's extremely helpful for you to send your entire R Markdown file, in addition to pointing out whatever specific issue is concerning you. This will help us respond faster and more accurately.
4. If you're having trouble figuring out how to do something in R, consider looking at [the r-basics document](https://github.com/THOMASELOVE/2020-432/tree/master/r-basics). It's not perfect, but it does cover a lot of common issues. Section 8.3, for instance, shows a method for creating a multi-categorical factor from a quantitative variable.
5. **On jittering in an interaction plot**. A student pointed out to me that the jittering in one of our plots was a bit confusing. [Here's a quick example displaying the problem and a possible solution](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class05/quick_example.md).
6. **[Course Notes](https://thomaselove.github.io/2020-432-book/) Updated**. I made some meaningful progress revising and updating [the 2020 Course Notes](https://thomaselove.github.io/2020-432-book/). 
    - You'll find some small revisions before Chapter 3, substantial revisions to Chapter 3, and new Chapters 4-9, which should provide ample material to supplement the slides through this week.
7. About Your [Project 1](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) Data.
    - **No multi-level data in Project 1**. As in 431, we don't want you working with multi-level data in 432 Project 1. An example of multi-level data (for which a multi-level model would be necessary) would be a setting where you study measures on individual patients as well as measures on health systems in which the individual patients are grouped. Hierarchical or multi-level models are extensions of the linear and generalized linear models we want you to use in Project 1. So, avoid nested data, where data for participants are organized at more than one level, please.
    - **Google Dataset Search** If you're looking to find a data set for Project 1, [Google Dataset Search](https://datasetsearch.research.google.com/) just [came out of beta](https://blog.google/products/search/discovering-millions-datasets-web/).
8. There's a new R package called `wikitablr` which has tools to help you [simply webscrape tables from Wikipedia](https://github.com/jkeast/wikitablr), and clean them up. It looks like it could be useful.

