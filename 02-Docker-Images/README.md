# Docker Images

This repository contains all the necessary and essential docker commands for docker images. Let's check them out.

# Pull an image from docker hub

```bash
docker pull ubuntu
# This command pulls an ubuntu image from the docker hub
```

# Pull an specific version of an image from docker hub

```bash
docker pull ubuntu:22.04
```

# List all the available images

```bash
docker images
```

# Remove specific docker image

```bash
docker rmi ubuntu:22.04 # using image name & a tag
docker rmi [image_id] # using image id
```

# Build a docker image

```bash
docker build -t webapp:v1.0 .
```

# Remove all the images

```bash
docker image prune
```
