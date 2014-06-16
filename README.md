
## Docker for R on Debian

This repository contains several Dockerfiles defining Docker images which
build on the default Debian image for Docker. 

### Docker Images

We start from Debian testing and then add

* add-r:  This image adds the R executable
* add-r-devel: This image adds a freshly-built R-devel version, as well as
all tools required to build R-devel from source
* add-r-devel-san: This image builds R-devel from source using gcc/g++ 4.9
with the Address Sanitizer configuration [described in Section 4.3.3 of the
Writing R Extension manual](http://cran.rstudio.com/doc/manuals/r-devel/R-exts.html#Using-Address-Sanitizer)

### Docker Hub

This repository is linked to 
[this automated build facility at Docker](https://registry.hub.docker.com/u/eddelbuettel/docker-debian-r/)
and one can retrieve the corresponding images via a standard `docker pull`.

### Author

Dirk Eddelbuettel

### License

GPL (>= 2)

