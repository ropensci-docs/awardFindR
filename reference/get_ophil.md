# Grab the Open Philanthropy grants data search for keyword-date combos

Grab the Open Philanthropy grants data search for keyword-date combos

## Usage

``` r
get_ophil(keyword, from_year, to_year, verbose = FALSE)
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

A data.frame

## Examples

``` r
ophil <- get_ophil("qualitative", 2019, 2020)
#> Warning: Forbidden (HTTP 403).
```
