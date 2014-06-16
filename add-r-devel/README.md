
## Docker Image 'add-r-devel'

This Dockerfile starts from out base image `add-r`, and adds

* all Build-Depends: for the R package
* subversion

and checks out the current SVN sources of R-devel, and then builds R-devel.

The binary is installed as `/usr/local/bin/Rdevel` to distinguish from `R`
which invokes the released version of R.


