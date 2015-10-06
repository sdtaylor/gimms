

# Introducing the R **gimms** package

### What it is all about
We've been collecting functions related to the download and processing of AVHRR 
GIMMS data for quite some time and with the most recent update to GIMMS3g 
(Pinzon and Tucker, 2014), we thought it was a good time to stuff the most 
fundamental work steps into a proper R package. In this context, 'most 
fundamental' refers to certain operations which we tended to repeat over and 
over again, including

* list all GIMMS files available online at [NASA ECOCAST](http://ecocast.arc.nasa.gov/data/pub/gimms/3g.v0/),
* download selected (or all) files, 
* re-arrange the list of downloaded files according to date, 
* transform binary data in ENVI format to proper **raster** format (Hijmans, 2015) and 
* aggregate the bi-monthly datasets to monthly maximum value composites (MVC).

In the following, you'll find a short introduction of what we came up with so 
far. Feel free to comment, raise issues and provide (constructive) criticism.
Any suggestions on how to improve the **gimms** package are highly appreciated!

### How to install
At present, the **gimms** package can be installed directly from 
[GitHub](https://github.com/environmentalinformatics-marburg/gimms) via 


```r
## install 'gimms' package
library(devtools)
install_github("environmentalinformatics-marburg/gimms")

## load 'gimms' package
library(gimms)
```

There is no such thing as a 'development' branch yet, but be assured that such 
things will possibly be provided in the near-distant future. 
