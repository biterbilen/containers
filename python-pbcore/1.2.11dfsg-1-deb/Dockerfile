FROM biocontainers/biocontainers:debian-stretch-backports
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="python-pbcore" \ 
    container="python-pbcore" \ 
    about.summary="Python library for processing PacBio data files" \ 
    about.home="https://github.com/PacificBiosciences/pbcore" \ 
    software.version="1.2.11dfsg-1-deb" \ 
    version="1" \ 
    about.copyright="2011-2015 Pacific Biosciences of California, Inc." \ 
    about.license="PacBio-BSD-3-Clause" \ 
    about.license_file="/usr/share/doc/python-pbcore/copyright" \ 
    extra.binaries="/usr/bin/pbopen" \ 
    about.tags=""

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y python-pbcore && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker
