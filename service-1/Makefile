BRANCH  ?= $(shell git rev-parse --abbrev-ref HEAD)
ifeq ($(BRANCH),master)
        BRANCH=latest
endif
IMG=myimage:$(BRANCH)

all: push

build:
        docker build -t $(IMG) .
