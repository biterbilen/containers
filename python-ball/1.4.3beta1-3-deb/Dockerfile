FROM biocontainers/biocontainers:debian-stretch-backports
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="python-ball" \ 
    container="python-ball" \ 
    about.summary="Python bindings for the Biochemical Algorithms Library" \ 
    about.home="http://www.ball-project.org/" \ 
    software.version="1.4.3beta1-3-deb" \ 
    version="1" \ 
    about.copyright=" 1998-2013 the BALL project group" \ 
    about.license="GPL-2+" \ 
    about.license_file="/usr/share/doc/python-ball/copyright" \ 
    about.tags="uitoolkit::qt" 

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y python-ball && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker
