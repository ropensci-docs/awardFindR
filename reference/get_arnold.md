# Get Arnold Foundations/Arnold Venture awards

Get Arnold Foundations/Arnold Venture awards

## Usage

``` r
get_arnold(keyword, from_year, to_year, verbose = FALSE)
```

## Arguments

- keyword:

  Keyword to query

- from_year:

  Beginning year to search

- to_year:

  Ending year to search

- verbose:

  enable verbose HTTP messages. TRUE/FALSE, default: false

## Value

a data.frame

## Examples

``` r
arnold <- get_arnold("qualitative", 2016, 2017)
```
