## start with the Debian testing
FROM debian:testing

## That's me
MAINTAINER Dirk Eddelbuettel edd@debian.org

## Remain current
RUN apt-get update -qq
RUN apt-get dist-upgrade -y

RUN apt-get install -y --no-install-recommends r-base r-base-dev r-recommended littler
RUN ln -s /usr/share/doc/littler/examples/install.r /usr/local/bin/install.r

## can be launched / used from the command-line via 
##   cat Dockerfile | docker build -t debian:testing-with-R -
## to create an image under tag 'debian:testing-with-R'
