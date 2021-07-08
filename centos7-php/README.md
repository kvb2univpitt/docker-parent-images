# centos7-php

This is a Docker image of Centos 7.9.2009 with the following software preinstalled:

- Apache HTTPD 2.4 with SSL
- PHP 7.x
- Unzip

## Build the Docker Image

To build the docker image in your local repository, open up a terminal in the directory ***centos7-php***, containing the file **Dockerfile**, and execute the following command:

```
docker build -t local/centos7-php .
```

## Verify the Docker Image

To verify that the Docker image is in your local repository, execute the following command:

```
docker images
```

You should see the output similar to the one below:

```
REPOSITORY                     TAG              IMAGE ID       CREATED          SIZE
local/centos7-php              latest           b5310bd4b394   15 seconds ago   204MB
```

## Remove the Docker Image

To remove the Docker image from the local repository, and execute the following command:

```
docker rmi local/centos7-php
```

## Use the Prebuilt Docker Image

If you don't want to build the image yourself, you can use the prebuilt one on Docker Hub.  Just add the following on the first line of your Dockerfile:

```docker
FROM kvb2univpitt/centos7-php:v1.2021.7
```
