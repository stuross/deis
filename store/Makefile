include ../includes.mk

build:
	$(call rsync_all)
	$(call ssh_all,'cd share/store && sudo docker build -t deis/store .')
