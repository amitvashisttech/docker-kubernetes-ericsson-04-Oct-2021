```
    1  ls
    2  cd 03-DockerVolumes/
    3  ls
    4  docker volume ls 
    5  docker create volume my-vol 
    6  docker volume create my-vol 
    7  docker volume ls 
    8  docker volume inspect my-vol
    9  docker run -it --name volume-test-1 -v my-vol:/app ubuntu:16.04
   10  ls
   11  docker ps 
   12  docker ps -a
   13  docker volume ls 
   14  docker rm volume-test-1
   15  docker ps -a
   16  docker volume ls
   17  cd 
   18  ls
   19  docker run -it --name volume-test-2 -v /var/www/amit ubuntu:16.04
   20  ls
   21  docker ps 
   22  docker run -it --name volume-test-1 -v my-vol:/app:ro ubuntu:16.04
   23  ls
   24  docker ps 
   25  docker kill $(docker ps -qa)
   26  docker rm $(docker ps -qa)
   27  ls
   28  docker volumes ls 
   29  docker volume ls 
   30  docker volume rm f8d1333b7a890e78a3e84e77dd06c9591e5ef9af8d9ca074b944316d86269843
   31  ls
   32  cd docker-kubernetes-ericsson-04-Oct-2021/
   33  ls
   34  cd 01-Docker/03-DockerVolumes/
   35  s
   36  ls
   37  history > README.md

```
