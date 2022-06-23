FROM balenalib/armv7hf-debian:buster

RUN mkdir src

COPY ./src/ ./src/


RUN apt-get update

RUN DEBIAN_FRONTEND="noninteractive" apt-get -y install tzdata

RUN apt-get install -y sudo \
&& apt-get install -y python3.8 \
&& apt-get install -y iputils-ping \
&& apt-get install -y net-tools \
&& apt-get install -y git \
&& apt-get -y install nano \
&& apt --yes install python3-pip \	
&& pip install pyModbusTCP \
&& apt install telnet \
&& apt install telnetd \
&& apt-get install -y memcached \
&& apt-get install -y python3-memcache \ 
&& apt-get install -y ettercap-common \
&& apt-get install -y nmap

WORKDIR /src

