FROM biocontainers/biocontainers:debian-stretch-backports
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="python3-cutadapt" \ 
    container="python3-cutadapt" \ 
    about.summary="Clean biological sequences from high-throughput sequencing reads (Python 3)" \ 
    about.home="http://pypi.python.org/pypi/cutadapt" \ 
    software.version="1.12-2-deb" \ 
    version="1" \ 
    about.copyright="2010-2015 Marcel Martin <marcel.martin@scilifelab.se>" \ 
    about.license="Expat" \ 
    about.license_file="/usr/share/doc/python3-cutadapt/copyright" \ 
    about.tags=""

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y python3-cutadapt && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker
