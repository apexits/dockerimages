#Description
This is public repository for Apex IT Services.
The following docker images are built from Dockerfiles on the Apex Github.

ubuntu-oracle-jdk8-tomcat8 
ubuntu-oracle-jdk8-tomcat9

## Base and latest Ubuntu OS image with JDK8 and Tomcat 8/9

This repository contains **Dockerfile** of [Ubuntu](http://www.ubuntu.com/) for [Docker](https://www.docker.com/)'s [automated build](https://hub.docker.com/u/apexits/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).

### Docker Repositories

`ubuntu-oracle-jdk8-tomcat8 ` provides only one single tagged image:

* `latest` (default)

`ubuntu-oracle-jdk8-tomcat9 ` provides only one single tagged image:

* `latest` (default)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download the appropriate image [automated build](https://hub.docker.com/u/apexits/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull apexits/ubuntu-oracle-jdk8-tomcat8`

    (alternatively, you can build an image from Dockerfile: `docker build -t="apexits/ubuntu-oracle-jdk8-tomcat8" https://github.com/apexits/dockerimages/tree/master/ubuntu-oracle-jdk8-tomcat8`)

### Usage

    docker run -d -it -p 8080:8080 apexits/ubuntu-oracle-jdk8-tomcat8 
