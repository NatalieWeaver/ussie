
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ussie

<!-- badges: start -->

[![R-CMD-check](https://github.com/NatalieWeaver/ussie/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/NatalieWeaver/ussie/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of ussie is to help you work with European soccer league data
supplied by the `engsoccerdata` package.

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
#>    country tier  season date       home         visitor goals_home goals_visitor
#>    <chr>   <fct>  <int> <date>     <chr>        <chr>        <int>         <int>
#>  1 England 1       1888 1888-12-15 Accrington ~ Aston ~          1             1
#>  2 England 1       1888 1889-01-19 Accrington ~ Blackb~          0             2
#>  3 England 1       1888 1889-03-23 Accrington ~ Bolton~          2             3
#>  4 England 1       1888 1888-12-01 Accrington ~ Burnley          5             1
#>  5 England 1       1888 1888-10-13 Accrington ~ Derby ~          6             2
#>  6 England 1       1888 1888-12-29 Accrington ~ Everton          3             1
#>  7 England 1       1888 1889-01-26 Accrington ~ Notts ~          1             2
#>  8 England 1       1888 1888-10-20 Accrington ~ Presto~          0             0
#>  9 England 1       1888 1889-04-20 Accrington ~ Stoke ~          2             0
#> 10 England 1       1888 1888-11-24 Accrington ~ West B~          2             1
#> # ... with 191,994 more rows
```
