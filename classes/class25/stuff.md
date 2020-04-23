# Stuff that Dr. Love wanted to share today

## Minard's Map: A Graphical Memorial

Here are two reproductions of Charles Joseph Minard's map of Napoleon's disastrous losses suffered during the Russian campaign of 1812.

### A Large Version of the Original

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/Minard_large.png)

### A More "Modern" Presentation

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/modern-minard.png)

## On Abraham Wald 

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/wald.PNG) from [Seva Gunitsky](https://twitter.com/SevaUT/status/1097880873368801287)

- An excerpt from Jordan Ellenberg's *How Not To Be Wrong* touches on the [Wald story](https://medium.com/@penguinpress/an-excerpt-from-how-not-to-be-wrong-by-jordan-ellenberg-664e708cfc3d)

## On Building Maps

### The first map (static, built using [the sociome package](https://github.com/NikKrieger/sociome) developed by Nik Krieger)

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/cuyahoga_adi_map.png)

- See the documentation for this work as a [github markdown file](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/map_example_sociome_TEL/Ohio_sociome_by_tract.md), or in [R Markdown](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/map_example_sociome_TEL/Ohio_sociome_by_tract.Rmd).
- One thing I haven't yet done is use thematic maps, which [can produce some spectacular results](https://github.com/mtennekes/tmap).
- And if you want to produce 2D and 3D hillshaded maps of elevation matrices, you want [rayshader](https://www.rayshader.com/).

### The [more interactive map, from Better Health Partnership](http://betterhealthpartnership.org/data_center/report_22/maps/report22_overweight_obesity_map.asp) was built using `leaflet`. A screenshot follows...

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/leaflet_bhp_map.png)

- See the code (but not the data) in [R Markdown here](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/map_leaflet_TEL/leaflet_map_overweightorobese_rates.Rmd)
- If you want to learn how to build an interactive map using leaflet, I recommend [R Studio's leaflet page](https://rstudio.github.io/leaflet/), as well as learning something about using mini-charts within a leaflet visualization from [this Github repository](https://github.com/rte-antares-rpackage/leaflet.minicharts).
- Here's [another great tutorial](https://github.com/momiji15/apptomap/tree/master/R%20Ready%20to%20Map) to help you learn how to write code to collect tweets using the `rtweet` package and to display tweets on a basic interactive map using Leaflet for R.

## On Propensity Scores, Causal Inference and the Design and Analysis of Observational Studies

1. from @EpiEllie: [This is why](https://twitter.com/EpiEllie/status/1095864462664495105) your data science needs causal inference!
2. Take my 500 course next Spring.
3. Take a look at [some of the materials from a workshop I gave in 2018](https://github.com/THOMASELOVE/ichps2018) on the subject at the International Conference on Health Policy Statistics.
4. Lucy D'agostino McGowan's [Understanding propensity score weighting](https://livefreeordichotomize.com/2019/01/17/understanding-propensity-score-weighting/) may be very helpful to you.
5. Here is a [reading list of key ideas in causal inference](https://docs.google.com/document/d/1a-_VYQrZDLIAWCUs_JKvnwNT2onn-rIiLh69W53fh1o/edit) designed for a general clinical / public health audience.

## Visualization

1. Want to build your linear regression diagnostic plots using ggplot2? Take a look at [the `lindia` package](https://github.com/yeukyul/lindia).

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/lindia.png)

2. [Plots within Plots with ggplot2 and ggmap](https://statisticaloddsandends.wordpress.com/2019/02/24/plots-within-plots-with-ggplot2-and-ggmap/).
3. from Timo Grossenbacher, some [bivariate maps with ggplot2 and sf](https://timogrossenbacher.ch/2019/04/bivariate-maps-with-ggplot2-and-sf/)
4. The [colorblindr package](https://github.com/clauswilke/colorblindr) may be of interest to some of you. It lets you make a figure in ggplot2 and then look at it in various color-vision-deficiency simulations. Still doesn't cover everyone, but it might help a bit. It also provides an alternative to viridis that some people like. [Color Oracle](https://colororacle.org/) can also help.
5. [25 examples of tables built using the `gt` package in R](https://frm1789.github.io/gt_examples/).
6. In my early days learning to visualize data in R, the most useful book for me was Winston Cheng's [R Graphics Cookbook](https://r-graphics.org/), and the second edition is [available online, for free](https://r-graphics.org/)!

## Learning and Using R

1. Here is a [community-sourced data science repository](https://github.com/Chris-Engelhardt/data_sci_guide). The overarching goal here is to provide anyone interested in learning data science with a wealth of open source, industry-best learning materials and learning tracks. This started out with the [links for learning more about data science provided in this Twitter stream](https://twitter.com/EngelhardtCR/status/1116743032492253185).
2. These [Data Science primers](https://rstudio.cloud/learn/primers) built [using the learnr package](https://rstudio.github.io/learnr/) are fantastic!
3. [Dataquest.io](https://www.dataquest.io/) may be an attractive way to learn something specific we haven't covered. The Data Analyst in R pathway appears to be free, at least, at the moment.
4. If you're interested in [Advanced R, by Hadley Wickham](http://adv-r.had.co.nz/), you're probably also interested in [this solutions manual](https://advanced-r-solutions.rbind.io/).
5. You may also be interested in [Hadley's R Packages](http://r-pkgs.had.co.nz/) book.
6. Some [great resources (and demos) are gathered here by Mara Averick](https://connect.rstudioservices.com/content/282/gov1005.html)
7. Want to create dynamic dashboards using the shinydashboard R package? [Check this out](https://leanpub.com/c/shinydashboard).
8. Some people complain about using R, instead of some other software. If you get this complaint, take a look [at this Twitter stream](https://twitter.com/SameerDesai1/status/1095907255755526145).

## Important Issues in Statistics

1. [Large studies reduce random error, but not systematic error](https://twitter.com/aztezcan/status/1119233306300563460)
2. I can also recommend Brian Caffo's [Regression Models for Data Science in R](https://leanpub.com/regmods), and Roger Peng's [Exploratory Data Analysis with R](https://leanpub.com/exdata) and Rafael Irizarry's [Introduction to Data Science](https://leanpub.com/datasciencebook).
3. [ModernDive remains a terrific resource](https://moderndive.com/) for statistical inference via data science.
4. Interested in implementing machine learning ensemble strategies, like the SuperLearner? Check out [Alex Hayes' post using tidymodels to implement the SuperLearner](https://www.alexpghayes.com/blog/implementing-the-super-learner-with-tidymodels/).
5. Check out this article by Bates, Machler, Bolker and Walker on [Fitting Linear Mixed-Effects Models using lme4](https://www.jstatsoft.org/article/view/v067i01/0?utm_campaign=digest&utm_medium=email&utm_source=nuzzel)
6. You may be interested in [Maverick Lin's 10-page "cheat sheet" about data science](https://www.datasciencecentral.com/profiles/blogs/new-data-science-cheat-sheet), which is inspired by William Chen's [The Only Probability Cheatsheet You'll Ever Need](https://www.datasciencecentral.com/profiles/blogs/probability-cheat-sheet).
7. An extremely useful idea is that of splitting continuous predictors into thirds, rather than dichotomizing, [as described here](http://www.stat.columbia.edu/~gelman/research/published/thirds5.pdf). If you must categorize, think about the gains in efficiency this approach can provide.
8. Here's a nice video from David Spiegelhalter on "[What would Florence Nightingale make of big data](https://www.bbc.com/ideas/videos/what-would-florence-nightingale-make-of-big-data/p075lxkt?playlist=thinkers-from-the-past-on-the-world-today)?"
9. From Darren Dahly, [here is a simulation to demonstrate how you should decide which covariates to adjust for in the context of a randomized controlled trial.](https://threadreaderapp.com/thread/1115902270888128514.html). There's an excellent follow-up series of posts, [from Frank Harrell and others at this link](https://twitter.com/f2harrell/status/1116311832652910597).
10. "[A Second Chance to Get Causal Inference Right: A Classification of Data Science Tasks](https://amstat.tandfonline.com/doi/full/10.1080/09332480.2019.1579578#.XNBr545JGUm)" from Miguel A. Hernán, John Hsu & Brian Healy in *Chance*. Find it at https://doi.org/10.1080/09332480.2019.1579578
11. "[Calculating Observed Power is Like Believing in Fairy Tales](https://lesslikely.com/statistics/observed-power-magic/) at [LessLikely](https://lesslikely.com/)
    - "A discussion of events that transpired in 2018-19, where a group of surgical researchers decided to ignore much of the statistical literature and promote a highly misleading practice of calculating post-hoc power using the observed effect size."
    - Some related pieces at LessLikely include "[When Can We Say That Something Doesn't Work?](https://lesslikely.com/statistics/evidence-of-absence/)" and "[Misplaced Confidence in Observed Power](https://lesslikely.com/statistics/misplaced-power/)"


## [Ten Simple Rules for Effective Statistical Practice](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004961)

This insightful article from Robert E. Kass, Brian S. Caffo, Marie Davidian, Xiao-Li Meng, Bin Yu, and Nancy Reid in 2016 in [PLOS Computational Biology](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004961) as part of their "Ten Simple Rules" series is very helpful. The Ten Rules are...

1. Statistical Methods Should Enable Data to Answer Scientific Questions
2. Signals Always Come with Noise
3. Plan Ahead, Really Ahead
4. Worry about Data Quality
5. Statistical Analysis Is More Than a Set of Computations
6. Keep it Simple
7. Provide Assessments of Variability
8. Check Your Assumptions
9. When Possible, Replicate!
10. Make Your Analysis Reproducible

### A few other great "Ten Simple Rules" pieces to explore...

- [Ten Simple Rules for Graduate Students](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.0030229) by Gu J Bourne PE 2007
- [Ten Simple Rules for Better Figures](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003833) by Rougier NP Droettboom M Bourne PE 2014
- [Ten Simple Rules for Creating a Good Data Management Plan](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004525) by Michener WK 2015

I'll also remind you of the existence of [the References page](https://github.com/THOMASELOVE/2020-432/blob/master/references/README.md), which has all sorts of good things to read.

## Why Do Replicable/Reproducible Research?

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/broman1.png) 

- That's from Karl Broman who has some [initial steps toward reproducible research](https://kbroman.org/steps2rr/)

## Advice for Graduate Students, from David Robinson

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class25/figures/gradschool.PNG)


