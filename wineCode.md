---
title: "Wine Analysis Task"
author: "DGC"
date: "2023-03-06"
output: 
  html_document: 
    keep_md: yes
    theme: cerulean
    toc: true
    number_sections: true
---



Connect RStudio to Git client and initialize libraries


```r
#install.packages("usethis")
library(usethis)
library(magrittr)
library(highcharter)
library(explore)
library(dplyr)
library(DataExplorer)
library(skimr)
library(readr)
# usethis::create_from_github(
#  "https://github.com/dezzygc/WineData.git", destdir = "C:/Users/dezzy/Documents/happygit/wine_repo")
```
Import dataset


```r
wine_df <- read_csv("red_wine_data.csv")
as_tibble(wine_df)
```

Generate exploratory html reports


```r
 #wine_df %>% explore()
# wine_df %>% report(output_file = "report.html", output_dir = getwd())
```


#readthedown Theme (from rmdformats Package)




