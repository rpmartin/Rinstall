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

There are two paths here:  

1) the easy way.

2) the hard way. 

## The easy way:

* Go to [rstudio cloud](https://rstudio.cloud/)
* Click on get started for free.
* 15 hours/month free, but you can create multiple accounts if you have multiple email addresses. 
* Click signup... and sign up.
* Click new project... new project.
* At the prompt > type `install.packages("tidyverse")` and hit enter.
* At the prompt > type `library("tidyverse")` and hit enter.
* You should get a message that looks like this:

` ── Attaching packages ──────────────────────────────────────────────────────────────────────── tidyverse 1.3.0 ──
✓ ggplot2 3.3.3     ✓ purrr   0.3.4
✓ tibble  3.0.5     ✓ dplyr   1.0.3
✓ tidyr   1.1.2     ✓ stringr 1.4.0
✓ readr   1.4.0     ✓ forcats 0.5.0
── Conflicts ─────────────────────────────────────────────────────────────────────────── tidyverse_conflicts() ──
x dplyr::filter() masks stats::filter()
x dplyr::lag()    masks stats::lag() `

### Testing instructions:

Top left corner of Rstudio, click on `File` then `New File` then `R Markdown` and then hit `Ok`. If you get a message saying you need to install packages, choose yes. It will ask you what sort of output you want: choose pdf.  A `hello world` Rmarkdown file should open. 

Find the `knit` button (there is an icon of a ball of yarn with a needle sticking out of it) and click it. Rstudio will ask what your Rmarkdown file should be named and where to save it. Once you are done that a new window should open with the knitted pdf output of your `hello world` Rmarkdown file.

## The hard way:

Follow the [installation guide](https://techvidvan.com/tutorials/install-r/) for R and Rstudio for all operating systems.  **Note that software should be installed on your local hard drive, not on a network/cloud drive.** 

Once you have installed R and Rstudio, open Rstudio. At the prompt > (bottom left of the IDE) type:

    install.packages("tidyverse")

Then hit enter.  **packages are software, and software should be installed on your local hard drive, not on a network/cloud drive.** Here is a link to fix the problem on  [Windows10](https://medium.com/@ValidScience/how-to-fix-rstudios-package-installation-on-windows-10-c1e602bf3a1f)

The `tidyverse` provides the plotting functionality that we require.

Once that is done (it may take a while) at the blinking cursor type:

    install.packages("rmarkdown")

Then hit enter. `Rmarkdown` weaves together your plots created in R with your prose to produce your assignment submission. Once that is done (this should be relatively quick) at the blinking cursor type:

    install.packages('tinytex')

Then hit enter. `Tinytex` allows us to create pdf documents.  Once that is done (this should be relatively quick) at the blinking cursor type:

    tinytex::install_tinytex()
    
Assignments will be made available on Github.  Cloning the assignment is marginally easier but requires you to install [Git](https://git-scm.com/downloads) on your computer.  If you have *any* difficulties with the install of Git, don't bother.  The other option is to download the assignments as zip files and manually unzip them, which does not require an install of Git.

 

