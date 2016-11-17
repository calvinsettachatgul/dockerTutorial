https://docs.docker.com/engine/tutorials/dockerizing/

run a hello world
docker run ubunto /bin/echo 'hello world'

run an interactive container
docker run -t -i ubuntu /bin/bash

run some linux commands
pwd
ls

start a daemonized hello world
docker run -d ubuntu /bin/sh -c "while true; do echo hello world; sleep 1; done"

docker ps # prints docker processes

look inside the container with docker logs command
docker logs <container name>

docker logs hopeful_goldstine

<stop the container>
docker stop <container name>

docker ps
docker logs
docker stop




