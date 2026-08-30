# Query and scrape Open Society foundation awards

Query and scrape Open Society foundation awards

## Usage

``` r
get_osociety(keyword, from_year, to_year, verbose = FALSE)
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
osociety <- get_osociety("qualitative", 2016, 2019)
#> Warning: Forbidden (HTTP 403).
```
