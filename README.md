make-commands:
	make up: docker-up
	make init: docker-down-clear docker-pull docker-build docker-up manager-init
	make test: manager-test
more: Makefile	