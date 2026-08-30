# Search the Andrew W. Mellon Foundation grant database

Search the Andrew W. Mellon Foundation grant database

## Usage

``` r
get_mellon(keyword, from_year, to_year, verbose = FALSE)
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
mellon <- get_mellon("qualitative", 2013, 2021)
#> Warning: Not Found (HTTP 404).
#> Error in if (total_grants == 0) {    return(NULL)}: argument is of length zero
```
