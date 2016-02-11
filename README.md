# Apex Ubuntu Images
This is public repository for Apex IT Services.
This repository contains **Dockerfile** of [Ubuntu](http://www.ubuntu.com/) for [Docker](https://www.docker.com/)'s [automated build](https://hub.docker.com/u/apexits/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).

The following docker images are built from Dockerfiles on the Apex Github. 
1. ubuntu-oracle-jdk8-tomcat8 
2. ubuntu-oracle-jdk8-tomcat9


### Docker Repositories

`ubuntu-oracle-jdk8-tomcat8 ` Ubuntu with Oracle JDK 8.74 and Tomcat 8.0.32:

* `latest` (default)

`ubuntu-oracle-jdk8-tomcat9 ` provides Ubuntu with Oracle JDK 8.74 and Tomcat 9.0.0.M3:

* `latest` (default)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download the appropriate image [automated build](https://hub.docker.com/u/apexits/) from public [Docker Hub Registry](https://registry.hub.docker.com/): 
	For e.g. 
 		The command will pull the ubuntu-oracle-jdk8-tomcat8 image:  `docker pull apexits/ubuntu-oracle-jdk8-tomcat8`
    	Alternatively, you can build an image from Dockerfile: 
    	`docker build -t="apexits/ubuntu-oracle-jdk8-tomcat8" https://github.com/apexits/dockerimages/tree/master/ubuntu-oracle-jdk8-tomcat8`)

### Usage
	The command below creates a container with tomcat up and running and port 8080 exposed. 
    docker run -d -it -p 8080:8080 apexits/ubuntu-oracle-jdk8-tomcat8 

### Courtesy
	JDK Installation instructions i[isuper/java-oracle] (https://hub.docker.com/r/isuper/java-oracle/)
	Tomcat Installation instructions i[tomcat] (https://hub.docker.com/_/tomcat/)
