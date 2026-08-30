# Search SSRC fellowships and grants by keyword and date Note: API limitations prevent returning more than 1000 results.

Search SSRC fellowships and grants by keyword and date Note: API
limitations prevent returning more than 1000 results.

## Usage

``` r
get_ssrc(keyword, from_year, to_year, verbose = FALSE, totals = FALSE)
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

- totals:

  Only return the total number of results, not a table

## Value

a data.frame

## Examples

``` r
if (FALSE) ssrc <- get_ssrc("qualitative", 2015, 2016) # \dontrun{}
```
