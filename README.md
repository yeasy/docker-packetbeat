Docker-Packetbeat
===
Docker images for the packetbeat.


# Supported tags and respective Dockerfile links

* [`1.0.1, latest` (latest/Dockerfile)](https://github.com/yeasy/docker-packetbeat/blob/master/Dockerfile)

For more information about this image and its history, please see the relevant manifest file in the [`yeasy/docker-packetbeat` GitHub repo](https://github.com/yeasy/docker-packetbeat).

# What is docker-packetbeat?
Docker image with packetbeat installed. The image is built based on [phusion/baseimage](https://github.com/phusion/baseimage-docker).


# How to use this image?
The docker image is auto built at [https://registry.hub.docker.com/u/yeasy/packetbeat/](https://registry.hub.docker.com/u/yeasy/packetbeat/).


## In Dockerfile
```sh
FROM yeasy/packetbeat:latest
```

## Local Run
```sh
$ docker run --net=host -it yeasy/packetbeat packetbeat -e -c /etc/packetbeat/packetbeat.conf
```

# Which image is based on?
The image is based on official `phusion/baseimage:latest`.

# What has been changed?
## install libpcap
Install required  libpcap 0.8.

## install packetbeat
Install packetbeat 1.0.1-x86_64 versin.

## add default conf file
Add the packetbeat.yml to /etc/packetbeat/.

# Supported Docker versions

This image is officially supported on Docker version 1.7.0.

Support for older versions (down to 1.0) is provided on a best-effort basis.

# User Feedback
## Documentation
Be sure to familiarize yourself with the [repository's `README.md`](https://github.com/yeasy/docker-packetbeat/blob/master/README.md) file before attempting a pull request.

## Issues
If you have any problems with or questions about this image, please contact us through a [GitHub issue](https://github.com/yeasy/docker-packetbeat/issues).

You can also reach many of the official image maintainers via the email.

## Contributing

You are invited to contribute new features, fixes, or updates, large or small; we are always thrilled to receive pull requests, and do our best to process them as fast as we can.

Before you start to code, we recommend discussing your plans through a [GitHub issue](https://github.com/yeasy/docker-packetbeat/issues), especially for more ambitious contributions. This gives other contributors a chance to point you in the right direction, give you feedback on your design, and help you find out if someone else is working on the same thing.
