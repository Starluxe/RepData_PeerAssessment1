---
title: "Reproducible Research: Peer Assessment 1"
output: 
  html_document:
    keep_md: true
---


## Loading and preprocessing the data

```r
rm(list = ls())
listfiles <- dir()
if ("activity.csf" %in% listfiles){
    actdf <- read.csv("activity.csv")
}else{
    if ("activity.zip" %in% listfiles){
        unzip(zipfile = "activity.zip")
        actdf <- read.csv("activity.csv") 
    }else{
        print("No files found!!!")
    }
}
```


## What is mean total number of steps taken per day?



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
