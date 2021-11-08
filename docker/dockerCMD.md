# Basic info docker commands

docker version - version of soft
docker info - info on (images, container ...)

# Run a container in interactive mode (-it) with ports exposed (-p)

docker container run -it -p <localPort>:<containerPort> <imageName>

# Run a container in background (-d) (-it) with ports exposed (-p)

docker container run -d -p <localPort>:<containerPort> --name <customContainerName> <imageName>

# Attach a volume from your machine to your container (-v option)

docker container run -d -p <localPort>:<containerPort> -v <localDir>:<containerDir> <imageName>

# Bash into a running container

docker container exec -it <container_name> bash

# Stop a container

docker container stop <container_id|container_name>

# List of docker container running

docker container ls

docker ps

# List of docker container running or not

docker container ls -a

docker ps -a

# Erase a container

docker container rm <container_id>
docker container rm <container_id> -f (if container is running)

# List images

docker images

# Erase an image

docker image rm nginx

# Pull manually an image

docker pull <imageName>
