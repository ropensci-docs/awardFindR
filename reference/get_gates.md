# Query awards from the Bill & Melinda Gates Foundation

Query awards from the Bill & Melinda Gates Foundation

## Usage

``` r
get_gates(keyword, from_year, to_year, verbose = FALSE)
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
gates <- get_gates("qualitative", 2018, 2020)
```
