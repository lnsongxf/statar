statar
======

statar makes it easier to work with tabular datasets. The package includes a set of functions to clean and summarize variables, to join datasets with an SQL-syntax, and to manipulate datasets with a panel
structure. statar is based on the data.table package and is inspired by Stata.

The first vignettes presents [data.frame functions](vignettes/summary.Rmd),  the second presents [panel data functions](vignettes/panel-data.Rmd), the third presents [vector functions](vignettes/vector.Rmd)
the fourth presents [fuzzy merges](vignettes/merge-records.Rmd) , the fifth presents [string and expression interpolation](vignettes/macros.Rmd).

You can install 

- The latest released version from [CRAN](http://cran.r-project.org/web/packages/statar/index.html) with

	```R
	install.packages("statar")
	```
-  The current version from [github](https://github.com/matthieugomez/statar) with  

	```R
	devtools::install_github("matthieugomez/statar")
	```




# News
## 0.3
- demean() is depreciated (still available in utils), now that you can use `felm` with multiple `lhs`
- graph() is deprecated
- stat_binmean() allows to plot the mean of y over the mean of x in given xtiles
- new function pctile() that corresponds to Stata _pctile
## 0.2
- lag(, along_with) and lead(, along_with) become separate functions with prefix t: tlag(, along_with) and tlead(, along_with). The usual lag/lead based on rows can still be found in dplyr
- bin is renamed xtile
- In join, the option type = "outer" is renamed type = "full" similarly to dplyr
- sum_up(), tab(), and find_duplicates() now accept data.frames and grouped dataframes




