FROM ubuntu:14.04

MAINTAINER Michal Stuglik <stuglik@gmail.com>

RUN apt-get update -y

RUN apt-get install -y wget openssl bzip2

RUN echo 'export PATH=/opt/conda/bin:$PATH' > /etc/profile.d/conda.sh && \
    wget --quiet https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh && \
    /bin/bash /Miniconda2-latest-Linux-x86_64.sh -b -p /opt/conda && \
    rm Miniconda2-latest-Linux-x86_64.sh && \
    /opt/conda/bin/conda install --yes conda
