Shiny Application and Reproducible Pitch Assignment
========================================================
author: Ranjit Subudhi
date: 27th June 2019
autosize: true

Course Project Assignment
========================================================


- Peer-graded Assignment: Course Project: Shiny Application and Reproducible Pitch
- The Project consists of two activites
  - Create a Shiny application and deploy it on Rstudio's servers
  - Use Slidify or Rstudio Presenter to prepare a reproducible pitch presentation about your application

Select the Best Car for the Trip
========================================================
This app helps us to choose a car for a trip, using the mtcars dataset from [R].

- First, we need to inform the distance of your trip and the price of gasoline in your region. These information will be used to calculate the Gasoline Expenditure for each car in the dataset. Then, we can enter the maximum amount of money we want to spend on gasoline, and the table shows only the cars that have Miles per Gallon (mpg) that can go below this value.

- Second, we can choose some caractheristcs of the cars that you desire: Cylinders, Displacement, Horse Power and Transmission. The table will show only the cars with the filters selected. We can sort the table according to the variable you want by clicking the arrows at the top of the table.


Select the Best Car for the Trip
========================================================


```r
data(mtcars)
head(mtcars)
```

```
                   mpg cyl disp  hp drat    wt  qsec vs am gear carb
Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1
```

Plotting Data
========================================================
  


```r
pairs(mtcars, panel=panel.smooth, main="Pair Graph of Motor Trend Car Road Tests")
```

![plot of chunk unnamed-chunk-2](Shiny Assignment-figure/unnamed-chunk-2-1.png)
