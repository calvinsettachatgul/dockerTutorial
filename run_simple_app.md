https://docs.docker.com/engine/tutorials/usingdocker/

### Learning About the Docker client
docker version 

### Get Docker Help Command
docker --help

### Docker Help on specific command
docker <command> --help

### Run a Web App in Docker
running more containers
run a Python Flask application 

docker run  -d -P training/webapp python app.py
-d daemon
-P run required ports inside container to your host

### Network Port Shortcut
docker port cranky_ptolemy 5000

### View Web Application Logs
docker logs -f cranky_ptolemy

### Inspect the Web App Container
docker inspect <container_name>
inspect the json representation of the processes
request a sepcific element also 

### Stop the Web App Container
docker stop <container_name>

check to see if stopped
docker ps -l

### Restart the Web App Container
docker start <container_name>


### Remove the Web App Container
can't remove a running container
docker stop <container_name>
docker rm <container_name>

now the container is deleted


