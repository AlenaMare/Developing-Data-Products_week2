---
title: "City of Hundred Spires_"
author: "AM"
date: "8 12 2022"
output: md_document
---

```{r setup, include=TRUE}
knitr::opts_chunk$set(echo = TRUE)
```

## Summary

The goal of the project is to create a web page using R Markdown that features a map created with Leaflet, and to host the resulting web page on either GitHub Pages, RPubs, or NeoCities.


## R Markdown
```{r, echo=TRUE}
library(leaflet)
my_map <- leaflet() %>%
  addTiles() %>%
addMarkers(lat=50.073658, lng=14.418540, popup = "Prague")

my_map
```