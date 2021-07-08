# centos7-openjdk8

This is a Docker image of Centos 7.9.2009 with the following software preinstalled:

- OpenJDK 8
- Unzip

## Build the Docker Image

To build the docker image in your local repository, open up a terminal in the directory ***centos7-openjdk8**, containing the file **Dockerfile**, and execute the following command:

```
docker build -t local/centos7-openjdk8 .
```

## Verify the Docker Image

To verify that the Docker image is in your local repository, execute the following command:

```
docker images
```

You should see the output similar to the one below:

```
REPOSITORY                     TAG              IMAGE ID       CREATED          SIZE
local/centos7-openjdk8         latest           d027c7475858   11 seconds ago   571MB
```

## Remove the Docker Image

To remove the Docker image from the local repository, and execute the following command:

```
docker rmi local/centos7-openjdk8
```

## Use the Prebuilt Docker Image

If you don't want to build the image yourself, you can use the prebuilt one on Docker Hub.  Just add the following on the first line of your Dockerfile:

```docker
FROM kvb2univpitt/centos7-openjdk8:v1.2021.7
```
