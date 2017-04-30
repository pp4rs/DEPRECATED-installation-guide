# R and RStudio

R is a language for statistical computing and graphics.
It's use in the data science and econometrics community has taken off over recent years and (at a bare minimum) should be considered as a replacement software to Stata.

## Installing R

Go to the [R homepage](https://cran.r-project.org/) and download the installer for your operating system.

The current version of R is 3.3.1 -- "Bug in Your Hair."

## Installing RStudio

RStudio provides an easy to work with interface to R, and its format should feel familiar to Stata and Matlab users.

Download and install RStudio for your operating system from [here](https://www.rstudio.com/products/rstudio/download3/).

## Installing Additional R Packages

We will need some additional libraries to conduct our statistical analysis. Proceed as follows:

* Open RStudio
* In the console, copy and paste the following:

        uzh_progecon = c("ggplot2", "tibble", "dplyr",
                      "tidyr", "stringr", "reshape",
                          "purrr", "plm", "Hmisc", "sandwich",
                          "Ecdat", "stargazer", "knitr",
                          "xtable")

        install.packages(uzh_progecon)

* Wait until all the packages have been installed and the you are done.
