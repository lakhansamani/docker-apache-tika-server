# docker-apache-tika-server

This repo contains the Dockerfile to create a docker image that contains the latest Ubuntu running the Apache Tika 1.21 Server on Port 9998 using Java 8. It does not include `tesseract`.

## Usage

First you need to pull down the build from Dockerhub, which can be done by invoking:

    docker pull lakhansamani/docker-apache-tika-server

Then to run the container, execute the following command:

    docker run -d -p 9998:9998 lakhansamani/docker-apache-tika-server

## Building

To build the image from scratch, simply invoke:

    docker build -t 'docker-apache-tika-server' github.com/lakhansamani/docker-apache-tika-server

You can then use the following command (using the name you allocated in the build command as part of -t option):

    docker run -d -p 9998:9998 docker-apache-tika-server

## More

For more info on Apache Tika Server, go to the [Apache Tika Server documentation](http://wiki.apache.org/tika/TikaJAXRS).

## Author

- Lakhan Samani (<lakhan.m.samani@gmail.com>)
