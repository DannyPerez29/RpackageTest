
<!-- README.md is generated from README.Rmd. Please edit that file -->

\*\*NOTE: This is a toy package to practice the methods for creation of
R packages for personal use.

# RpackageTest

<!-- badges: start -->
<!-- badges: end -->

The goal of RpackageTest is to …

## Installation

You can install the development version of RpackageTest from
[GitHub](https://github.com/) with:

``` r
# install.packages("pak")
pak::pak("DannyPerez29/RpackageTest")
```

## Usage

This package contains only one function to split character vectors into
its parts based on a separator.

## Example

This is a basic example which shows you how to solve a common problem:

``` r
(x <- "alfa,bravo,charlie,delta")
#> [1] "alfa,bravo,charlie,delta"
strsplit(x, split = ",")
#> [[1]]
#> [1] "alfa"    "bravo"   "charlie" "delta"
stringr::str_split(x, pattern = ",")
#> [[1]]
#> [1] "alfa"    "bravo"   "charlie" "delta"
```

This outputs a list with all the segments.

``` r
library(RpackageTest)

str_split_one(x, pattern = ",")
#> [1] "alfa"    "bravo"   "charlie" "delta"
```
