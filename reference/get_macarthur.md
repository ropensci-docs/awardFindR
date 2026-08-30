# Search MacArthur foundation for awards

Search MacArthur foundation for awards

## Usage

``` r
get_macarthur(keyword, from_year, to_year, verbose = FALSE)
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
macarthur <- get_macarthur("qualitative",
"1999-01-01", "2020-01-01")
} # }
```
