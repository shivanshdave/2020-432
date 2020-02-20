# 432 Spring 2020 Class 11: 2020-02-20

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 11 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class11/432_2020_slides11.pdf) | [Class 11 Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class11/432_2020_slides11.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Announcements

1. The [Homework 3 Answer Sketch](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw03) (including the grading rubric) is available now.
2. Reactions from Dr. Love and the TAs to all [Project 1 Proposals](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1#deliverable-1-the-proposal) have been posted to Canvas.
    - Everyone needs to do at least some little revision, except for the one pair of folks who've already completed theirs. 
    - All revisions for Project 1 proposals should go to the same place in Canvas where you submitted the initial draft, and **all** Project 1 Proposal revisions are due at 9 AM on Monday 2020-02-24. 
    - We encourage early submission of these revisions and additional conversation with the TAs or Dr. Love via email to 431-help or in person as you move forward. If your revision doesn't reach the level of approval (and a score of 10), you'll know that as soon as we can tell you (likely by Monday afternoon), and you'll have to revise it again, and that revision will be due at 9 AM Wednesday 2020-02-26.
    - If your initial grade on the proposal was below 8, we especially encourage you to complete your revision quickly, so that we can review it over the weekend and get you on track to a 10 as quickly as possible. 
    - Please address all the things we listed in Canvas for you to work on, as well as the list below... 

Whether we mentioned it in our comments on Canvas or not, **ALL REVISED PROJECT 1 PROPOSALS should...**
- **not** use `skim_with(numeric = list(hist = NULL), integer = list(hist = NULL))` since it leads to a lengthy and pointless function listing. If you want to skim without charts use `skim_without_charts` which came into existence in 2019.
- **not** use `source("Love-boost.R")` or any other R script or package unless you actually need somethin it provides
- load the tidyverse last, and not anywhere else, and avoid loading other packages that are loaded already by the tidyverse. The complete list of packages that the tidyverse loads is [the set of core packages listed at this link](https://www.tidyverse.org/packages/).
- should use **code-folding** in the HTML result (add code_folding: show to your YAML)
- should use the **tidyverse** for data management, almost without exception
- use `message = FALSE` in the code chunk where the packages are listed to eliminate the messages in the HTML showing warnings about when packages were built or how objects were masked
- use `comment = NA` in the setup chunk to avoid R output being preceded by hashtags `##`
- be run using **R version 3.6.2** or later, and include **session info** at the end of the document
- use the ENTER key sufficiently to prevent any code chunks in the HTML file from requiring a scrolling window in order to be seen (note that this is a particularly common problem when people list many, many packages on the same line, separated by semicolons)
- use `clean_names()` to clean up the names in the variables in the final tidied version of the data, and have no names that are longer than they need to be (10 characters or less is a good plan for variable names)
- include a **tidied version of the data file**, in .csv format, perhaps in addition to the raw data, and this tidied version should adhere to the requirements for minimum and maximum number of rows and columns, with a row (subject) identifier at the far left of the .csv file. This is a new and additional requirement for the revised proposal, to demonstrate that you've done the necessary work.

## Next Few Deliverables (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
----: | ---------------------------------------------------------------
TBA   | Project 1 Proposal Revision submitted to Canvas.
02-26 | [Quiz 1](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) will be made available.
03-02 | [Quiz 1](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) is due at 9 AM.
03-09 | [Project 1 Posters/Portfolios](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) are due at 2 PM.
