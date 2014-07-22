FROM ubuntu:14.04
MAINTAINER OpDemand <info@opdemand.com>

RUN apt-get update && apt-get install swift-proxy memcached

CWD /etc/swift
RUN openssl req -new -x509 -nodes -out cert.crt -keyout cert.key

RUN perl -pi -e "s/-l 127.0.0.1/-l $PROXY_LOCAL_NET_IP/" /etc/memcached.conf

RUN service memcached restart

EXPOSE 8080
