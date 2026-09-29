# awardFindR

`search_awards` is meant to be the top-level function for interacting
with grant database search functions.

## Load awardFindR

``` r

library(awardFindR)
```

## Simple keyword search, single source

``` r

nsf <- search_awards(keywords="illicit", sources="nsf", from_date="2023-01-01")
str(nsf)
#> 'data.frame':    36 obs. of  12 variables:
#>  $ institution: chr  "University of Notre Dame" "Dartmouth College" "The University of Central Florida Board of Trustees" "Barnard College" ...
#>  $ pi         : chr  "Nichols, Lisa" "Zhang, Xiaojing" "Yao, Fan" "Moncada, Eduardo" ...
#>  $ year       : chr  "2026" "2023" "2024" "2024" ...
#>  $ start      : chr  "2026-07-15" "2023-09-01" "2024-03-01" "2025-01-01" ...
#>  $ end        : chr  "2029-06-30" "2027-08-31" "2029-02-28" "2027-12-31" ...
#>  $ program    : chr  "47.070, 47.083" "47.041" "47.070" "47.075" ...
#>  $ amount     : chr  "1200000" "399541" "556875" "230928" ...
#>  $ id         : chr  "2613803" "2318814" "2340777" "2416429" ...
#>  $ title      : chr  "CICI:TCR: Demonstrating NSPM-33 Cybersecurity Critical Controls Transition at Research Institutions Through Acc"| __truncated__ "Label-free Detection of Opioids in Liquid Using Zinc Oxide Nanophotonic Sensor" "CAREER: Understanding and Ensuring Secure-by-design Microarchitecture in Modern Era of Computing" "RUI: Criminal Competition and Collective Political Mobilization in Comparative Perspective" ...
#>  $ abstract   : chr  "Foreign adversaries continue campaigns to seek scientific and technological advantage through both legitimate a"| __truncated__ "Illicit drug abuse has become another major national health crisis since the Covid-19\r\npandemic started, due "| __truncated__ "Microarchitectural attacks (i.e., side and covert channels) have opened a new chapter in computer system securi"| __truncated__ "Millions of people across the developing world live and work in marginalized urban spaces with limited access t"| __truncated__ ...
#>  $ keyword    : chr  "illicit" "illicit" "illicit" "illicit" ...
#>  $ source     : chr  "NSF" "NSF" "NSF" "NSF" ...
```

## Multiple sources and keywords, specific date range

``` r

nsf_and_nih <- search_awards(keywords=c("ontological", "audio recordings"), sources=c("nsf", "nih"), from_date="2018-01-01", to_date="2018-09-01")
table(nsf_and_nih$source)
#> 
#> NIH NSF 
#>  21  11
unique(nsf_and_nih$keyword)
#> [1] "ontological"      "audio recordings"
```

For more than a few keywords, you can specify an external simple csv
file. If you specify a .csv file path for `keywords`, the file should be
a list of keywords, one string per line. For example:

    qualitative data
    qualitative analysis
    case study
    case studies
