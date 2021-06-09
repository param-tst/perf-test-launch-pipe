# Base Docker Image

* [java:8-jdk-alpine](https://registry.hub.docker.com/_/java/)

# Docker Tags



# Installation

* Install [Docker](https://www.docker.com/)

* Get automated build from public registry:

Latest version:

`docker pull gatling:latest`





# Usage

Use image to run container

```
docker run -it --rm imageId:tag
```

Mount configuration and simulation files from host machine and run gatling in interactive mode

```
docker run -it --rm -v /home/core/gatling/results:/opt/gatling/results \
imageId:tag
```

Use the -e switch to use JAVA_OPTS to pass parameters to gatling tests

```
docker run -e JAVA_OPTS="Need to specify the " -it --rm imageId:tag
```
