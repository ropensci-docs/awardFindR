# awardFindR grant search

Query a collection of online grant databases for awards. These queries
can be limited by keyword, source and date terms.

## Usage

``` r
search_awards(
  keywords,
  sources = c("arnold", "carnegie", "gates", "macarthur", "mellon", "nih", "nsf",
    "ophil", "osociety", "rockefeller", "rsf", "rwjf", "sloan", "ssrc", "templeton",
    "usaspend"),
  from_date = "2019-01-01",
  to_date = Sys.Date(),
  verbose = FALSE
)
```

## Arguments

- keywords:

  Path to keywords csv file (1 term per line) or vector.

- sources:

  A vector of sources to pull from. Default: all

- from_date:

  A date object to limit the search, defaults to Jan 1 2019

- to_date:

  A date object to limit the search, defaults to today

- verbose:

  enable verbose HTTP messages. TRUE/FALSE, default: false

## Value

a data.frame

## Examples

``` r
# Results for "ethnography" from NSF between 1/1 and 2/1 2020
if (FALSE) awards <- search_awards("ethnography", "nsf",
"2020-01-01", "2020-02-01") # \dontrun{}

# More intensive queries
if (FALSE) { # \dontrun{
# Specific keywords, all sources:
specific <- search_awards(keywords=c("ethnography", "case studies"))

# Specific keyword, all sources, specific date range:
five_years <- search_awards(keywords="qualitative",
from_date="2015-01-01", to_date="2020-01-01")
} # }
```
