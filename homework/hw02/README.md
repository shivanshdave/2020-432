432 Homework 2
================

# General Instructions

Submit your work via [Canvas](https://canvas.case.edu/). The deadline is
specified on [the Course
Calendar](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md).

  - Your response should include an R Markdown file and an HTML document
    that is the result of applying your R Markdown file to the
    `hbp432.csv` data, available in the data subfolder for this
    homework, as well as on our Data and Code page. - Start a separate R
    Project for Homework 2, as your first step, and place the data in
    that project’s directory or (perhaps better) in a data
    sub-directory.
  - In all of our homeworks, do not include R output without complete
    sentences describing what you are doing in each step, and what you
    conclude from that work.

## Question 1. (20 points)

Develop at least one useful and attractive visualization of the data in
the `hbp432` file that we used in Homework 1, that helps us to
understand the association between the `practice` where a subject is
seen for care, their `insurance` status and their `income` level.

  - Use the wisdom provided in Spiegelhalter’s first five chapters
    (particularly Chapters 2 and 4) for guidance in developing your
    Question 1 response, and (in your Question 2 response) specify what
    you learned from Spiegelhalter that motivated your choices.

## Question 2. (20 points)

Write 150-250 words in complete sentences to describe the purpose of
your Question 1 visualization(s), and to explain what you are trying to
convey. As mentioned, specify what you learned from Spiegelhalter
directly, and connect it to your visualization(s) explicitly.

## Question 3. (20 points)

Use the `hbp432` data to fit and interpret an ANOVA model to evaluate
the effect of `race` on `income`. What conclusions can you draw? In
developing an answer, please decide whether collapsing the `race` factor
into a smaller number of levels would be sensible in this case. You’ll
also want to assess the role of missingness in this work, and consider
removing the cases with missing values (or imputing them with simple
imputation) if they include only a small fraction of the total sample.
Be sure to provide a written explanation of your findings, in complete
sentences.

## Question 4. (20 points)

Now fit a two-factor ANOVA model to evaluate the effects of `race`
(either collapsed or uncollapsed, as you decide) and `sex` on `income`.
What can you conclude? Be sure to provide a written explanation of your
findings, in complete sentences. Your answer for Question 2 is not
complete unless you provide a plot that helps you decide whether an
interaction term is useful.

## Question 5. (20 points)

Now attempt to fit a two-factor ANOVA model to evaluate the effect of
`race` and `insurance` on `income`. Note that a problem should occur
when you fit this `race` and `insurance` model, that doesn’t happen, for
instance, when you evaluate the effects of both `race` and `sex` on
`income`. So what happens when you fit the `race`-`insurance` model,
exactly, and why does it happen? (Note that a plot regarding interaction
may or may not be helpful, but is not needed in your response to
Question 5.)

  - Here’s a hint…

> R may well warn you about “singularities” in your output for Question
> 5, but we’d like a clearer answer than that from you. To obtain it,
> consider exploratory data analysis, specifically the value of counting
> things. In particular, ask yourself questions like “How many people
> fall into the levels of the product term I’ve created?” or “What if I
> build a table, say with race in the rows and insurance in the columns
> - how many people fall into each cell of that table?” as a way to
> figure out what the real problem is.

  - And here’s another hint …

> In order to see this problem, you’ll need to have at least three
> `race` groups (so if you’ve collapsed the original data more than
> that, don’t - at least for question 5) and you’ll need to fit an
> interaction term, and look at more than just the `anova` results, but
> in fact also summarize the linear model.

### Please add the session information.

Finally, at the end of this homework and all subsequent assignments
(including the projects), please add the session information. My
preferred way for you to do this is:

``` r
sessioninfo::session_info()
```

### This is the end of Homework 2.
