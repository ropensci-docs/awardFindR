# Search NIH RePORTER

Search NIH RePORTER

## Usage

``` r
get_nih(keyword, from_date, to_date, verbose = FALSE, payload = NULL)
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

- payload:

  A custom NIH search query object. Only for advanced purposes. default:
  null

## Value

a data.frame

## Examples

``` r
nih <- get_nih("ethnography", "2019-01-01", "2019-05-01")
```
