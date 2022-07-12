# Docker-Learnong

## commands

### run - start a container
*   docker run `IMAGE-NAME`

### ps - list containers (ps: process status)
*   docker ps
*   docker ps -a

### stop - stop a container
*   dockee stop `CONTAINER-NAME` or `CONTAINER-ID`

### rm - remove a container
*   docker rm `CONTAINER-NAME` or `CONTAINER-ID`

### images - list images
*   docker images

### rmi - remove a image
*   docker rmi `IMAGE-NAME`

### pull - download an image
*   docker pull `IMAGE-NAME`

### sleep
*   docker run ubuntu sleep `Integer(secs)`

### exec - execute a command
*   docker exec `CONTAINER-NAME` or `CONTAINER-ID` command

### detach and attach
*   docker run -d `IMAGE-NAME`
*   docker attach `CONTAINER-NAME` or `CONTAINER-ID`

### run - tag
*   docker run `IMAGE-NAME`:`tag`

#### run - stdin
*   docker run -it `IMAGE-NAME`
*   -i for interactive
*   -t for psedu terminal

### run - port mapping
*   docker run -p `free port on docker host`:`port inside of docker container` `IMAGE-NAME`

### run - volume mapping
*   docker run -v `DIRECTORY OUTSIDE`:`DIRECTORY INSIDE` `IMAGE-NAME`

### inspect
*   docker inspect `CONTAINER-NAME`

### logs
*   docker log `CONTAINER-NAME`

### environment variables
*   -e for export
*   docker run -e `EV=ev`  `IMAGE-NAME`

## Dockerfile
### INSTRUCTION ARGUMENT
*   FROM, RUN, COPY, ENTRYOINT
*   sudo docker build . -f `DOCKER-FILE-NAME` -t `IMAGE-NAME`

## Docker compose
*   yaml file docker-compose.yml
*   docker-compose up

### name
*   docker run --name=`NAME` `IMAGE-NAME`

### link - connecting 2 containers for using each other
*   docker run -d --name=`NAME` redis
*   docker run -d --name=vote -p 5000:80 --link redis:`NAME` voting-app
