# Translate R Markdown and Quarto documents using poEdit

<!-- badges: start -->
<!-- badges: end -->

With {rmdpo} you convert R Markdown and Quarto documents into .po files that contain each block of the original document as a string to be translated using, for instance, [poEdit](https://poedit.net). This is done with the `rmd2po()` function. Once the translation is done, you can convert the .po file back into a translated R Markdown or Quarto document with `po2rmd()`.

When the original document is modified, just rerun the `rmd2po()` function to update the .po file with the new strings to be translated. The translation can be done incrementally, block by block, and the translated document can be updated incrementally as well.

Most of the work is done internally by the `mdpo` Python library. Special care is taken for R Markdown and Quarto specific syntax, such as the YAML header and code chunks than `mdpo` does not handle correctly otherwise.

## Installation

You can install the development version of {rmdpo} from [GitHub](https://github.com/) with:

``` r
# install.packages("remotes")
remotes::install_github("SciViews/rmdpo")
```

## Example

TODO...

``` r
library(rmdpo)
## basic example code
```

## Code of Conduct

Please note that the {rmdpo} project is released with a [Contributor Code of Conduct](https://contributor-covenant.org/version/2/1/CODE_OF_CONDUCT.html). By contributing to this project, you agree to abide by its terms.
