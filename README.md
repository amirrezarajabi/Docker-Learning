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