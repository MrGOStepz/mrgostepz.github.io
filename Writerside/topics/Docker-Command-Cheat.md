# Docker Command Cheat
```sh
# Run Docker with Image find in local first. if there no in local. Find on the docker hub
docker run <image>

# Run Latest
docker run redis
# Run with Tag
docker run redis:4.0 <-- Tag

# list all container used
docker ps ---all

# list of container
docker ps

# list of running container
docker ps -a

# Execute with Command
docker exec -it <container id> <command>

# Stop Docker
docker stop <NAMES>

# Remove Conntainer
docker ps -a
docker rm <NAMES>

# List of all images
docker images

# Remove Image
docker rmi <NAMES>

# Pull - download an image
#Pull and Run
docker run <IMAGE_NAME>

# Pull Only
docker pull <IMAGE_NAME>

# Append a command
docker run <IMAGE_NAME>
docker run <IMAGE_NAME> sleep 5

# Exec - execute a command
docker ps -a
docer exec <NAME> <COMMAND>

# Run - attach and detach
docker run <NAME>

# Run Docker Background
docker run -d <NAME>

docker attach <FROM_-d>

# If container does not step. Kill them
docker kill

# Clear Docker container
docker system prune

# Run - stdin
docker run -i <CT>
docker run -it <CT>

# Run - PORT mapping
docker run <CT>

docker run -p 80:5000 <CT>
docker run -p 8000:5000 <CT>
docker run -p 80001:5000 <CT>

# RUN - Volumn mapping
docker run mysql
docker run -v /opt/datair:/var/lib/mysql mysql

# Inspect Container
docker inspect <CT>

# Container Logs
docker logs <CT>

# build a Dockerfile
docker build .
```
