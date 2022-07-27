
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ussie

<!-- badges: start -->

[![R-CMD-check](https://github.com/NatalieWeaver/ussie/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/NatalieWeaver/ussie/actions/workflows/R-CMD-check.yaml)
[![test-coverage](https://github.com/NatalieWeaver/ussie/actions/workflows/test-coverage.yaml/badge.svg)](https://github.com/NatalieWeaver/ussie/actions/workflows/test-coverage.yaml)
<!-- badges: end -->

## Introduction

All of the students in the “Building Tidy Tools” workshop at
rstudio::conf(2022) built `ussie` to learn package development. A huge
thanks to Emma Rand and Ian Lyttle for being fantastic teachers.

Course materials:

-   [Course
    website](https://rstudio-conf-2022.github.io/build-tidy-tools/)
-   [“BT2T” course package](https://github.com/rstudio-conf-2022/btt22)
-   [ussie example from
    instructors](https://github.com/rstudio-conf-2022/ussie)

The goal of `ussie` is to help you work with European soccer league data
supplied by the `engsoccerdata` package. The name “ussie” is a reference
to the Apple tv show “Ted Lasso”.

## Installation

You can install the development version of ussie from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("NatalieWeaver/ussie")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(ussie)
# get the England league data in standard format
uss_make_matches(engsoccerdata::england, "England")
#> # A tibble: 192,004 x 8
#>    country tier  season date       home            visitor       goals~1 goals~2
#>    <chr>   <fct>  <int> <date>     <chr>           <chr>           <int>   <int>
#>  1 England 1       1888 1888-12-15 Accrington F.C. Aston Villa         1       1
#>  2 England 1       1888 1889-01-19 Accrington F.C. Blackburn Ro~       0       2
#>  3 England 1       1888 1889-03-23 Accrington F.C. Bolton Wande~       2       3
#>  4 England 1       1888 1888-12-01 Accrington F.C. Burnley             5       1
#>  5 England 1       1888 1888-10-13 Accrington F.C. Derby County        6       2
#>  6 England 1       1888 1888-12-29 Accrington F.C. Everton             3       1
#>  7 England 1       1888 1889-01-26 Accrington F.C. Notts County        1       2
#>  8 England 1       1888 1888-10-20 Accrington F.C. Preston Nort~       0       0
#>  9 England 1       1888 1889-04-20 Accrington F.C. Stoke City          2       0
#> 10 England 1       1888 1888-11-24 Accrington F.C. West Bromwic~       2       1
#> # ... with 191,994 more rows, and abbreviated variable names 1: goals_home,
#> #   2: goals_visitor
#> # i Use `print(n = ...)` to see more rows
```
