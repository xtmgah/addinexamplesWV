
<!-- README.md is generated from README.Rmd. Please edit that file -->
Note: John Mount, Win-Vector LLC, 11-17-2017
--------------------------------------------

[This repository](https://github.com/WinVector/addinexamplesWV) is a fork of [RStudio's original](https://github.com/rstudio/addinexamples).

Added [`insertDotPipeAddin()`](https://github.com/WinVector/addinexamplesWV/blob/master/R/insertDotPipeAddin.R) which inserts [`wrapr`](https://winvector.github.io/wrapr/)'s [`%.>%`](https://winvector.github.io/wrapr/articles/dot_pipe.html) ("dot pipe").
Suggest using the RStudio instructions and binding this to `F9` (which has a right-facing glyph on some Mac keyboards) via `Tools->Addins->BrowseAddins->KeyboardShortCuts`.

We have renamed the package and removed all other functionality so that this package does not interfere with installing and using the original package.

Installation
------------

First, ensure that you have the latest versions of [htmltools](https://github.com/rstudio/htmltools), [shiny](https://github.com/rstudio/shiny), [miniUI](https://github.com/rstudio/miniUI), [formatR](https://CRAN.R-project.org/package=formatR), and [wrapr](https://CRAN.R-project.org/package=wrapr); then install this package.

``` r
if (!requireNamespace("devtools", quietly = TRUE)) {
  install.packages("devtools")
}
install.packages(c("htmltools", "shiny", "miniUI", "formatR", "wrapr"))
# Edit: installing forked version instead of original "rstudio/addinexamples"
devtools::install_github("WinVector/addinexamples")
```
