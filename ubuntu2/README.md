# dockerfiles-ubuntu-user-adderable
Ubuntu, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build   --rm -t kangdo/ubuntu:5 .
	docker run -it --rm --name u1  kangdo/ubuntu:5
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE                COMMAND             CREATED             STATUS              PORTS               NAMES
63a0ba73bf81        kangdo/ubuntu:test   "/bin/bash"         4 seconds ago       Up 3 seconds                            u1
```

To test,
```
	tree
```
To Rollback
```
    docker rm u1 -f 
    docker rmi kangdo/ubuntu:test
```
