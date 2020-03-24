# 432 Spring 2020 Class 17: 2020-03-26

## Today's Materials

Information on connecting to class and to TA office hours via Zoom was emailed 2020-03-17. For details, [visit this link](https://github.com/THOMASELOVE/2020-432/blob/master/zoom.md). 

PDF of Slides | .Rmd of Slides | Notes during Class | Need Help? 
------------: | :------------------: | :---------------------------: | :------------------------:
[Class 17 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class17/432_2020_slides17.pdf) | [Class 17 RMD](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class17/432_2020_slides17.Rmd) | [Google Doc](https://docs.google.com/document/d/1VpnXK654mVLJKMnbxMyhvLSEaOwyZhO2itaMf1a3N4U/edit?usp=sharing) | Email **431-help at case dot edu** or attend [TA office hours](https://github.com/THOMASELOVE/2020-432/blob/master/calendar.md#ta-office-hours)

- When Zoom finishes its processing, [the link to the Class 17 recording will go here].
- The [Google Doc of Notes During Class](https://docs.google.com/document/d/1VpnXK654mVLJKMnbxMyhvLSEaOwyZhO2itaMf1a3N4U/edit?usp=sharing) is a place for you to communicate with Dr. Love and the rest of us (and for Dr. Love to remind himself of things) during class, especially if you cannot connect to the Zoom Chat. I'll also leave some follow-up there after each class as needed, on things that come up in the chat, etc.

## Announcements

1. There is a Minute Paper after Class 17. Details to come.

2. The Homework 4 Answer Sketch and Grading Rubric will be posted as soon as we have everyone's assignment.

3. Project 1 Grading. Dr. Love will provide an update.

4. We'll start today's session with **Slide 70** from the [Class 16 Slides](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class16/432_2020_slides16.pdf), and then move on to Class 17 materials.

5. We talked about hanging **rootograms** last time as a means of understanding the fit of count outcome models, like Poisson or Negative Binomial regressions. If you want some more information, a key paper is Kleiber C Zeileis A "[Visualizing Count Data Regressions Using Rootograms](https://arxiv.org/pdf/1605.01311)".

6. Alison Hill gave a very interesting talk at the R Studio 2019 conference on [Making Slides for HTML with R Markdown](https://arm.rbind.io/slides/xaringan.html). There's a lot to unpack, but these are impressive tools.

## Improving/Augmenting Your Visualizations

Visualizing data can be extremely difficult. Even *The Economist* has an interesting history in this regard, as Sarah Leo writes in [Mistakes, we've drawn a few](https://medium.economist.com/mistakes-weve-drawn-a-few-8cdd8a42d368?gi=79a4498d7670). 

1. If you want to arrange plots into a grid in a more nuanced way than `gridExtra::grid.arrange()` provides and you don't like `patchwork` for whatever reason, you probably should consider `cowplot`. The [introductory vignette is here](https://cran.r-project.org/web/packages/cowplot/vignettes/introduction.html), and the [`plot_grid` function vignette is here](https://cran.r-project.org/web/packages/cowplot/vignettes/plot_grid.html). The [github site for cowplot is here](https://github.com/wilkelab/cowplot).
2. If you're looking for ways to improve the themes used in your ggplots, or perhaps to use a specific font or color scheme, you might want to look over [these examples in the hrbrthemes package](https://github.com/hrbrmstr/hrbrthemes).
3. Another interesting idea is highlighting specific values / paths within a plot, and the [gghighlight vignette](https://cran.r-project.org/web/packages/gghighlight/vignettes/gghighlight.html) may be of some interest. This was presented at the R Studio Conference 2019: [more details are here](https://yutani.rbind.io/post/2018-06-03-anatomy-of-gghighlight/).
4. Tables are a kind of visualization, too, of course, and [the gt package](https://github.com/rstudio/gt) can be a big help in trying to build information-dense and attractive tables.

Of course, if you really do a good job, it's always possible you'll be rewarded [with a parade](https://twitter.com/DapperHistorian/status/1111007778469040133)!

![](https://github.com/THOMASELOVE/2020-432/blob/master/classes/class17/figures/parade.png)