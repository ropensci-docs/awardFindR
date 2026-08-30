# Search for a set of keywords in the Templeton grants database.

Search for a set of keywords in the Templeton grants database.

## Usage

``` r
get_templeton(keywords, from_year, to_year, verbose = FALSE)
```

## Arguments

- keywords:

  Vector of strings to search

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
if (FALSE) { # \dontrun{
templeton <- get_templeton(c("qualitative data", "case studies"), 2018, 2020)
} # }
```
