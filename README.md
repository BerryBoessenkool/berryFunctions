### intro

Miscellaneous R functions. Notable: colPoints, horizHist, logAxis, pointZoom, smallPlot, lsc.

**See the [Vignette](https://cran.r-project.org/web/packages/berryFunctions/vignettes/berryFunctions.html) for an overview of the package.**

[Recent changes](http://starlogs.net/#brry/berryFunctions) (Thanks, [Jenny](http://happygitwithr.com/comic-relief.html))


### installation
Install release version from CRAN:
[![CRAN_Status_Badge](http://www.r-pkg.org/badges/version-last-release/berryFunctions)](http://cran.r-project.org/package=berryFunctions) 
[![downloads](http://cranlogs.r-pkg.org/badges/berryFunctions)](http://www.r-pkg.org/services)
[![Rdoc](http://www.rdocumentation.org/badges/version/berryFunctions)](http://www.rdocumentation.org/packages/berryFunctions)


```R
install.packages("berryFunctions")
library(berryFunctions)
vignette("berryFunctions")
?berryFunctions
```

Update to the current development version from github:
<script src="http://gist-it.appspot.com/github/brry/berryFunctions/blob/master/DESCRIPTION?slice=3:5"></script>
```R
source("http://raw.githubusercontent.com/brry/berryFunctions/master/R/instGit.R")
instGit("brry/berryFunctions")

# or use devtools:
if(!requireNamespace("devtools", quitly=TRUE)) install.packages("devtools")
devtools::install_github("brry/berryFunctions")
```

### trouble

If direct installation from CRAN doesn't work, your R version might be too old. In that case, an update is really recommendable: [r-project.org](http://www.r-project.org/). If you can't update R, try installing from source (github) via `instGit` or devtools as mentioned above. If that's not possible either, here's a manual workaround:
click on **Clone or Download - Download ZIP** (top right, [link](https://github.com/brry/berryFunctions/archive/master.zip)), unzip the file to some place, then
```R
setwd("that/path")
dd <- dir("berryFunctions-master/R", full=T)
dummy <- sapply(dd, source)
```
This creates all R functions as objects in your globalenv workspace (and overwrites existing objects of the same name!).

### license

This package is under the GPL license.
I am fine with you doing whatever you want with it, provided that my name and credit remains attached to it.
If you legally need a more permissive license, let me know and I can probably change it.
