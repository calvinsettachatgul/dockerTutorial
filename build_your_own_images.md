#### https://docs.docker.com/engine/tutorials/dockerimages/

from docker docs

### Listing Images on the Host
docker images
each downloaded from docker hub	
3 pieces of information
	* repo
	* tags for each image
	* image id

visulization tools for images

if you don't specify a variant of the image then you get the latest image
unbuntu:latest
as opposed to
ubuntu:14.04

### Getting a New Image
auto download of image if not on the host 
takes some time to launch container

pre-load an image you can use the 
docker pull
command

download centos image

docker pull centos
then each layer of the image has been pulled down
can run and not have to wait to download

docker run -t -i centos /bin/bash

-t --tty allocate a pseudo-TTY
-i interactive ( keep STDIN open even if not attached)

### Finding Images
uploaded already to Docker Hub
search

official repositories
redis
ubuntu
wordpress

search for terms sinatra
by stars
image name, description

official repos are carefully curated

Automated repositories
automated builds that allow you to validate source and content of the image

decided to use 
training/sinatra

2 types of image repository names

ubuntu base or root image

training/sinatra
user images belongs to a member of the Docker community built and maintained by them
identified with the user name prefix
in this case training user that created them

### Pulling your Image
docker pull training/sinatra

use the image by running them in their own containers
docker run -i -t training/sinatra /bin/bash

update ruby

apt-get install -y ruby2.0-dev	ruby2.0

install json gem
gem2.0 install json

make a docker commit
docker commit -m "added json gem" -a "Calvin Settachatgul" \
<container_id> ouruser/sinatra:v2

2 flags -m and -a
commit message and the author

### Build Docker Image from Dockerfile
docker file with set of instructions that tell Docker how to build image
create directory and Dockerfile
mkdir sinatra
cd sinatra
touch Dockerfile

instruction statement



