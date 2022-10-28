# Docker-Cheat-Sheet
## Docker is a containerization technology. 
Docker is a set of PAAS(Platform as a service)products which use OS-level virtualization to deliver software in packages called containers.
Docker containers are lightweight standard unit software, which contain all its dependencies and enable applications to run quickly in one go.

## Dockerfile
Dockerfile is a text file which contains all instructions and commands to build a docker image. To build an image we use docker build command so that several commands and instructions are in succession.


## Docker-Compose
Docker-compose is a YAML file, used to write configurations to run multiple containers in one go. In Docker-Compose a single command is used to run multiple services, i-e to start multiple services and can run the whole app in one go. Most famous command to start and run services,
#### docker-compose up


## Docker Commands

docker ps     => show all docker running container instances<br> 
docker ps -a  => will show all containers available on machine<br> 
docker pull   => used to pull docker images<br> 
docker images => will show all images downloaded on machine<br> 
docker rm     => is used for removing images<br> 
docker rm -f  => used for removing running docker containers<br> 
docker rmi    => used to remove docker image<br> 
docker restart=> used to restart docker container<br> 
docker system prune   => is used for removing stopped containers, all networks not used, all dangling images<br> 
docker image prune    => used for removing dangling images<br> 
docker stop           => used for stopping docker container<br> 
docker start          => used to start a docker container<br> 
docker logs           => to see logs of running container<br> 
docker logs -f        => used to see logs continuously<br> 
docker volume create  => used to create volumedocker volume ls => to see volume used by containers<br> 
docker volume inspect vol_Name => to see details of volume<br> 
docker ps --size      => to check the size of docker containers<br> 
docker ps -aq         =>list all containers id<br> 
docker rm -v          => used to remove container volume<br> 
e.g                   => docker run -v volName:/var/lib <br> 
 >     -p    => used for assigning port -p 8080:80<br> 
 >     -d    => usd to run a container in detached mode<br> 
 >     -exec => used to attach with a running container<br> 
 >     --rm  => if you use this while run while running container then it will delete/remove container right after when it got executed<br> 
>      ctrl+p+q => used to detach from a running container cli<br> 
>      docker cp db.sql 40e7e1697192:/ to copy from local to docker container<br> 

##Docker-Compose Commands
docker-compose up     => used for starting services from scratch<br> 
docker-compose up -d  => used for starting services in detached mode<br> 
docker-compose start  => used for starting composer services(existing services)<br> 
docker-compose down   => used to stop services and removing containers<br> 
docker-compose stop   => used for stopping services without removing them(containers, volume, networks)<br> 
docker-compose ps     => used to see running processes of docker compose<br> 
docker-compose config => used for checking the validity of docker-compose<br> 
docker-compose pause  => pausing running services<br> 
docker-compose unpause=> used for unpausing paused services<br> 
docker-compose up -d --scale serviceName=2,3,4 => for scaling a service<br> 
docker-compose top    => used for giving docker services pid, user, and time<br> 
docker-compose restart=> used to restart services<br> 
>      build           => build or rebuild services bundle <br> 
>      exec            => execute a command in running container<br> 
>      images          => give list of images<br> 
