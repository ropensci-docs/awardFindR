# Get Robert Wood Johnson foundation awards

Get Robert Wood Johnson foundation awards

## Usage

``` r
get_rwjf(keyword, from_year, to_year, verbose = FALSE)
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
rwjf <- get_rwjf("qualitative data analysis", 2014, 2014)
#> Warning: Internal Server Error (HTTP 500).
```
