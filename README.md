# HackDo Docker Image

A Docker image for [HackDo](https://github.com/hackerspacesg/hackdo/).

> HackDo is meant to be a membership (and others) management system for Hackerspaces.

## Installation

Pull [the image](https://hub.docker.com/r/valentine/rclone/) from Docker Hub:

    docker pull valentine/hackdo:latest

Create a container using `docker run`, specifying the host and container port respectively in the `-p=` parameter:

    docker run -d \
      -p=58180:80 \
      valentine/hackdo:latest

The above, in one line:

    docker run -d -p=58180:80 valentine/hackdo:latest

## Usage

The superuser credentials are currently hardcoded by default. The username is `hackdo` and the password is `demo`.

You may wish to fork the repository and build your own container if you would like to change the credentials.

## Licence

Code licensed under The MIT License (MIT).
