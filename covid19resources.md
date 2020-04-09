# Data and Resources related to COVID-19

## Posted during the week of 2020-04-06

- FiveThirtyEight Video Podcast: [Why Forecasting COVID-19 Is Harder Than Forecasting Elections](https://fivethirtyeight.com/videos/why-forecasting-covid-19-is-harder-than-forecasting-elections/) by Galen Druke, Laura Bronner and Maggie Koerth (from 2020-04-03). Related FiveThirtyEight pieces include:
    - [Why It’s So Freaking Hard To Make A Good COVID-19 Model](https://fivethirtyeight.com/features/why-its-so-freaking-hard-to-make-a-good-covid-19-model/) by Maggie Koerth, Laura Bronner and Jasmine Mithani (2020-03-31)
    - [When Is It Safe To Go Outside?](https://fivethirtyeight.com/features/a-crowded-park-isnt-much-safer-than-a-crowded-movie-theater/) by Kaleigh Rogers (2020-04-01)
    - [Science Has No Clear Answers On The Coronavirus. Face Masks Are No Exception](https://fivethirtyeight.com/features/science-has-no-clear-answers-on-the-coronavirus-face-masks-are-no-exception/) by Maggie Koerth (2020-04-06)
    - [Coronavirus Case Counts Are Meaningless *Unless you know something about testing. And even then, it gets complicated*.](https://fivethirtyeight.com/features/coronavirus-case-counts-are-meaningless/) by Nate Silver (2020-04-04)
    - [Best-Case And Worst-Case Coronavirus Forecasts Are Very Far Apart](https://fivethirtyeight.com/features/best-case-and-worst-case-coronavirus-forecasts-are-very-far-apart/) by Jay Boice and Anna Wiederkehr (2020-04-02)
- There's a lot of good data science work being done related to COVID-19, and, as Mark Alan Fontana points out, [a lot of scary stuff, too](https://twitter.com/metamaf/status/1245816735309193216).
- Rob Hyndman on [Why log ratios are useful for tracking COVID-19](https://robjhyndman.com/hyndsight/logratios-covid19/) shows how to use the new `tidycovid19` package to build graphs like this:
    
![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class20/figures/hyndman1.png)

- In that same post, Rob discusses why per capita numbers aren't shown instead, and describes the value of looking at log ratios.
- Rob also links to Kieran Healy's [Get Your Epidemiology from Epidemiologists](https://kieranhealy.org/blog/archives/2020/03/21/covid-19-tracking/) post, which shows R code to create this plot:

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class20/figures/covid_cumulative_22-03-20.png)
    
- Kieran Healy also has a very interesting post called [A COVID Small Multiple](https://kieranhealy.org/blog/archives/2020/03/27/a-covid-small-multiple/) which shows you how to build this...
    
![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class20/figures/cov_case_sm.png)

- [MetroHealth Releases COVID-19 Projections](https://news.metrohealth.org/metrohealth-releases-covid-19-projections/) (2020-04-07)
- I've posted them before, but [shinyps1 has new pictures of the evolution by state in the US](https://twitter.com/shinyps1/status/1247743234358390790) as of 2020-04-07.
- [Data.world COVID-19 Resources](https://data.world/resources/coronavirus/)
- [Interminable Meetings Found Ineffective for Treatment of COVID-19](https://twitter.com/hmkyale/status/1247578342825566216)
- [Broadstreet COVID-19 Data Project](https://covid19dataproject.org/) is a volunteer driven data collection and presentation effort.
- [Some Select COVID-19 Modeling Resources](https://rviews.rstudio.com/2020/04/07/some-select-covid-19-modeling-resources/) by Joseph Rickert at R Views (RStudio's R Community Blog)

## Things Posted During the Week of 2020-03-27

- [IHME (University of Washington) COVID-19 Projections](https://covid19.healthdata.org/projections), and some of [these tweets from Carl T. Bergstrom](https://twitter.com/CT_Bergstrom/status/1244815009303023616?s=20) are motivating my thoughts. 
    - I want to try to help you spread the word to people who haven't caught on to the distinction between the UW model and other models (like the initial Imperial College projections - see [Report 9 here](https://www.imperial.ac.uk/mrc-global-infectious-disease-analysis/covid-19/).)
- [Why It’s So Freaking Hard To Make A Good COVID-19 Model](https://fivethirtyeight.com/features/why-its-so-freaking-hard-to-make-a-good-covid-19-model/) at 538.
- [COVID-19 Info Posters](https://github.com/eleanormurray/COVID_19) by Dr Ellie Murray in collaboration with Dr Benjamin Linas and the Boston Medical Center. In many, many languages, now.
    - Five Tips for Everyone (shown above)
    - What to do if you're waiting for a COVID test result
    - What to do if you have tested positive for COVID
    - What to do if you are feeling sick but haven't been (or can't get) tested
    - What to do if you have been in contact with someone with known or suspected COVID
- Coursera Course on "[Fighting COVID-19 with Epidemiology](https://www.coursera.org/learn/covid19-epidemiology)" starts 2020-03-31 online.
- [Bill Petti's Shiny app for COVID-19 data and charts](https://billpetti.shinyapps.io/covid_19_country_state_dashboard/)
- [Johns Hopkins CSSE's data repository for COVID-19](https://github.com/CSSEGISandData/COVID-19)
- Jesse Burk-Rafel's [summary of all current COVID19 Clinical Trials](http://bit.ly/COVIDtrials) at http://bit.ly/COVIDtrials.
    - includes Google Sheet and Infographic.
- [We’re Sharing Coronavirus Case Data for Every U.S. County](https://www.nytimes.com/article/coronavirus-county-data-us.html) *NY Times* 2020-03-28.
- [University of Washington COVID-19 model dashboard](https://covid19.healthdata.org/projections)
    - "The charts show projected hospital resource use based on COVID-19 deaths."


## Things posted prior to 2020-03-27 by TEL

- Health Policy Institute of Ohio: [Coronavirus (COVID-19) in Ohio Latest News](https://www.healthpolicyohio.org/coronavirus-covid-19-in-ohio/)
- Johns Hopkins University [Coronavirus Resource Center](https://coronavirus.jhu.edu/)
    - [Interactive Map of Coronavirus COVID-19 Global Cases](https://coronavirus.jhu.edu/map.html) by the Center for Systems Science and Engineering
    - [Dashboard](https://www.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6)
    - [Mapping 2019-nCov](https://systems.jhu.edu/research/public-health/ncov/) by Lauren Gardner
- World Health Organization [Rolling updates on coronavirus disease (COVID-19)](https://www.who.int/emergencies/diseases/novel-coronavirus-2019/events-as-they-happen)
- Centers for Disease Control and Prevention [Coronavirus (COVID-19) page](https://www.cdc.gov/coronavirus/2019-ncov/index.html)
    - Data on [Cases in the U.S.](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html)
- Our World in Data: [Coronavirus Disease (COVID-19) Statistics and Research](https://ourworldindata.org/coronavirus) by Max Roser, Hannah Ritchie and Esteban Ortiz-Ospina
- Novel Corona Virus 2019 Dataset: Day level information on covid-19 affected cases [hosted at Kaggle](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset)
- [The COVID Tracking project](https://covidtracking.com/)
- Bob Winkelman and Colin Waltz
    - [Shiny App exploring US COVID-19 Data](https://rdwinkelman.shinyapps.io/US_COVID_Explorer/)
    - [Exploring the Temporal Evolution of COVID-19 Cases in the US](https://rpubs.com/rdwinkelman/covid19_us_spread_gif)
- [COVID-19 Real Time Tracker for US and Canada](https://coronavirus.1point3acres.com/en) built by first generation Chinese immigrants
- Predictive Healthcare team at University of Pennsylvania's School of Medicine: [COVID-19 Hospital Impact Model for Epidemics](http://penn-chime.phl.io/)
- COVID-19 modeling reports from Imperial College, UK: Report 9: [Impact of non-pharmaceutical interventions (NPIs) to reduce COVID-19 mortality and healthcare demand](https://www.imperial.ac.uk/mrc-global-infectious-disease-analysis/news--wuhan-coronavirus/)
- Screencast by David Robinson on YouTube: [Cleaning and exploring the COVID-19 Open Research Dataset](https://www.youtube.com/watch?v=-5HYdBq_PTM)
    > I (David) show how to open and explore the CORD-19 dataset of scientific publications related to COVID-19 (coronavirus). This includes parsing json files with jsonlite, rectangling the data with tidyr's hoist and unnest_wider, and doing named entity recognition by combining tidytext with the spacyr package and scispacy models.
    - The [CORD data set is housed by Kaggle as part of a research challenge here](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge).
- [Mine Cetinkaya-Rundel's covid19-r repository](https://github.com/mine-cetinkaya-rundel/covid19-r/blob/master/README.md) gathers analyses on and representations of COVID-19 data in R.
    - A post that Mine links to that I found interesting: ["Ten Considerations Before You Create Another Chart About COVID-19"](https://medium.com/nightingale/ten-considerations-before-you-create-another-chart-about-covid-19-27d3bd691be8)
- My friend from graduate school, Alan Salzberg, weighs in with "[It's All About Stopping Exponential Growth](https://salthillstatistics.com/posts/59)".
- Several posters have linked to this [Epidemic Calculator](http://gabgoh.github.io/COVID/index.html) by Gabriel Goh (and others) which lets you play around with various simulations. If you like it, great. I make no claims about its accuracy. I got more from the [NY Times piece from 2020-03-25](https://www.nytimes.com/interactive/2020/03/25/opinion/coronavirus-trump-reopen-america.html) for which Gabriel's work was a key starting point.
- FiveThirtyEight, unsurprisingly, is producing more and more material on the [impact (politically, economically and otherwise) of the novel Coronavirus](https://fivethirtyeight.com/tag/coronavirus/).
- Weichuan Dong, a spatial analyst in PQHS here at CWRU posted this [public Tableau dashboard of US state responses](https://public.tableau.com/profile/weichuan.dong#!/vizhome/USGovernorsResponsesonCoronavirus/GovernorTwitter). He'd be interested in hearing any suggestions you have.
- [This tweet from JD Long on 2020-03-24](https://twitter.com/CMastication/status/1242392769127157761?s=20) highlights a [visualization of the outbreak by @shinyps](https://twitter.com/shinyps1/status/1242324692620345345/photo/1) that I agree does several things well.
- From [Ellie Murray, 2020-03-26](https://twitter.com/EpiEllie/status/1243170268568264704)

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class17/figures/murray_2020-03-26.png)

- [Cleveland Recovers](https://cleveland.recovers.org/): Cleveland Pandemic Response - COVID19 Community Hub
- [How the Pandemic will End](https://www.theatlantic.com/health/archive/2020/03/how-will-coronavirus-end/608719/) by Ed Yong in *The Atlantic*.
- From Frank Harrell: [Resources for COVID-19 Randomized Clinical Trial Design](http://hbiostat.org/proj/covid19/)
- [Trump Wants to "Reopen America." Here’s What Happens if We Do.](https://www.nytimes.com/interactive/2020/03/25/opinion/coronavirus-trump-reopen-america.html) by Nicholas Kristof and Stuart A. Thompson. Model created with Gabriel Goh, Steven De Keninck, Ashleigh Tuite and David N. Fisman, *New York Times* 2020-03-25.

