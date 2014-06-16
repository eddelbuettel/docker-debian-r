
## Docker Image 'add-r-devel-san'

This Dockerfile starts from out base image `add-r`, and adds

* all Build-Depends: for the R package
* subversion
* gcc-4.9, g++-4.9 and gfortran-4.9

and checks out the current SVN sources of R-devel.  This image then builds
R-devel from these source using gcc/g++ 4.9 with the Address Sanitizer
configuration [described in Section 4.3.3 of the Writing R Extension
manual](http://cran.rstudio.com/doc/manuals/r-devel/R-exts.html#Using-Address-Sanitizer)

The binary is installed as `/usr/local/bin/Rdevel` to distinguish from `R`
which invokes the released version of R.

