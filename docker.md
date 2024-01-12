# Docker Cheat Sheet

A cheat sheet for Docker commands.

#

### Start Docker

> docker-compose up

### only Build Docker Image

> docker-compose build

### go to the root directory of your porject and list the running containers

> docker ps

### open bash in container

> docker exec -it [containerID or containerName] bash -l

### show docker logs

> docker-compose -f docker-compose.prod.yml logs

> docker-compose logs

### show docker logs for specific container

> docker-compose -f docker-compose.prod.yml logs [containerName or containerID]

> docker-compose logs [containerName or containerID]

or

> docker logs [containerName or containerID]

### how to remove all docker containers

> docker rm $(docker ps -a -q)

### Restart Container

> docker restart [containerID or containerName]

### Restart all containers

> docker restart $(docker ps -q)

### delete container volume

> docker volume rm [containerID or containerName]

or

> docker rm -v [containerID or containerName]

### delete all container volumes

> docker volume rm $(docker volume ls -q)
