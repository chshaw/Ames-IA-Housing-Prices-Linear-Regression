
# Project 2: Ames, Iowa Housing Prices


## Problem Statement

What is the best way to model housing prices in Ames, Iowa?

## Executive Summary

Modeling the Ames, Iowa housing data to predict sales prices, the best regression model involved amplifying highly correlated features and creating interaction terms between them.

### Contents:
- [Data Dictionary](#Data-Dictionary)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

## Data Dictionary

The original data dictionary for this dataset can be found at 
[http://jse.amstat.org/v19n3/decock/DataDocumentation.txt]

For all interaction terms, refer to the follow table:

|Feature|Type|Dataset|Description|
|---|---|---|---|
|1st_flr_sf_2|float|created|Duplicated 1st floor squarefootage column.| 
|overall_qual_2|float|created|Duplicated overall quality column.| 
|gr_liv_area_2|float|created|Duplicated ground living area column.| 
|overall_qual_*gr_liv_area|float|created|Multiplied overall quality by ground living area.| 
|overall_qual_*1st_flr_sf|float|created|Multiplied overall quality by 1st floor squarefootage.|

## Conclusions and Recommendations

The strong correlation of overall quality, ground living area and 1st floor squarefootage allowed for the creation of other polynomial features which enhanced the model.  Of the three types of linear regression (linear, ridge and lasso), ridge and lasso performed much better than simple linear regression.
