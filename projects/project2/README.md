# Project 2 for 432

# This material is a work in progress. There will be a final version posted before class on Thursday 2020-03-19.

# The Four Deliverables

1. The Project 2 Proposal Google Form, due 2020-04-01.
2. The Main Project 2 Document (which includes R Markdown and HTML files, plus an tidied .Rds file), due 2020-05-04.
3. The Project 2 (recorded) Video Presentation, due 2020-05-04.
4. The End-of-Term Google Form, also due 2020-05-04.

-----------

# The Project 2 Proposal Google Form

*Details to come.*

## Advice on Developing a Research Question

Straightforward questions with a clear link to models we’ve studied or studying are the best option.

Jeff Leek, in his book [How to be a Modern Scientist](https://leanpub.com/modernscientist) has some excellent advice on this. In particular, identify a research question that:

- is concrete, (and for which you can find useful data), and that
- solves a real problem, and that
- gives you an opportunity to do something new,
- that you will feel ownership of, and
- that you want to work on.

I’ll add that your research question needs to be reasonable and plausible given the constraints on your time and energy. This is the time to develop something that can work in this setting, not try to boil the ocean. 

## Suggested Data Sources

Three especially appealing sources that I'd really like to see people use for Project 2 are:

1. The [Health and Retirement Study](https://hrs.isr.umich.edu/data-products/access-to-public-data)
2. The [General Social Survey](https://gssdataexplorer.norc.org/)
3. The many many public use data sets available at [ICSPR](https://www.icpsr.umich.edu/icpsrweb/ICPSR/)

Other sources students have used successfully in the past and that I’m happy to see include:

4. [National Center on Health Statistics](https://www.cdc.gov/nchs/data_access/ftp_data.htm) including NHANES
5. [Behavioral Risk Factor Surveillance System](https://www.cdc.gov/brfss/data_documentation/index.htm)
6. [500 Cities](https://chronicdata.cdc.gov/browse?category=500+Cities)
7. [County Health Rankings](https://www.countyhealthrankings.org/explore-health-rankings/rankings-data-documentation)

## Data Set Specifications/Requirements

- Dr. Love strongly prefers that you use data that can be shared with anyone in the world, but this is not mandatory.
- You will need special approval from Dr. Love (email him to ask for it before submitting the Proposal Form) to do a project that does not have between 250 and 10,000 observations. Anything in that range is fine, and if your data include meaningfully more than 10,000 observations, it’s OK to start by sampling them.
- Repeating a few things from the Tidying Data section...
      - Your final analytic tibble must contain between 250 and 10,000 observations on between 5 and 15 variables, excluding the row identifiers (like subject IDs.) 
      - If you have a categorical variable in your final analytic tibble, each category in that variable should happen in at least 25 rows of your data. If that's not the case, you'll have to collapse some categories together.
      - At least one of the variables (outcome or predictor) you are studying must be quantitative, and at least one must be categorical with 3 or more categories.

## Some Restrictions (What data are you *not* allowed to use?)

- No projects on coronavirus or COVID-19, please. If it is important to you to do work in that area, please do it in the setting of [Homework 5](https://github.com/THOMASELOVE/2020-432/tree/master/homework/hw05).
- No data stored as part of any R package, without Dr. Love’s express approval (send email to request approval before submitting the proposal form.)
- You are not allowed to use data from a textbook or other educational resource for learning statistics, data science or related methods (online or otherwise).
- You are not allowed to use data Dr. Love or Dr. Briggs or any other faculty member at CWRU has provided to you for educational purposes.
- You cannot reuse the data from your 432 Project 1, although you can use related data to answer related questions. You are welcome to reuse data you used in your 431 project if it is suitable and you haven’t used it in Project 1 for 432.
- No hierarchical data. We want to powerfully discourage you from working with data that really require the use of multi-level models.
      - One example would be a model of patient results that contains measures not just for individual patients but also measures for the providers within which patients are grouped, and also for health systems in which providers are grouped. 
      - Another example would be a model of individual people’s outcomes where the covariates are gathered at the state or county level, as well as at the level of individuals. 
      - If your proposed research question involves the analysis of data that are nested like those above, we will reject the project. There simply isn’t time to learn the best approaches for that stuff in this context.
- Dr. Love is pretty tired of data from Kaggle, from the UC Irvine Machine Learning Repository, from the Cleveland Clinic Lerner College Repository and data from data analysis competitions. Avoid those unless you can make a very strong argument for their relevance to a question of real interest to you.

-----------

# The Main Project 2 Document and its Eight Sections

A key deliverable for Project 2 is an R Markdown document (and HTML result) which includes the eight sections described below. 
Your R Markdown document must create an HTML result containing:

- a meaningful title (of 80 characters or less) that describes your research question, 
- an automated table of contents, and 
- attractive HTML formatting (the approaches used in any of the Project 1 templates would be fine in terms of formatting) 
- load the tidyverse last, and not anywhere else, and avoid loading other packages that are loaded already by the tidyverse. The     complete list of packages that the tidyverse loads is [the set of core packages listed at this link](https://www.tidyverse.org/packages/).
- should use **code-folding** in the HTML result (add code\_folding: show to your YAML)
- should use the **tidyverse** for data management, almost without exception
- use appropriate subsection headings (which you identify with hashtags on new lines in your R Markdown file) and with numbers     automatically applied by R to match the section numbering specified below.
- Be sure `number_sections: true` is in your YAML section at the top of your R Markdown file.
      - To create a numbered section called “Data Source”, use the code `# Data Source` preceded and followed by a blank line in your R Markdown file
      - To create a numbered subsection called “First Source”, use the code `## First Source` preceded and followed by a blank line in your R Markdown file
      - To create an unnumbered section called “Packages”, use the code `# Packages {-}` preceded and followed by a blank line in your R Markdown file
- use `message = FALSE` in the code chunk where the packages are listed to eliminate the messages in the HTML showing warnings about when packages were built or how objects were masked
- use `comment = NA` in the setup chunk to avoid R output being preceded by hashtags `##`
- be run using **R version 3.6.2** or later, as demonstrated in your session information section.

## Section 1 should be labeled Preliminaries

Here, you will load all necessary R packages for the work you are doing.

## Section 2 should be labeled Research Question

Here, you will identify and describe a researchable question that is amenable to study using statistical tools that are associated with the 432 course.

- A question is expressed so as to elicit information, and ends with a question mark. Make the question the high point of this Section.
- The question must be one that lends itself well to the use of a regression model (you are welcome to adapt any regression modeling strategy connected to the 432 course) to develop an answer.

You can study anything you like, so long as you steer clear of things that Dr. Love thinks are inappropriate for a course project.
Before stating the question, provide as much background as is necessary for an intelligent person not familiar with the field of interest that encompasses your research question.

- For example, if your question is about genomics, do not assume the reader has a substantial education in genomics.  If your question is about sports, do not assume the reader is a sports fan. Avoid field-specific jargon.
- Assume that your reader has as clear an understanding as you do of all of the material we’ve discussed in our 431 and 432 classes.

## Section 3 should be labeled Data Source (or Sources)

Here, you must completely identify the source(s) of the data, so that Dr. Love understands what data you are using very well.

- Should the data be available online, you must also provide a URL where the reader can access the data in this section.
- Should the data not be available online, you must provide a detailed description of where the data come from, how it was gathered, and any restrictions that apply (for instance, if the data are not available to the public, be sure that we know that.) 
- You must also provide in this section evidence that you have any and all necessary approvals to use your data in a Project for this course.

By the end of this section, make it completely clear to the reader why your chosen data is worthy of exploration in the context of your question.

## Section 4 should be labeled Ingesting and Tidying the Data

Begin this section by loading in the data you will use.

Next, we want to see the work required to manage and tidy the data into the form you used for your analyses. 

- Do not show sanity checks or false starts. Instead, stick to presenting only the activities which are needed to turn the initial data into the analytic tibble you will use for your analyses.
- Use subsections to delineate the management tasks you perform, and provide guidance in English in between the code chunks that helps the reader understand what you are doing every step of the way.
- If you have a categorical variable in your final analytic tibble, each category in that variable should happen in at least 25 rows of your data. If that's not the case, you'll have to collapse some categories together.
- At least one of the variables (outcome or predictor) you are studying must be quantitative, and at least one must be categorical with 3 or more categories.
- On Dealing with Missingness
      - If you have missing data in an outcome or key predictor variable, we want you to drop those values from your data set in this tidying process.
      - If you have missing data in any other variable, we want you to discuss here whether a missing at random assumption is reasonable.
            - If so, we want you to use multiple imputation in generating your final analyses (although you are encouraged to consider simple imputation or complete case approaches in your intermediate analytic steps.)
            - If not, we suggest you reduce the scope of your data set to eliminate either the observations that are not missing at random, or to eliminate the variables containing those missing values.

The next to last subsection of Section 4 should be a listing of your final analytic data set (just type its name) to prove that you have generated a tibble in R. Call this subsection **Listing the Analytic Tibble**

- This tibble should include any columns of identifying information for the subjects that you deem necessary, plus the variables you intend to use in your Data Analysis.
- Your tibble listing must be the result of a single line of code where you call the name of the data set. You cannot manipulate it in any way.
      - As it will be a tibble, this listing should provide Dr. Love (in the HTML) with a correct count of the number of rows and number of columns in your analytic data set.
- Your final analytic tibble as shown in this Section and used in the codebook and analyses that follow must contain between 250 and 10,000 observations on between 5 and 15 variables, excluding the row identifiers (like subject IDs) although your original raw data set may contain more than 10,000 observations and/or more than 15 non-identification variables, so long as you prune it down to fit within that limit in this Section.

The final subsection of Section 4 should be a single line of code where you save the final analytic tibble to an .Rds file. Call this subsection **Saving the Analytic Tibble**.

- If Dr. Love is permitted to have access to your data, you will then provide that .Rds file to him as part of your Canvas submission at the end oft he term.
- If Dr. Love is not permitted to have access to your data, you will need to provide an .Rds file containing two randomly selected and de-identified rows from your tibble.

## Section 5 should be labeled Codebook

Produce a codebook for the variables that you intend to use in your Data Analysis. For each variable, provide the following in an attractive and user-friendly format:

- its name in the tibble you printed at the end of Section 4; be sure that every variable in the Codebook is in the Analytic Tibble
- a description of what the variable means, in English, with appropriate units of measurement specified, or in the case of categorical variables, a description of each possible level of the variable
- the type of variable (quantitative, count, binary, ordered multi-categorical, unordered multi-categorical, or censored time-to-event)
the number of missing values contained in the Analytic Tibble for that variable.

## Section 6 should be labeled Data Analysis

This includes your work to Transform, Visualize and Model your data so as to address your research question. 

- You are welcome to use any reasonable strategy connected to **either 431 or 432** or even something else you’ve learned about to visualize and transform the data.
- You can adapt any **regression modeling strategy connected to the 432 course** to model the data. 

Present the material here in an order that makes sense to you as being of maximum value to your reader. 

- Do not present detours or false starts or sanity checks that detract from the main analyses you wish to present.
- Use subsections to delineate separate analytic tasks, and to guide the reader.

End this section with a clear description of the final model you settle on, remembering that this may require multiple imputation.

## Section 7 should be labeled Conclusions

Here, you will describe, in complete English sentences, what you have learned about your research question by doing the work in the previous sections. 

- Be sure to begin your Conclusions section by restating the research question in new words and then providing a clear answer (which is not likely to be a completely definitive answer) to your question.
- The remainder of the Conclusions section should discuss the strengths and limitations of your approach, and also comment on possible next steps and describe what you would now do differently in studying this question (if anything) having gone through this experience. 
- A good Conclusions section will likely require between 250 and 500 words.
 
## Section 8 should be labeled Session Information

Here, you will include the R session information, using `sessioninfo::session_info()`.

-----------

# The Project 2 (Recorded) Video Presentation

This is a short pre-recorded video presentation where you display and discuss whatever you feel are the most important parts of Sections 6 and 7 of your document. The deadline is also 2020-05-04, submitted via Canvas.

- **Working Alone?** Your presentation should be 3-4 minutes in length.
- **Working with a Partner?** You will provide two separate presentations (one from each of you) each of 3-4 minutes in length, along with a written note indicating which of your two presentations should be watched first. 

At a minimum, your presentation should specify your research question, highlight key findings, demonstrate the model you developed, and answer the research question. 

- Given the short length of the presentation, that’s probably all you’ll be able to do.
- The first thing you will do on any recording is introduce yourself by name.
- After that, I don’t need to be able to see your face - so it’s fine (and appropriate) to show results from a slide deck or from your portfolio. Be sure I can see and hear your video clearly.
- If you use **slides** rather than your main document in your presentation, please submit them via Canvas as well so that I can follow along.

-----------

# The End-of-Term Google Form

You will complete an end-of-term Google Form also due 2020-05-04, where you will be ...

1. asked to summarize the key finding of your study briefly in your own well-chosen set of 50 or fewer words, and 
2. asked about the most important thing you’ve learned in 432, 
3. asked about the next step you’re most eager to take in developing yourself as a data scientist, and 
4. asked about the most important piece of advice you wished you’d heard when starting the 431-432 sequence. 

If you’re working as a pair, each of you must submit the end-of-term Google Form separately. We will post the end-of-term Google Form by mid-April.

-----------

# Grading Project 2

All students who complete all Project 2 elements on time, while attending to each of the requirements listed above will earn an A grade on Project 2.

# Questions?

Questions about Project 2 should be directed to `431-help`.

