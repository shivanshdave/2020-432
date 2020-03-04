# Project 2 for 432

Complete Project 2 instructions will be posted before 1 PM on 2020-03-17.

**Right now, here's all that I am willing to commit to.**

Project 2 requires you to answer two research questions of your own choosing with data you obtain, using tools learned in the 431-432 sequence. Those questions should be amenable to regression analysis (using any sort of outcome we've discussed: quantitative, binary, multi-categorical or time-to-event.) You can study any question you like, although I’d steer clear of anything that you think Dr. Love might find inappropriate.

You can work individually or in a group of 2 people. 

Jeff Leek, in *How to be a Modern Scientist* has some excellent advice in his section on “How Do You Start a Paper.” In particular,     you want to identify a research question or (perhaps) two questions that:

- are concrete, (and for which you can find useful data), and that
- solve a real problem, and that
- give you an opportunity to do something new,
- that you will feel ownership of, and
- that you want to work on.
      
There will be three deliverables:

1. Filling out a form (that will be available on 2020-03-17: due date is 2020-04-01) to register your project and specify presentation times for which you (and your partner, if you have one) are available.
    - The form will require you to specify the project title (a real title - not "432 Project 2", and the title can have a maximum of 80 characters including spaces), your two research questions, and to provide some specific details about your data set.
    - The research questions are the toughest part of this form.
    - On the basis of this submission, Dr. Love will either approve or reject your Project 2 idea, and once he approves it, you can   proceed.
        - If he cannot approve your project, he’ll tell you why, and you’ll need to try again, by editing your response and re-submitting it.
        - The main reason why Dr. Love doesn’t approve projects is that he doesn’t understand your description of your data set, or how your research questions are linked to your data set - so you will need to focus on making those descriptions and questions as clear as possible.

2.  You will build a **written portfolio** of Project 2 materials. This will include some background, your research questions, your data management work and codebook, and then your analytic work, data descriptions, results and conclusions.
    -  You will submit the portfolio (including at least an R Markdown file and an HTML result of knitting that R Markdown file) via  Canvas. The Canvas location to submit the portfolio will go live shortly before our last class of the semester.

3. You will give a **presentation of your portfolio** to Dr. Love in his office (Wood WG 82-J). Your presentation time will be determined in early April, once the forms are in.

# Your Data

- You must completely identify the source of the data, so that Dr. Love understands what data you are using very well, but you will not be required to share the data with him, or anyone else.
- You must have any necessary approvals to use your data in a Project for this course.
    - Dr. Love does not need to see the actual data you use in Project 2, but he will see the results, naturally, and he will need to see a sample of potential values for all variables you wind up discussing in your portfolio.
    - If the data are available online, you must provide a working URL with instructions to access the data.

## Data Specifications

- You will need special approval from Dr. Love to do a project that does not have between 250 and 10,000 observations. If you're in that range, it'll be OK.
- Your final portfolio should describe a data set containing between 6 and 18 variables, not including the row identifiers (like subject IDs) although your original raw data set may contain more than 18 variables, so long as you prune it down.
    - If you are describing a binary or multi-categorical outcome, each category you are studying should happen in at least 25 rows of your data.
    - At least one of the variables (outcome or predictor) you are studying must be quantitative, and at least one must be categorical with more than two categories.
- We want you, in project 2, to have to confront the challenge of dealing with missing data via multiple imputation. If your raw data has missing values, we do not want you to reduce all of your work to complete cases, although you can compare complete case to simple imputation to multiple imputation results if you like. If your raw data has no missing values, then OK, but that's rare in "real" data.

## Suggested Data Sources

Three **especially appealing** options for Project 2 that I'd really like to see people use more are:

1. The [Health and Retirement Study](https://hrs.isr.umich.edu/data-products/access-to-public-data)
2. The [General Social Survey](https://gssdataexplorer.norc.org/)
3. The many many public use data sets available at [ICSPR](https://www.icpsr.umich.edu/icpsrweb/ICPSR/)

Other sources that students have often used in the past include:

4. [National Center on Health Statistics](https://www.cdc.gov/nchs/data_access/ftp_data.htm) including NHANES
5. [Behavioral Risk Factor Surveillance System](https://www.cdc.gov/brfss/data_documentation/index.htm)
6. [500 Cities](https://chronicdata.cdc.gov/browse?category=500+Cities)
7. [County Health Rankings](https://www.countyhealthrankings.org/explore-health-rankings/rankings-data-documentation)

## Some Restrictions on Your Data Set (What data are you *not* allowed to use?)

- You are not allowed to use data stored as a data set in any R package.
- You are not allowed to use data from a textbook or other educational resource for learning statistics, data science or related methods (online or otherwise).
- You are not allowed to use data Dr. Love or Dr. Briggs or any other faculty member at CWRU has provided to you for educational purposes.
- You cannot reuse the data you used in Project 1 for 432, although you can use a different data set to answer related questions. You are welcome to reuse data you used in your 431 project if it is suitable and you haven’t used it in Project 1 for 432.
- Dr. Love is pretty tired of data from Kaggle, from the UC Irvine Machine Learning Repository, from the Cleveland Clinic Lerner College Repository and data from data analysis competitions. Avoid those unless you can make a very strong argument for their relevance to a question of real interest to you.

## No hierarchical data!

- We want to powerfully discourage you from working with data that really require the use of multi-level models. 
      - One example would be a model of patient results that contains measures not just for individual patients but also measures for the providers within which patients are grouped, and also for health systems in which providers are grouped. 
      - Another example would be a model of individual people’s outcomes where the covariates are gathered at the state or county level, as well as at the level of individuals.
      - If your proposed research questions involve the analysis of data that are *nested* like those above, Dr. Love is probably going to reject the project. There simply isn’t time to learn the best approaches for that stuff in this context.

## Questions

> Does Project 2 have to include everything that we did in Project 1?

In Project 2, you don’t need to present everything in Project 1’s Tasks 1-9, and you’re not even required to format any of it in that way, but I would think you’d want to have most of that information at your fingertips in a presentation, so think carefully about what to keep and what to drop.


