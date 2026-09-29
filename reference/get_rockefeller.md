# Search Rockefeller Foundation grants

Search Rockefeller Foundation grants

## Usage

``` r
get_rockefeller(keyword, from_date, to_date, verbose)
```

## Arguments

- keyword:

  Keyword to query

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
rockefeller <- get_rockefeller("test", "2012-01-01", "2021-01-01")
} # }
```
