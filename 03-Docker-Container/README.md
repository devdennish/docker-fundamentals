# Docker Container

This repository contains all the necessary and essential docker commands for docker containers. Let's check them out.

# List all the running docker containers

```bash
docker ps
```

# List all the docker containers

```bash
docker ps -a
# Flag -a is to list all the container
```

# Run a docker container

```bash
docker run -d --name nginx-webserver -p 3000:80 nginx
# -d flag is to run the container in a detached mode
# --name flag is to name the container
# -p flag is map the docker container port to the host. Nginx runs default on port 80 and it is mapped to port 3000 for the host
```

# Run a docker container in an interactive mode

```bash
docker run -it --name ubuntu-container ubuntu:22.04
# -it flag is to run the container in a interactive mode
```

# Attach an interactive mode to a running container

```bash
docker attach ubuntu-container
```

# Stop a running container

```bash
docker stop nginx-webserver # Stop using container's name
docker stop a6f4 # Stop using container's first four characters.
```

# Remove a docker container

```bash
docker rm nginx-webserver # Remove using container's name
docker rm a6f4 # Remove using container's first four characaters.
```

# Remove all stopped docker containers

```bash
docker container prune
```
