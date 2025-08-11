# Docker

Docker is a containerization platform that automates the deployment, scaling, and management of applications inside lightweight, portable containers. It simplifies application distribution by packaging code, dependencies, and runtime into isolated environments, ensuring consistency across different systems.

---

### Images

| Command                            | Description                                         |
| ---------------------------------- | --------------------------------------------------- |
| docker search [image]              | Searches for an image on Docker Hub                 |
| docker pull [image]                | Downloads an image to your machine from Docker Hub  |
| docker images                      | Lists all local images                              |
| docker rmi [image]                 | Removes a local image                               |
| docker build [directory]           | Builds an image from a Dockerfile                   |
| docker build -t [name] [directory] | Builds an image and tags it with a name             |

---

### Containers

| Command                             | Description                                                |
| ----------------------------------- | ---------------------------------------------------------- |
| docker run [image]                  | Runs an image (pulls if not present), creating a container |
| docker run --name [name] [image]    | Runs an image with a specified container name              |
| docker ps -a                        | Lists all containers (running and stopped)                 |
| docker start [container]            | Starts an existing container                               |
| docker stop [container]             | Stops a running container                                  |
| docker rm [container]               | Deletes a container                                        |
| docker inspect [container \| image] | Shows technical details in JSON                            |
| docker logs [container]             | Displays container logs                                    |
| docker exec [container] [command]   | Executes a command inside a running container              |
| docker exec -it [container] bash    | Opens an interactive shell inside a running container      |

---

### Docker Compose

| Command                                  | Description                                                          |
| ---------------------------------------- | -------------------------------------------------------------------- |
| docker-compose up                        | Starts services defined in docker-compose.yml                        |
| docker-compose up -d                     | Starts services in detached mode                                     |
| docker-compose down                      | Stops and removes containers and networks (keeps volumes by default) |
| docker-compose down -v                   | Stops and removes everything including volumes                       |
| docker-compose stop                      | Stops containers without removing them                               |
| docker-compose start                     | Starts stopped containers                                            |
| docker-compose restart                   | Restarts containers                                                  |
| docker-compose build                     | Builds (or rebuilds) local images                                    |
| docker-compose build --no-cache          | Builds images without using cache                                    |
| docker-compose logs                      | Shows logs for all services                                          |
| docker-compose logs -f                   | Follows logs in real time                                            |
| docker-compose ps                        | Shows the status of Compose containers                               |
| docker-compose exec [service] bash       | Accesses the shell of the specified service                          |
| docker-compose run [service] [command]   | Runs a command in a new container based on the service               |
| docker-compose config                    | Validates and prints the interpolated docker-compose.yml             |

---