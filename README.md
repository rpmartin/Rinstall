---
title: "guide to R, Rstudio, Rmarkdown install"
author: "Richard Martin"
output:
  html_document:
    keep_md: yes
---

# Assignments:

For this course your assignments will involve the analysis of data that is generated from a series of 6 experiments.  This allows you to gain experience with the models from two different perspectives: from the inside (as subjects in the experiments) and the outside (as a scientist studying the observed behaviour). This document provides links for setting up the software you will require to do the assignments. No programming experience is assumed or required. 

# Installation instructions:

![](threepaths.jpeg)

## The easy way: slow and expensive.

* Go to [rstudio cloud](https://rstudio.cloud/)
* Click on get started for free (up to 15 hours/month)
* Click signup... and sign up.
* Click new project... new project.
* At the prompt > type `install.packages("tidyverse")` and hit enter.
* At the prompt > type `library("tidyverse")` and hit enter.
* If no error messages, you are ready for testing (instructions below).

## The hard way: fast and free.

**All software should be installed on your local hard drive, not on a network/cloud drive.**

1) Follow instructions [here](https://techvidvan.com/tutorials/install-r/#install-r-windows) to install R and Rstudio.

2) An annoying "feature" of windows10+Rstudio is that the default is to install packages on the cloud.  Here is how to fix this [Problem.](https://medium.com/@ValidScience/how-to-fix-rstudios-package-installation-on-windows-10-c1e602bf3a1f)

3) open Rstudio. At the prompt > (bottom left of the IDE) type:

    `install.packages("tidyverse")` then hit enter.  

    `install.packages("rmarkdown")` then hit enter.
    
    `install.packages("tinytex")` then hit enter.
    
    `tinytex::install_tinytex()` then hit enter.

* If no error messages, you are ready for testing.If you were not able to get the above libraries installed you will need to take the easy path: Rstudio cloud (instructions above.) 

# Testing instructions:

Top left corner of Rstudio, click on `File` then `New File` then `R Markdown` and then hit `Ok`. If you get a message like "Creating Rmarkdown documents requires...", choose yes. It will ask you for a title and an output format: choose pdf.  A `hello world` Rmarkdown file should open. 

Find the `knit` button (there is an icon of a ball of yarn with a needle sticking out of it) and click it. Rstudio will ask for a file name and where to save it. Once you are done that a new window should open with the knitted pdf output of your `hello world` Rmarkdown file.


## Git er done.

Assignments will be made available on Github.  If you took the easy path (Rstudio cloud) you should be able to clone the assignment.  If you took the hard path (local install), cloning the assignment is marginally easier but requires you to install [Git](https://git-scm.com/downloads) on your computer.  If you have *any* difficulties with the install of Git, don't bother.  The other option is to download the assignments as zip files and manually unzip them, which does not require an install of Git.

 

