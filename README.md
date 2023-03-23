# Fifa2021-Data-Cleaning-Task

## Introduction

This documentation entails the Data cleaning process of the FIFA 21 data set, sourced [kaggle.com](https://www.kaggle.com/) The raw data; **“fifa21 raw data v2.csv”** was used for the Data cleaning task. Power Query Editor for PowerBi was used to complete this process.


## Data Description

The FIFA 21 dataset contains 18,979 rows and 77 columns. The dataset included various data types, including whole numbers, text, and dates. The columns contain information about players such as statistics, positions, photo-URL, earnings, Nationality, clubs,  performance metrics, etc.

## Problem statements

- What is the contract duration years?
- What players are on loan or free contract?
- What are the players' values, Wages, and Release clause in Dollars?
- What are the players’ heights in (cm) and Weights in (lbs)?


## Data Cleaning Process

I used M language and other power query features to clean and transform the data set to be cleaned and ready for further analysis.


## Photo URL correction

The original URL links contain an error that made the link invalid, and unable to provide the players' photos. I noticed the links contain **“.com” and “_60”**  which are supposed to be **“.net” and “_240”**. For example, ([original link](https://cdn.sofifa.com/players/158/023/21_60.png)) - invalid.  

To fix the error, I corrected the link by replacing **“.com” and “_60”**  with **“.net” and “_240”** using replace value function.  For example, ([corrected link](https://cdn.sofifa.net/players/158/023/21_240.png)) - valid.


## Before

:-----------------------------:                                                                  

![](https://github.com/Drwaley/Fifa2021--Data--Cleaning-Task/blob/main/unclean_photo_url.png) ![](https://github.com/Drwaley/Fifa2021--Data--Cleaning-Task/blob/main/clean_photo_url.png)


