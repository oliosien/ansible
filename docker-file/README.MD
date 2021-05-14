# Target

Create a docker image with:
 
 - SSH service installed
 - Paython 3.7 installed
 - ansible group created
 - ansible user created (with shell to be able to create ssh connection)
 - expose 22 port to localhost

## Docker reference

Coomand line reference

https://docs.docker.com/engine/reference/run/

Dockerfile

https://docs.docker.com/engine/reference/builder/

Compose specification

https://docs.docker.com/compose/compose-file/

## Some usefull commands

To create a container named `centos-8-test` from `centos` image and `8` tag, with a pesudo-tty (`-t`) and in intercative mode (`-i`). We bind port 8080 of the container to TCP port 80 on 127.0.0.1 (for `tcp` protocol):

`$docker run --name -p 127.0.0.1:80:8080/tcp centos-8-test -it centos:8`

To create an image called `c8-systemd` tagged by `latest` deleting all intermediate containers (`--rm`) starting from a Dockerfile (located in current path `.`):

`$docker build --rm -t c8-systemd:latest .`

Here we run container in background (`-d`) and give all capabilities to the container (`--privileged`):

`$docker run -it -p 127.0.0.1:22:22 --privileged --name=c8-systemd-ansible c8-systemd:latest`


