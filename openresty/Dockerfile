FROM centos

MAINTAINER "penglong"

COPY ./a.text /test/

COPY ./test.sh /test/

RUN yum install -y openssl openssl-devel  gcc

RUN yum install -y perl pcre zlib pcre-devel

ADD ./openresty-1.13.6.1.tar.gz ./

RUN cd /openresty-1.13.6.1 && ./configure --prefix=/usr/local/openresty \
       && make \
       && make install \
       && make clean 

EXPOSE 22 80

