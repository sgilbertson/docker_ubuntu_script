ubuntu
======

Build a docker image for ubuntu.

Run `build-image.sh` to build the default docker image `32bit/ubuntu:18.04`.

You can also specify the desired version and architecture, using two optional arguments.
For example, to build an image for 64-bit Ubuntu 24.04:

```
sudo ./build-image.sh noble amd64
```

The resulting Docker image is minimal:

```
$ docker images
REPOSITORY            TAG       IMAGE ID       CREATED         SIZE
ubuntu-bionic-amd64   latest    b6126b1a891c   5 seconds ago   540MB
...
```

See also:
 - https://github.com/ioft/dockerhub
 - http://mwhiteley.com/linux-containers/2013/08/31/docker-on-i386.html
 - https://dzone.com/articles/docker-daemon-for-32-bit-architecture
