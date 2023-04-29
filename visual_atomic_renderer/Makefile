.phony : all, build, web, test, test-parallel, clean

DOCKER_IMAGE=forkvisualatom

all: build

build:
	-rm -f Manifest.toml docs/Manifest.toml
	docker build -t ${DOCKER_IMAGE} . --build-arg NB_UID=`id -u`
	docker compose build
