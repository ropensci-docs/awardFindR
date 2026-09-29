# Search the NSF API for awards

Search the NSF API for awards

## Usage

``` r
get_nsf(keyword, from_date, to_date, verbose = FALSE, cfda = NULL)
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

- cfda:

  Comma-separated CFDA codes to include, default: all

## Value

A data.frame

## Examples

``` r
nsf <- get_nsf("ethnography", "2020-01-01", "2020-02-01")
```
