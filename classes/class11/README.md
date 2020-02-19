# 432 Spring 2020 Class 11: 2020-02-20

## Key Materials

Slides in PDF | Slides in R Markdown | Audio Recording | Need Help?
------------: | :------------------: | :--------------: | ---------------------------
[Class 11 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class11/432_2020_slides11.pdf) | [Class 11 Rmd](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class11/432_2020_slides11.Rmd) | [Shared Drive](http://bit.ly/432-2020-audio) | Email **431-help at case dot edu** or visit [Office Hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#tas-and-office-hours)

## Today's Announcements

1. The [Homework 3 Answer Sketch](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw03) (including the grading rubric) is available now.
2. As of 6:30 PM on 2020-02-19, reactions to 26 of the 38 Project 1 Proposals have been posted to Canvas, and reactions to the remaining 12 (all of which had initial scores from the TAs of 9 or 10) will be posted by class time on Thursday. Dr. Love will provide more details (including deadlines for revisions) between now and Thursday's class, once he has posted Canvas reactions to all 38 proposals.

Whether we mentioned it in our comments on Canvas or not, to be approved, **ALL REVISED PROPOSALS should...**
- use `message = FALSE` in the code chunk where the packages are listed to eliminate the messages in the HTML showing warnings about when packages were built or how objects were masked
- use `comment = NA` in the setup chunk to avoid R output being preceded by hashtags `##`
- be run using **R version 3.6.2** or later, and include **session info** at the end of the document
- should use **code-folding** in the HTML result (add code_folding: show to your YAML)
- should use the **tidyverse** for data management, almost without exception
- include a **tidied version of the data file**, in .csv format, perhaps in addition to the raw data, and this tidied version should adhere to the requirements for minimum and maximum number of rows and columns, with a row (subject) identifier at the far left of the .csv file.
- use the ENTER key sufficiently to prevent any code chunks in the HTML file from requiring a scrolling window in order to be seen (note that this is a particularly common problem when people list many, many packages on the same line, separated by semicolons)
- use `clean_names()` to clean up the names in the variables in the final tidied version of the data, and have no names that are longer than they need to be (10 characters or less is a good plan for variable names.)

## Next Few Deliverables (from [the Course Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md))

Date | Deliverable
----: | ---------------------------------------------------------------
TBA   | Project 1 Proposal Revision submitted to Canvas.
02-26 | [Quiz 1](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) will be made available.
03-02 | [Quiz 1](https://github.com/THOMASELOVE/2020-432/tree/master/quizzes) is due at 9 AM.
03-09 | [Project 1 Posters/Portfolios](https://github.com/THOMASELOVE/2020-432/tree/master/projects/project1) are due at 2 PM.
