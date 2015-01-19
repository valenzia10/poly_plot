---
title       : Polynomial Plotter
subtitle    : A Shiny app to plot a polynomial right inside your browser!
author      : E. Valencia
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

- How many times have you wondered how would that polynomial function look like?

- Pen and paper is boring and exhasperating...

- and you not always have RStudio or Matlab around...

- but you always have a browser close to you!

---

## Polynomial Plotter: Magic inside the browser

- The browser is the most widely spread runtime environment.

- Polynomial Plotter solves your pain point allowing you to plot that polynomial function right inside your browser.

- Polynomial Plotter is a Shiny app that shines by itself ;p

--- .codefont

## How it works?
- Introduce the coefficients using the numeric fields. You can plot up to an order 5 polynomial.
- Coefficients are input from highest order to the lowest one:
$$y =  \alpha_5 \cdot x^5 + \alpha_4 \cdot x^4 + \alpha_3 \cdot x^3 + \alpha_2 \cdot x^2 + \alpha_1 \cdot x + \alpha_0$$

- For instance, $\alpha_5=0.8$, $\alpha_4=0.3$, $\alpha_3=-0.5$, $\alpha_2=0.4$, $\alpha_1=-0.2$, and $\alpha_0=0$ will produce following plot:

```r
x <- seq(-10,10,0.1)
y <- 0.8*x^5 + 0.3*x^4 - 0.5*x^3 + 0.4*x^2 - 0.2*x + 0
plot(x,y,col='blue',type='l')
```

<img src="assets/fig/unnamed-chunk-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" style="display: block; margin: auto;" />

---

## Where can I find it?

- Just follow the link:

[Polynomial Plotter](https://polyplot.shinyapps.io/shinyPolynomialPlotter/)


