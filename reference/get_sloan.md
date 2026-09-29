# Search for a set of keywords in the Sloan grants database.

Search for a set of keywords in the Sloan grants database.

## Usage

``` r
get_sloan(keyword, from_year, to_year, verbose = FALSE, grantee = FALSE)
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

- grantee:

  Use the web-based search function instead of an internal grep(), ideal
  for searching names

## Value

A data.frame

## Examples

``` r

if (FALSE) { # \dontrun{
sloan <- get_sloan("case studies", 2018, 2020)
} # }
```
