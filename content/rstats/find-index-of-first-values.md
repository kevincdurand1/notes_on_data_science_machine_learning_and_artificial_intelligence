Title: Finding the location (the index) of the first instance of values in a vector
Slug: find-index-of-first-values
Summary: Finding the location (the index) of the first instance of values in a vector
Date: 2016-05-01 12:00
Category: R Stats
Tags: Data Wrangling
Authors: Chris Albon


Original source: http://www.unc.edu/~jasperlm/Rsnippets.html

Want to learn more? I recommend working through: [R for Data Science](http://amzn.to/2myxnhi), [R Cookbook](http://amzn.to/2lF6hkb), and [R Graphics Cookbook](http://amzn.to/2m0fcPL).
```R
# Create a list of wars
wars <- c("Spanish Civil War", "Spanish Civil War", "Spanish Civil War", "Spanish Civil War", "WWII", "WWII")
```


```R
# Create a function that finds the index of the first unique value
find.firsts <- function(x) { match(unique(x), x) }
```


```R
# Run the function on the list of wars
find.firsts(wars)
```




    [1] 1 5
