---
title: "guide to R, Rstudio, Rmarkdown install"
author: "Richard Martin"
date: "21/10/2020"
output:
  html_document:
    keep_md: yes
---



# Assignments:

For this course your assignments will involve the analysis of data that is generated from a series of 6 experiments.  This allows you to gain experience with the models from two different perspectives: from the inside (as subjects in the experiments) and the outside (as a scientist studying the observed behaviour). This document provides links for setting up the various pieces of R software you will require to do the assignments. No programming experience is assumed or required. 

# Installation instructions:

Here is an [installation guide](https://techvidvan.com/tutorials/install-r/) for R and Rstudio for all operating systems.

Once you have installed R and Rstudio, open Rstudio. At the blinking cursor (bottom left of the IDE) type:

    install.packages("tidyverse")

Then hit enter. The `tidyverse` provides the plotting functionality that we require.  Once that is done (it may take a while) at the blinking cursor type:

    install.packages("rmarkdown")

Then hit enter. `Rmarkdown` weaves together your plots created in R with your prose to produce your assignment submission. Once that is done (this should be relatively quick) at the blinking cursor type:

    install.packages('tinytex')

Then hit enter. `Tinytex` allows us to create pdf documents.  Once that is done (this should be relatively quick) at the blinking cursor type:

    tinytex::install_tinytex()
    
Finally, you will be downloading the assignments and the data from GitHub, so you will need to [download](https://git-scm.com/downloads) and install Git.  

# Testing instructions:

Top left corner of Rstudio, click on `File` then `New File` then `R Markdown` and then hit `Ok`.  This should open a `hello world` Rmarkdown file. 

Find the `knit` button (there is an icon of a ball of yarn with a needle sticking out of it) and click it. Rstudio will ask what your Rmarkdown file should be named and where to save it. Once you are done that a new window should open with the knitted html output of your `hello world` Rmarkdown file.

In your Rmd file find the line at the top that says 

    output: html_document
    
and change it to:

    output: pdf_document
    
Click the `knit` button again.  This should create a pdf version of your `hello world` file. If this worked, you are ready to go!

Next up, read the first 4 chapters of https://r4ds.had.co.nz/index.html

