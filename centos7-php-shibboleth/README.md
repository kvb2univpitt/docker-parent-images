# centos7-php-shibboleth

This is a Docker image of Centos 7.9.2009 with the following software preinstalled:

- Apache HTTPD 2.4 with SSL
- PHP 7.x
- Unzip
- Wget
- Shibboleth

## Build the Docker Image

To build the docker image in your local repository, open up a terminal in the directory ***centos7-php-shibboleth***, containing the file **Dockerfile**, and execute the following command:

```
docker build -t local/centos7-php-shibboleth .
```

## Verify the Docker Image

To verify that the Docker image is in your local repository, execute the following command:

```
docker images
```

You should see the output similar to the one below:

```
REPOSITORY                         TAG              IMAGE ID       CREATED         SIZE
local/centos7-php-shibboleth       latest           43a0333c3f00   9 minutes ago   598MB
```

## Remove the Docker Image

To remove the Docker image from the local repository, and execute the following command:

```
docker rmi local/centos7-php-shibboleth
```

## Use the Prebuilt Docker Image

If you don't want to build the image yourself, you can use the prebuilt one on Docker Hub.  Just add the following on the first line of your Dockerfile:

```docker
FROM kvb2univpitt/centos7-php-shibboleth:v1.2021.8
```
