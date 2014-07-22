include ../includes.mk

build:
	$(call rsync_all)
	$(call ssh_all,'cd share/store-proxy && sudo docker build -t deis/store-proxy .')
