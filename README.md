# docker-aws-apex

[![Docker Stars](https://img.shields.io/docker/stars/jimdo/aws-apex.svg?maxAge=600)](https://hub.docker.com/r/jimdo/aws-apex/) [![Docker Pulls](https://img.shields.io/docker/pulls/jimdo/aws-apex.svg?maxAge=600)](https://hub.docker.com/r/jimdo/aws-apex/)


## Content
 * awscli
 * awscurl
 * apex

## Install
Pull from Docker Hub:

    $ docker pull jimdo/aws-apex

Or build from source:

    $ git clone https://github.com/jimdo/docker-aws-apex && cd docker-aws-apex
    $ docker build -t aws-apex .

## Usage
Simply run (a `bash` session):

    $ docker run --name aws_apex -it jimdo/aws-apex

Run and mount a local directory inside the container:

    $ docker run --name aws_apex -v ~/my/project/folder:/home/projectone -it jimdo/aws-apex

If you want to ***demonize*** the container just add the `-d` flag:

    $ docker run --name aws_apex -d -it jimdo/aws-apex

### Reattach container if demonized

    $ docker exec -it aws_apex bash

## License

MIT
