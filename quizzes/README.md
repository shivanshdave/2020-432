# 432 Quizzes for Spring 2020

This is where information on the course quizzes will appear. 

- Students will complete between 2 and 4 quizzes this semester - the exact number is not yet determined. All quizzes will be announced in advance and all such announcements will be posted to the web a minimum of one week prior to the Quiz becoming available.
- Quizzes in 432 are open-book, take-home affairs. Some are longer than others. Dr. Love reserves the right to make some Quizzes count more than others in determining your final Quiz grade at the end of the semester.

# Quiz 1 will be available at 5 PM on 2020-02-26. It is due at 2 PM on Monday 2020-03-02.

Quiz 1 is restricted to materials from Classes 1-11, from Chapters 1-14 in the Course Notes, and from Chapters 1-5 and 7-8 in Spiegelhalter's *Art of Statistics*. Subsequent quizzes will also include material from these sections of the course.

All questions about Quiz 1 must be directed to **431-help**. 

## The Data is already on the [Shared Google Drive](http://bit.ly/432-2020-quiz1-folder)

Two data sets are available to support your work on the Quiz. You'll find them in the [Shared Google Drive Folder for Quiz 1](http://bit.ly/432-2020-quiz1-folder) at http://bit.ly/432-2020-quiz1-folder.

- The `lind` data are provided to you in the **lind.Rds** file.
- The `riff` data are provided to you in the **riff.csv** file.

## Other Material You'll Need will appear on the [Shared Google Drive](http://bit.ly/432-2020-quiz1-folder)

By 5 PM Wednesday 2020-02-26, I will post [to that same folder](http://bit.ly/432-2020-quiz1-folder):

- a link to the Google Form Answer Sheet you'll use to submit your answers to the Quiz.
- a PDF file of the Quiz itself

## Packages I used to create the Quiz and Answer Sketch

For your information, here are the packages and themes I loaded into R to help me complete the Quiz. I used R version 3.6.2. I do not guarantee that all of these packages are actually used, but I didn't need any other packages to complete my answer sketch.

```{r packages, message = FALSE}
library(here); library(knitr); library(magrittr); library(janitor)
library(patchwork); library(tableone); library(rms); library(leaps)
library(caret); library(simputation); library(naniar); library(broom)
library(tidyverse)

theme_set(theme_bw())
```

