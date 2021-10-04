```

    1  docker version 
    2  git clone https://github.com/amitvashisttech/docker-kubernetes-ericsson-04-Oct-2021.git
    3  ls
    4  docker version 
    5  systemctl status docker
    6  ls
    7  docker images 
    8  ls
    9  cd docker-kubernetes-ericsson-04-Oct-2021/ 
   10  ls
   11  mkdir 01-Docker/00-Setup 
   12  mkdir 01-Docker/00-Setup  -p 
   13  ls
   14  cp -rf /home/vagrant/docker-kubernetes-Ericsson-17-May-2021/01-Docker/00-Setup 01-Docker/
   15  ls
   16  cd 01-Docker/
   17  ls
   18  cd 00-Setup/
   19  ls
   20  cd ..
   21  ls
   22  cd ..
   23  ls
   24  git add . ;git commit -m "Docker Install" ; git push 
   25  cd 
   26  ls
   27  docker images 
   28  docker run busybox echo "Hello World" 
   29  docker images 
   30  docker ps 
   31  docker ps -a
   32  docker run ubuntu:16.04 echo "Hey Ubuntu" 
   33  docker images 
   34  docker container ls 
   35  docker container ls -a 
   36  docker run -it ubuntu:16.04 
   37  docker ps 
   38  docker ps -a
   39  docker start 55fe42756198
   40  docker ps 
   41  docker attach 55fe42756198
   42  ls
   43  docker ps 
   44  docker ps -a
   45  docker kill 55fe42756198
   46  docker start 55fe42756198
   47  docker ps 
   48  docker kill 55fe42756198
   49  docker ps 
   50  docker rm 55fe42756198
   51  docker ps 
   52  docker ps -a
   53  docker run ubuntu:16.04 echo "Hey Ubuntu" 
   54  docker ps 
   55  docker ps -a
   56  docker ps 
   57  docker ps -a
   58  docker ps -aq
   59  docker rm $(docker ps -qa ) 
   60  docker ps -a 
   61  ls
   62  docker run ubuntu:16.04 echo "Hey Ubuntu" 
   63  docker ps -a 
   64  docker run ubuntu:16.04 --name test-1 echo "Hey Ubuntu" 
   65  docker run --name test-2 ubuntu:16.04  echo "Hey Ubuntu" 
   66  docker ps -a 
   67  docker run --name App-1 ubuntu:16.04  echo "Hey Ubuntu" 
   68  docker run --name App-A-1 ubuntu:16.04  echo "Hey Ubuntu" 
   69  docker run --name App-A-2 ubuntu:16.04  echo "Hey Ubuntu" 
   70  docker run --name App-A-3 ubuntu:16.04  echo "Hey Ubuntu" 
   71  docker run --name App-B-1 ubuntu:16.04  echo "Hey Ubuntu" 
   72  docker run --name App-B-2 ubuntu:16.04  echo "Hey Ubuntu" 
   73  docker run --name App-C-1 ubuntu:16.04  echo "Hey Ubuntu" 
   74  docker ps 
   75  docker ps -a
   76  ls
   77  cd docker-kubernetes-ericsson-04-Oct-2021/ 
   78  ls
   79  cd 01-Docker/
   80  ls
   81  mkdir 01-Docker_Into
   82  ls
   83  history 
   84  ls
   85  history > 01-Docker_Into/README.md
```
