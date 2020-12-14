
# qData <img src="inst/qData_hexlogo.png" align="right" width="200"/>

<!-- badges: start -->

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
![GitHub release (latest by
date)](https://img.shields.io/github/v/release/globalgov/qData) ![GitHub
Release
Date](https://img.shields.io/github/release-date/globalgov/qData)
![GitHub
issues](https://img.shields.io/github/issues-raw/globalgov/qData)
<!-- [![HitCount](http://hits.dwyl.com/globalgov/qData.svg)](http://hits.dwyl.com/globalgov/qData) -->
[![Codecov test
coverage](https://codecov.io/gh/globalgov/qData/branch/main/graph/badge.svg)](https://codecov.io/gh/globalgov/qData?branch=main)
<!-- ![GitHub All Releases](https://img.shields.io/github/downloads/jhollway/roctopus/total) -->
<!-- badges: end -->

`{qData}` is the central package in an ecosystem of packages aimed at
collecting, connecting and correcting network data across issue-domains
of global governance. It is a package both for users of this data as
well as for data owners and developers.

## Why qData?

For users, `{qData}` offers a way to access all of the tested data in
the ecosystem in so-called ‘qPackages’, and use this data in their
analyses of global governance. A special advantage of such qdata is that
it is not ‘opinionated’, in the sense of offering a single, supposedly
authoritative version of global governance events, but instead holds
many well-regarded datasets together in three-dimensional ‘datacubes’.
The chief advantage of this for global governance researchers is that it
enables a quick and easy way to check the robustness of their results to
different formulations of the study population or concept specification.
For more, please see the vignette.

For developers, `{qData}` provides the necessary tools to put their data
in the hands of users. The package includes many functions to make this
easier. It includes functions to help set up a qPackage, import their
existing data, and export them in structures consistent with the rest of
the data ecosystem. This facilitates the interoperability, contrast, and
comparison of data. For more, please see the vignette.

## Downloading and installing qData

The development version of the package `{qData}` can be downloaded from
GitHub.

    #install.package(remotes)
    remotes::install_github("globalgov/qData")

## Available qPackages

`{qData}` connects users to other packages that help fill global
governance researchers’ data needs. The `get_packages()` function can be
used to discover which packages are currently available.

``` r
 library(qData)
```

    ## Loading required package: tibble

``` r
 get_packages()
```

    ## # A tibble: 1 x 7
    ##   name  full_name     description latest updated_at       stargazers open_issues
    ##   <chr> <chr>         <chr>       <chr>  <chr>                 <int>       <int>
    ## 1 qData globalgov/qD… <NA>        v0.2.1 2020-12-04T13:2…          2          16

Please see [the website](https://globalgov.github.io/qData/) for more
information about how to use `{qData}` for both developers and users.
