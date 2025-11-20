myprojectfile
================
Aaron Castro
2025-11-20

``` r
# Source - https://stackoverflow.com/a
# Posted by enes dilber
# Retrieved 2025-11-20, License - CC BY-SA 4.0

#install.packages("devtools") # I guess you also need this
#devtools::install_github("ropensci/rnaturalearthhires")
#library("rnaturalearth")

##install.packages("tidytuesdayR")
##install.packages("devtools")
library(tidytuesdayR)
```

    ## Warning: package 'tidytuesdayR' was built under R version 4.5.2

``` r
library(sf)
```

    ## Linking to GEOS 3.13.1, GDAL 3.11.0, PROJ 9.6.0; sf_use_s2() is TRUE

``` r
library(tidyverse)
```

    ## ── Attaching core tidyverse packages ──────────────────────── tidyverse 2.0.0 ──
    ## ✔ dplyr     1.1.4     ✔ readr     2.1.5
    ## ✔ forcats   1.0.0     ✔ stringr   1.5.1
    ## ✔ ggplot2   3.5.2     ✔ tibble    3.3.0
    ## ✔ lubridate 1.9.4     ✔ tidyr     1.3.1
    ## ✔ purrr     1.1.0

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()
    ## ℹ Use the conflicted package (<http://conflicted.r-lib.org/>) to force all conflicts to become errors

``` r
library(dplyr)
library(tmap)
library(rnaturalearth)
```

    ## Warning: package 'rnaturalearth' was built under R version 4.5.2

``` r
library(rnaturalearthhires)
```

    ## ---- Compiling #TidyTuesday Information for 2025-08-19 ----
    ## --- There is 1 file available ---
    ## 
    ## 
    ## ── Downloading files ───────────────────────────────────────────────────────────
    ## 
    ##   1 of 1: "scottish_munros.csv"

    ## Reading 'ne_10m_lakes.zip' from naturalearth...
    ## Reading 'ne_10m_rivers_lake_centerlines.zip' from naturalearth...
    ## Spherical geometry (s2) switched off
    ## 
    ## although coordinates are longitude/latitude, st_intersects assumes that they
    ## are planar
    ## 
    ## although coordinates are longitude/latitude, st_intersects assumes that they
    ## are planar

![](getting_started_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

library(tidyverse) library(sf) library(knitr) library(kableExtra)

    ##   DoBIH_number     Name Height_m Height_ft X1891 X1921 X1933 X1953 X1969 X1974
    ## 1         1301 Ben More      966      3169 Munro Munro Munro Munro Munro Munro
    ##   X1981 X1984 X1990 X1997 X2021 Comments nearest_neighbor_dist_m         X
    ## 1 Munro Munro Munro Munro Munro     <NA>                53710.69 -6.014045
    ##          Y
    ## 1 56.42485

    ##       Name Height_m nearest_neighbor_dist_m         X        Y
    ## 1 Ben More      966                53710.69 -6.014045 56.42485

![](getting_started_files/figure-gfm/unnamed-chunk-5-1.png)<!-- -->
