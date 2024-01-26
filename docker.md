# Docker Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

A cheat sheet for Docker commands.

#

[variable] = placeholder for a variable

#

### Start Docker

> docker-compose up

### Start Docker in background

> docker-compose up -d

### only Build Docker Image

> docker-compose build

### Build Docker Image and start

> docker-compose up --build

### Stop Docker and remove containers

> docker-compose down

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

### Deleting

| Command                                            | Description                                                  |
| -------------------------------------------------- | ------------------------------------------------------------ |
| `docker rm [containerID or containerName]`         | Delete one or more containers                                |
| `docker rm -f [containerID or containerName]`      | Force remove one or more containers                          |
| `docker rm -v $(docker ps -a -q -f status=exited)` | Delete all stopped containers                                |
| `docker rm $(docker ps -a -q)`                     | Delete all containers                                        |
| `docker rmi [imageID or imageName]`                | Remove one or more images                                    |
| `docker rmi $(docker images -q)`                   | Delete all images                                            |
| `docker rmi $(docker images -q -f dangling=true)`  | Delete all dangling images                                   |
| `docker volume rm $(docker volume ls -q)`          | Delete all volumes                                           |
| `docker network rm $(docker network ls -q)`        | Delete all networks                                          |
| `docker system prune`                              | Delete all containers, images, volumes and networks not used |

### Stop all containers

> docker stop $(docker ps -a -q)

### delete container volume

> docker volume rm [containerID or containerName]

or

> docker rm -v [containerID or containerName]

### delete all container volumes

> docker volume rm $(docker volume ls -q)

### delete all docker images

> docker rmi $(docker images -q)

### delete all docker networks

> docker network rm $(docker network ls -q)

### set resource limits for a container

    deploy:
      resources:
        limits:
          cpus: "0.5" # Limits the container to use at most 50% of one CPU core
          memory: "2000M" # Limits the container to use at most 512 megabytes of memory
        reservations:
          cpus: "0.25" # Reserves 25% of one CPU core for the container
          memory: "1000M" # Reserves 256 megabytes of memory for the container
