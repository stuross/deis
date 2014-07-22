FROM ubuntu:14.04
MAINTAINER OpDemand <info@opdemand.com>

RUN apt-get update && apt-get install -y swift python-swiftclient openssh-server

RUN mkdir -p /etc/swift
RUN chown -R swift:swift /etc/swift/

RUN mkdir -p /var/cache/swift /srv/node/
RUN chown swift:swift /var/cache/swift
