VERSION=v3
PROJECT_ID=akrainoenea
PROJECT=docker.io/${PROJECT_ID}

all: build

build:
	docker build --pull -t ${PROJECT}/k8szk:${VERSION} .

push: build
	gcloud docker -- push ${PROJECT}/k8szk:${VERSION}

.PHONY: all build push
