# Docker Volumes

This repository contains all the necessary and essential docker commands for docker volumes. Let's check them out.

# List all the docker volume

```bash
docker volume ls
```

# Create a docker volume

```bash
docker volume create myvolume
```

# Inspect a docker volume

```bash
docker volume inspect myvolume
```

# Remove a volume

```bash
docker volume rm myvolume
```

# Remove unused local volumes

```bash
docker volume prune
```

# Attach a volume to a docker container

```bash
docker run --name ubuntu-container -it -v myvolume:/data ubuntu:22.04
# The volume we created above will be attached to the container in /data directory
```

# Mount a directory as a volume

```bash
docker run --name ubuntu -it -v "$(pwd)":/data ubuntu:22.04
# current working directory will be mounted as a volume.
# Datas are persistent. Any changes made in local directory are reflected on the mounted volume e
```
