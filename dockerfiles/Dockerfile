FROM ghcr.io/taffish-org/python:3.13.2

LABEL maintainer="taffish@163.com"

WORKDIR /root

COPY . .

RUN wget http://eddylab.org/software/hmmer/hmmer.tar.gz && tar zxf hmmer.tar.gz && cd hmmer-3.4 && ./configure --prefix /usr/local && make && make check && make install && cd easel && make install

ENV TAFFISH_ENV=TAFFISH
ENV TAFFISH_NAME=hmmer
