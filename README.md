# European Options Implied Volatilities (R Package)

This repository contains code for an R package that contains functions to compute and graph implied volatilities for European Options. 

September, 2016

## How to use this package

### 1. Make sure you have devtools installed

```
install.packages(c("devtools", "roxygen2", "testthat", "knitr"))
```

Technically `roxygen2`, `testthat`, and `knitr` are only required if you are going to further develop this (or any other) package.

### 2. Install the package using GitHub

```
devtools::install_github("jdoleiv/implied_volatility")
```

### 3. Load the package in R

```
library(ImpliedVolatility)
```

### 4. Use the functions included in the pacakge

To see the available datasets included in the package (currently only one), execute:

```
data(package = "ImpliedVolatility")
```

If you want to use the included European Options dataset, execute:

```
data(european_options)
```

You may compute and graph the implied volatilities with:

```
results <- compute_and_graph_implied_volatilities(european_options)
```

You may also use the functions directly yourself:

```
implied_voltility <- compute_implied_volatilities("call", )
results <- append_implied_volatilities(european_options)
graph_implied_volatility(results)
```


