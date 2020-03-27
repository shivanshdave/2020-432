# Project 1: Explaining the Feedback Sheet

At some point, you will receive access to a sheet from me that summarizes our feedback on your Project 1. When that becomes available, this material will be useful to you in interpreting what you receive.

# 1. Basic Summaries of Minimum Requirments that forced Dr. Love to look closely at what you did

## "Basics Complete"

This is the result of an initial minimal check. It was Yes if your project was ON TIME and included:

- R Markdown of your portfolio
- HTML of your portfolio
- R Markdown of your poster
- HTML of your poster
- Raw csv file (unless you were using NHANES data)
- Tidy RDS file
- Your Portfolio HTML includes...
    - Code-folding
    - An automated and clickable table of contents
    - Understandable (but perhaps not 100% appropriate) section headings
    - code to indicate the saving of the tidy Rds file (ideally where you were supposed to show it)
    - session information
    
## Number of Sections

- This is the number of numbered sections in the Portfolio HTML.
- 18 projects had 13, 10 had 14, 9 had 12 and the remaining one had 15.

## Most common packages explicitly loaded in portfolios

Projects | Package(s)
-------: | ------------------------------------
All 38 | `broom`, `magrittr`, `rms`, `tidyverse`
35-37 | `car`, `caret`, `here`, `janitor`, 
30-34 | `GGally`, `ROCR`, 
25-29 | `knitr`, 
20-24 | `naniar`, 
15-19 | `patchwork`, `skimr`,
10-14 | `Hmisc`, `simputation`, 
5-9 | `leaps`, `modelr`, `pROC`, `rmarkdown`, `rmdformats`, `tableone`

Less than five projects loaded the following packages...

- `arm`, `dbplyr`, `e1071`, `Epi`, `foreign`, `gridExtra` 
- `haven`, `kableExtra`, `lubridate`, `MASS`, `mice`, `mosaic`
- `nhanesA`, `plotly`, `posterdown`, `RColorBrewer`, `readxl`
- `sessioninfo`, `survey`, `vcd`, `visdat`

### Notes

- The list excludes misloads of packages that are part of the core tidyverse, and counts only once packages loaded in the same project multiple times.
- Note that loading `rms` also loads `Hmisc`.
- The mean number of packages explicitly loaded was 14.8, with a standard deviation of 3.4. The range was 9-22.

## R version used

- 34/38 students used R version 3.6.2 (2019-12-12)

## Operating Systems

- 20 used Windows
    - 16 used Windows 10 x64
    - 4 used Windows 7 x64 SP 1
- 17 used MacOS
    - 4 used macOS Catalina 10.15.3
    - 3 used macOS Mojave 10.14.6
    - 2 used macOS Catalina 10.15.2
    - 2 used macOS High Sierra 10.13.6
    - 1 each used macOS Catalina 10.15, macOS Catalina 10.15.1, macOS Mojave 10.14, macOS Mojave 10.14.2, macOS Mojave 10.14.4 and macOS Sierra 10.12.6
- 1 used Ubuntu 19.10

# 2. Description of the Linear Regression Modeling Work (Section/Task 10)

There are brief notes in the following areas, all derived from reading the Portfolio HTML document.

## Lin - Missing?

This section describes what you did about missing data in your linear regression (Section 10.)

- 28/38 used a complete case analysis, sometimes because there was no missing data to start with, and sometimes because the investigators dropped missing values.
- The other 10 did at least some simple imputation.

## Lin - Trans?

This section describes what outcome transformation you settled on in your linear regression (Section 10.)

Transformation | Inverse | Inverse Square Root | Logarithm | Square Root | None | Square 
-------------: | ---: | ---: | ---: | ---: | ---: | ---:
Projects | 1 | 1 | 11 | 13 | 9 | 3

## Lin - Augmentation

This section describes what non-linear augmentation(s) you attempted in building Model B (the augmented linear model.) 

Augmentation Type | rcs(5 knots) | rcs(4 knots) | rcs(3 knots) | Interaction Term | Polynomial Term
----------------: | ---: | ---: | ---: | ---: | ---: 
Projects | 20 | 14 | 5 | 12 | 2

Projects attempting more than one type of augmentation are listed multiple times in the table.

## Lin - Validation

This section describes what validation type(s) you attempted in comparing Models A and B. 

Validation Type | 10-fold Cross-Validation | 5-fold Cross-Validation | Training/Test Samples | `rms::validate`
-------------: | --------: | ---: | ---: | ---:
Projects | 13 | 16 | 3 | 24

Projects attempting more than one type of validation are listed multiple times in the table.

## Lin - Winner

Did the investigator(s) select Model A (main effects) or Model B (augmented) as their final linear model?

Model | A | B
------: | ---: | ---:
Projects | 23 | 15

## Lin - Final R2

What was the (validated if available) R-square value for the final linear regression model?

Value | Projects
--------: | ----:
Below 0.1 | 10
[0.1, 0.2) | 6
[0.2, 0.3) | 2
[0.3, 0.4) | 6
[0.4, 0.5) | 2
[0.5, 0.6) | 4
[0.6, 0.7) | 4
[0.7, 0.8) | 3
[0.8, 0.9) | 1
0.9 and above | 0

## Lin - Final Nomogram

Status of the nomogram for the final model

Projects | Comment
----: | --------------------------------------------------------------------
16 | OK, and appropriate back-transformation is part of the nomogram.
11 | Nomogram doesn't provide a needed back-transformation to the original outcome
9 | OK, and model did not use an outcome transformation.

# 3. Description of the Logistic Regression Modeling Work (Section/Task 11)

Again, there are brief notes in the following areas, all derived from reading the Portfolio HTML document.

## Log - Missing?

This section describes what you did about missing data in your logistic regression (Section 11.)

- 30/38 used a complete case analysis, sometimes because there was no missing data to start with, and sometimes because the investigators dropped missing values.
- The other 8 did at least some simple imputation.

## Decision Rules

This section describes what cutoff value you used in your decision rules for building Model Y and Model Z confusion matrices. Most groups (correctly) chose the same cutoff value for Model Z that they had used in Model Y.

Cutpoint | 0.5 | 0.065 | 0.1 | 0.2 | 0.3 | 0.4 | 0.8
--------: | --: | --: | --: | --: | --: | --: | --: 
Projects | 25 | 1 | 1 | 4 | 2 | 1 | 2

## Log - Augmentation

This section describes what non-linear augmentation(s) you attempted in building Model Z (the augmented logistic model.) 

Augmentation Type | rcs(5 knots) | rcs(4 knots) | rcs(3 knots) | Interaction Term | Polynomial Term
----------------: | ---: | ---: | ---: | ---: | ---: 
Projects | 10 | 15 | 8 | 18 | 2

Projects attempting more than one type of augmentation are listed multiple times in the table.

## Log - Validation

This section describes what validation type(s) you attempted in comparing Models Y and Z. 

Validation Type | 10-fold Cross-Validation | 5-fold Cross-Validation | Training/Test Samples | `rms::validate`
-------------: | --------: | ---: | ---: | ---:
Projects | 1 | 2 | - | 33

Projects attempting more than one type of validation are listed multiple times in the table.

## Lin - Winner

Did the investigator(s) select Model Y (main effects) or Model Z (augmented) as their final logistic model?

Model | A | B
------: | ---: | ---:
Projects | 26 | 12

## Lin - Final AUC

What was the (validated if available) C-statistic (area under the ROC curve) for the final logistic regression model?

Value | Projects
--------: | ----:
[0.5, 0.6) | 4
[0.6, 0.7) | 9
[0.7, 0.8) | 7
[0.8, 0.9) | 10
0.9 and above | 7

## Lin - Final Nomogram

Status of the nomogram for the final model

Projects | Comment
----: | --------------------------------------------------------------------
28 | OK, and appropriate back-transformation is part of the nomogram.
8 | Missed the opportunity to include the back-transformation to a statement about the probability of the outcome in the nomogram itself.

# 4. Comments on the Portfolio

The portfolio comments were written by Dr. Love, alone.

# 5. Portfolio Score

The score on the portfolio was out of a maximum of 25 points.

Portfolio Score | 22 or 23 | 20 or 21 | 18 or 19 | 16 or 17 | 15 or below
-----: | :---: | :---: | :---: | :---: | :---:  
Projects | 5 | 11 | 10 | 7 | 5
"Grade" | A | A- | B+ | B | B- or lower

**Please** interpret your score on the portfolio in context. 

- The appropriate scale is PERCENT = `3 x PORTFOLIO + 25`, and **not** `100 x (PORTFOLIO/25)`.
    - This accounts for the fact that most students turned in the proposal on time and received full marks there. 
- The "Grade" above applied PERCENT to the scale where A ranges from 85-100, B from 70-84, and below 70 is a problem.
