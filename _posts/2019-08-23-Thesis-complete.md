---
layout: post
title:  "My ms thesis is finally complete!"
image: /assets/img/blog2.jpg
---

# What a journey!

After 6 months of hard work, yesterday I've finally managed to send the complete version of my ms thesis to be reviewed from my thesis supervisor. It's my first "serious" work entirely made with [Rmarkdown](https://rmarkdown.rstudio.com/). I wanted to share what resources I used to make this entire work possible and how I managed to get all the things working appropriately. Enjoy!

# Why Rmarkdown?

If you already know R and R Markdown, you can skip to the next [section](#requirements).
When I started sorting things out for my thesis, I didn't know anything about LaTeX. I knew in advance I would have used R as my first choice programming language for all the thesis work and I wanted to minimize the struggle I've always encountered while working with Microsoft Word ("WHY CAN'T THIS PICTURE STAY EXACTLY HERE?!" [cit. Me, 2015]). I won't explain how all the magic works, there are already a ton of guides and documentation about it. I'm going to explain how and why Rmarkdown was the perfect solution which suited best for me:

1. Rmarkdown is a tool from R Studio which is used to write high quality documents of any kind (reports, presentations and even [dashboards](https://rmarkdown.rstudio.com/flexdashboard/)).
3. While writing my ms thesis, I needed to write some equations (we engineers love equations). Using Rmarkdown, I could write the equations I needed, using some LaTeX basics and the results were simply amazing:

![latex equations and resulting printed equations](/assets/img/eq.png)

2. An .rmd file is a plain text document in which one can insert *code chunks* of different programming language (Python, R) in order to make...anything you could do with some code. In my thesis, I've used some R code chunks in order to build plots and tables (as in the picture below). The orange box represents the plain text of the thesis. The code chunk, in the green box, is where I put all the R code needed to create the bar plot. No need to build the plot on a new R script and exporting the resulting image in a file: **everything I need is already in the chapter file, ready to be modified if needed**.

![R code chunk and the resulting plot. Rmarkdown FTW!]( /assets/img/sdd.png)

# Requirements

This is the list of the tools I've used while writing my thesis:

1. [Atom](https://flight-manual.atom.io/getting-started/sections/why-atom/): a versatile, powerful and highly
customizable (thanks to the many addons available) text editor which I used to organize and write all the chapters for my thesis. Atom also comes with Git and Github integrations which made it really easy to manage all the files of my thesis repository.

2. Rstudio and Rmarkdown, of course. I've used Rmarkdown to write the main.rmd file which is the master file where I've set all the instructions to build the different parts of the thesis.

3. [Zotero](https://www.zotero.org/): a free and simple tool which I used to organize all the documents and papers that I wanted to cite. Using Atom, I've also installed the package called [Zotero-picker](https://atom.io/packages/zotero-picker) which is really great to invoke Zotero and add citations keys.
