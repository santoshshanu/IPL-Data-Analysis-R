# IPL-Data-Analysis-R

Introduction:

Sports analytics is one of the metrics used in various games worldwide. It not only enhances game prediction but also aids in analyzing team and individual player performances. This analysis focuses on cricket, specifically the Indian Premier League (IPL), aiming to understand team strategies, player contributions, and overall game dynamics.

Overview:
This project utilizes R programming to conduct data analysis on IPL matches. The data sources include overview.csv, matches.csv, deliveries.csv, and deliveries2.csv. Below are the libraries used in this analysis:

library(flexdashboard)
library(tidyverse)
library(gapminder)
library(ggplot2)
library(knitr)
library(skimr)
library(dplyr)
library(flextable)
library(plotly)

Data Preparation:

overview <- read.csv("overview.csv", na.strings=c("","NA"))
matches <- read.csv("matches.csv", na.strings=c("","NA"))
deliveries <- read.csv("deliveries.csv", na.strings=c("","NA"))
deliveries2 <- read.csv("deliveries2.csv", na.strings=c("","NA"))

Visualizations:
Top 10 Batsman with Highest Runs: ggplotly(Top_10_Batsman)
Highest Toss Winning Teams: Piechart

Summary:
Runs Summary: Runs_Summary %>% flextable::flextable()

# Created by: Akshat Sharma
