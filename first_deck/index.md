---
title       : Regression model
subtitle    : visualisation / summary of the mtcars data set
author      : Bernard Orzechowski
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}

--- .class #id 

## Goal

Wouldnt't it be great to  


1. Create on the fly different linear models on the mtcars data set in R? 


2. Be able to visualize most importnat chracteristic about created mtcars linear model?  


3. View some plot's that visualise the goodness of the build model?  


--- .class #id 

## Place to do it

You can do it at https://bernardorzechowski.shinyapps.io/DevelopingDataProducts/  

Choose  
1. whatever variable you want as th regressed one (Miles/(US) gallon (mpg)?), and  
2. one or more as the regressors (Weight? Number of cylinders (cyl) and Gross horsepower?)


```r
data(mtcars)
head(mtcars)
```

```
##                    mpg cyl disp  hp drat    wt  qsec vs am gear carb
## Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
## Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
## Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
## Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
## Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
## Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1
```

--- .class #id 

## mtcars characteristics provided

You can check then the following characteristic:

1. general summary produced by R  


2. if residuals are uncorelated to model variables  


3. if mean of residuals is near 0  


4. Shapiro test: are model residuals normal distrbuted?  


--- .class #id 

## mtcars diagnostic plots

You have visualized 4 diagnostic plots:

1. 'Residulas vs Fitted', a plot of residuals values against fitted values (should not follow any pattern)  

2. 'Normal Q-Q'that checks if the residuals follow a Normal Distribution  

3. 'Scale-Location' plot, also called 'Spread-Location' is similar to the residuals versus fitted values plot, but it uses the square root of the standardized residuals. Like the first plot, there should be no discernable pattern to the plot.  

4. 'Cook's distance' is a statistic that tries to identify points which have more influence than other points. Generally these are points that are distant from other points in the data, either for the dependent variable or one or more independent variables.  







