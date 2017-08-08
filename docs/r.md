# R and RStudio

R is a language for statistical computing and graphics.
It's use in the data science and econometrics community has taken off over recent years and (at a bare minimum) should be considered as an open source replacement to Stata.

## Installing R

Go to the [R homepage](https://cran.r-project.org/) and download the installer for your operating system.

The current version of R is 3.4

## Installing RStudio

RStudio provides an easy to work with interface to R, and its format should feel familiar to Stata and Matlab users.

Download and install RStudio for your operating system from [here](https://www.rstudio.com/products/rstudio/download3/).

## Installing Additional R Packages

We will need some additional libraries to conduct our statistical analysis. Proceed as follows:

* Open RStudio
* In the **console**, copy and paste the following:
```r
uzh_progecon <- c("tidyverse",  "reshape",
                    "plm", "Hmisc", "sandwich",
                    "Ecdat", "stargazer", "knitr",
                    "xtable")

install.packages(uzh_progecon)
```
* Wait until all the packages have been installed and the you are done.
    * It *may* take a while, so be patient

## Command Line R for Windows Users

If you want R available from the command line (it is by default for Mac and Linux), we again need to update our PATH settings.

Right-click on Computer. Then go to "Properties" and select the tab "Advanced System settings". Choose "Environment Variables" and select "Path" from the list of system variables.

Choose “Edit” and append (i.e., do not overwrite the previous value):

        ;C:\Path\to\program.exe

to the variable value – make sure the rest remains as it is and do not include spaces between the ";" and the text.

Click on OK as often as needed.

If you accepted all defaults during your installation, and didn't have any other non-default setting prior to starting this guide, modifying the following string, with your relevant username *should* work:

        ;C:\Program Files\R\R-3.4.1\bin

Close your current terminal session, open a new one, and try
```bash
R --version`
```
followed by pressing `Return`.

The expected output begins with
```bash
R version 3.3.2 (2016-10-31) -- "Sincere Pumpkin Patch"
Copyright (C) 2016 The R Foundation for Statistical Computing
```
