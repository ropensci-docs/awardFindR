# Search Carnegie awards

Search Carnegie awards

## Usage

``` r
get_carnegie(keyword, from_year, to_year, verbose = FALSE)
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
if (FALSE) { # \dontrun{
carnegie <- get_carnegie("qualitative data", 2016, 2017)
} # }
```
