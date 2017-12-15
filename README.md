
<!-- Don't edit README.md; instead, please edit README.Rmd -->
bciex: Example data from Barro Colorado Island <img src="https://i.imgur.com/39pvr4n.png" align="right" height=44 />
====================================================================================================================

[![Travis-CI Build Status](https://travis-ci.org/forestgeo/bciex.svg?branch=master)](https://travis-ci.org/forestgeo/bciex) [![Coverage status](https://coveralls.io/repos/github/forestgeo/bciex/badge.svg)](https://coveralls.io/r/forestgeo/bciex?branch=master) [![CRAN status](http://www.r-pkg.org/badges/version/bciex)](https://cran.r-project.org/package=bciex)

Installation
------------

Install **bciex** from github with:

``` r
# install.packages("devtools")
devtools::install_github("forestgeo/bciex")
```

Example
-------

This is a basic example which shows you how to solve a common problem:

``` r
library(bciex)

# Mini dataset of 1000 randomly selected trees from BCI; data realeased in 2012
str(bci12t1mini)
#> 'data.frame':    1000 obs. of  20 variables:
#>  $ treeID   : int  858 1083 1129 2143 2388 3431 4448 5877 6487 7132 ...
#>  $ stemID   : int  1 1 1 1 1 1 1 1 1 1 ...
#>  $ tag      : chr  "000851" "001080" "001127" "002147" ...
#>  $ StemTag  : chr  "" NA "" "" ...
#>  $ sp       : chr  "apeime" "alchco" "quaras" "beilpe" ...
#>  $ quadrat  : chr  "4402" "4314" "4308" "3715" ...
#>  $ gx       : num  899 873 867 744 724 ...
#>  $ gy       : num  42 284 163 305 447 ...
#>  $ MeasureID: int  856 1083 1129 2150 2397 3446 4466 5922 6545 7197 ...
#>  $ CensusID : int  1 1 1 1 1 1 1 1 1 1 ...
#>  $ dbh      : num  598 807 503 181 366 491 233 492 305 184 ...
#>  $ pom      : chr  "1.3" "1.3" "1.3" "1.3" ...
#>  $ hom      : num  1.3 1.3 1.3 1.3 1.3 ...
#>  $ ExactDate: chr  "1981-05-03" "1981-07-01" "1981-05-26" "1981-07-18" ...
#>  $ DFstatus : chr  "alive" "alive" "alive" "alive" ...
#>  $ codes    : chr  NA NA NA NA ...
#>  $ nostems  : num  1 1 1 1 1 1 1 1 1 1 ...
#>  $ date     : num  7793 7852 7816 7869 7884 ...
#>  $ status   : chr  "A" "A" "A" "A" ...
#>  $ agb      : num  2.07 4.204 2.028 0.163 0.838 ...

# The stem data corresponding to the 1000 trees above.
str(bci12s7mini)
#> 'data.frame':    2165 obs. of  20 variables:
#>  $ treeID   : int  858 1083 1083 1083 1083 1083 1083 1083 1083 1083 ...
#>  $ stemID   : int  1 1 2 3 4 5 6 7 8 9 ...
#>  $ tag      : chr  "000851" "001080" "001080" "001080" ...
#>  $ StemTag  : chr  "" NA NA NA ...
#>  $ sp       : chr  "apeime" "alchco" "alchco" "alchco" ...
#>  $ quadrat  : chr  "4402" "4314" "4314" "4314" ...
#>  $ gx       : num  899 873 873 873 873 ...
#>  $ gy       : num  42 284 284 284 284 ...
#>  $ MeasureID: int  766 NA NA NA NA NA NA NA NA NA ...
#>  $ CensusID : int  171 NA NA NA NA NA NA NA NA NA ...
#>  $ dbh      : num  720 NA NA NA NA NA NA NA NA NA ...
#>  $ pom      : chr  "3.6" NA NA NA ...
#>  $ hom      : num  3.5 NA NA NA NA NA NA NA NA NA ...
#>  $ ExactDate: chr  "2010-09-16" NA NA NA ...
#>  $ DFstatus : chr  "alive" "stem_gone" "stem_gone" "stem_gone" ...
#>  $ codes    : chr  "B,cylN" NA NA NA ...
#>  $ countPOM : num  1 NA NA NA NA NA NA NA NA NA ...
#>  $ date     : num  18521 18485 18485 18485 18485 ...
#>  $ status   : chr  "A" "G" "G" "G" ...
#>  $ agb      : num  3.24 NA NA NA NA ...
```
