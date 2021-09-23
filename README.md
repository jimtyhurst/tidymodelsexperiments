
# tidymodelsexperiments

A collection of sample code demonstrating how to use {[tidymodels](https://www.tidymodels.org/)} packages. I use it as a workspace for my own explorations. I do not expect other people to use it, but if someone else finds it useful while learning about {tidymodels}, so much the better.

---

## Contents

* [Installation](#installation)
* [Build a vignette](#build-a-vignette)
* [Analyses](#analyses)
* [Package dependencies](#package-dependencies)
* [Why is this project organized as an R package?](#why-is-this-project-organized-as-an-r-package)
* [Resources](#resources)
* [License](#license)

---

## Installation

Install `tidymodelsexperiments` from [GitHub](https://github.com/) with:

``` r
remotes::install_github("jimtyhurst/tidymodelsexperiments")
```

## Build a vignette

To build a vignette from the command line:

```r
rmarkdown::render("./vignettes/my-vignette.Rmd")
```

## Analyses

* [Hello Models: Ames Housing Data](./vignettes/Ames-Housing-Data.md)


## Package dependencies

See the `Imports` in the [DESCRIPTION](./DESCRIPTION) file.


## Why is this project organized as an R package?
Even though I do not expect other people to use this code, I find it very useful to organize my code within the framework of an R package, because the package structure provides a standard set of conventions for:

* Project directory structure for organizing the many components of a cohesive set of code files and configuration files:
    * source files in the [R](./R) directory.
    * example code in the [vignettes](./vignettes) directory.
    * unit tests in the [tests/testthat](./tests/testthat) directory.
    * dependency configurations in the [DESCRIPTION](./DESCRIPTION) file.
    * data in the [inst](./inst) directory.
* Building the project from within [RStudio](https://www.rstudio.com/) or on the command line with `R CMD build`.
* Running the unit tests with [devtools::test()]().

For all these reasons, I do most of my R development within a package project.


## Resources

* Max Kuhn and Julia Silge. 2021-09-08. [Tidy Modeling with R](https://www.tmwr.org/).
* [Tidymodels](https://www.tidymodels.org/)
* Jim Tyhurst. [{tidymodels}: Notes](https://github.com/jimtyhurst/annotated_bibliography/blob/main/tidymodels-notes.md).


## License
Copyright &copy; 2021 Jim Tyhurst

Licensed under the [MIT](https://opensource.org/licenses/MIT) License.
