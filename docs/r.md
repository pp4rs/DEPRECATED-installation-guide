# R and RStudio

R is a language for statistical computing and graphics.
R's use in the data science and econometrics community has taken off over recent years and (at a bare minimum) should be considered as an open source replacement to Stata.

## Installing R

Go to the [R homepage](https://cran.r-project.org/) and download the installer for your operating system.

The current version of R is 3.4

## Installing RStudio

RStudio provides an easy to work with interface to R, and its format should feel familiar to Stata and Matlab users.

Download and install the free version of RStudio for your operating system from [here](https://www.rstudio.com/products/rstudio/download3/).

## Verifying your Install of R

Open a terminal and enter:

```bash
R --version
```

followed by pressing `Return`.

The current version for Mac and Windows is `R version 3.5.1` and for Linux it is `R version 3.4.1` output begins with:

!!! danger " Windows PATH Setting redux"
    If you want R available from the command line (it is by default for Mac and Linux), we again need to update our PATH settings.

    Right-click on Computer. Then go to "Properties" and select the tab "Advanced System settings". Choose "Environment Variables" and select `Path` from the list of system variables.

    Choose `Edit`.

    **Windows 7 and 8 machines:**
    If you accepted all defaults during your installation, and didn't have any other non-default setting prior to starting this guide, copy and paste the following string without spaces at the start or end:

            ;C:\Program Files\R\R-3.4.1\bin

    **Windows 10 machines:**
    Click `New` and paste the following string:

            C:\Program Files\R\R-3.4.1\bin

    Click on `OK` as often as needed.

    After you have done this, open a **new** terminal and try and verify your install.

## Installing Additional R Packages

We will need some additional libraries to conduct our statistical analysis. Proceed as follows:

*   Open RStudio
*   In the **console**, copy and paste the following:
```r
uzh_progecon <- c(  "reshape", "rmarkdown",
                    "plm", "Hmisc", "sandwich",
                    "Ecdat", "stargazer", "knitr",
                    "httr", "rvest", "xml2",
                    "xtable","tidyverse", "AER",
                    "rdd", "car", "aod", "lmtest",
                    "lfe", "nlme", "lme4",
                    "erer", "margins",
                    "multiwayvcov", "RSQLite", "dbplyr")

install.packages(uzh_progecon)
```

* If you are asked if you want to install packages that need compilation, type `y` followed by `Return` to confirm this.
*   Wait until all the packages have been installed and the you are done.
    *   It *may* take a while, so be patient
