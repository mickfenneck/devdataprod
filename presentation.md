BMI: calculate your Body Mass Index now
========================================================
author: mickfenneck
date: 22/02/2015

Why
========================================================

I chose this subject because:

- it's pretty easy to develop
- it's a simple ui-server app
- I was very busy with my work


How
========================================================

The code, like in every shiny app, is divided in two part:

- ui.R: containing the interface
- server.R: containg the calculus


How it works
========================================================
You can choose you weight and height

```r
weight<-69
height<-1.7
```
And have the calculation done

```r
BMI_value<-weight/(height^2)
ifelse(BMI_value<18.5,"underweight", ifelse(BMI_value<25, "normal weight", ifelse(BMI_value<30,"overweight","obesity")))
```

```
[1] "normal weight"
```

Where can I find it?
========================================================

The app is hosted on shinyapps.io at https://mickfenneck.shinyapps.io/weight/

You can find the R code at https://github.com/mickfenneck/devdataprod
