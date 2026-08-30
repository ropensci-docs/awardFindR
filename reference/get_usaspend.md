# Search the USAspending database

Search the USAspending database

## Usage

``` r
get_usaspend(keywords, from_date, to_date, verbose)
```

## Arguments

- keywords:

  Vector of strings to search

- from_date:

  Date object to begin search

- to_date:

  Date object to end search

- verbose:

  enable verbose HTTP messages. TRUE/FALSE, default: false

## Value

a data.frame

## Examples

``` r
if (FALSE) { # \dontrun{
results <- usaspend_get(c("qualitative", "interview"),
 "2019-01-01", "2020-01-01")
} # }
```
