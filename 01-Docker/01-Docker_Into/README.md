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
   86  vim 01-Docker_Into/README.md
   87  ls
   88  cd ..
   89  ls
   90  vim /root/.bashrc 
   91  source /root/.bashrc
   92  git add . ;git commit -m "Docker Install" ; git push 
```



```
# Demo 2 
   98  vim /etc/default/docker 
   99  ls
  100  docker ps 
  101  docker ps -a 
  102  docker run -it ubuntu 
  103  docker run -it ubuntu:16.04 
  104  docker ps 
  105  docker ps -a 
  106  docker attach d0302ec2e731
  107  docker start  d0302ec2e731
  108  docker ps 
  109  docker attach  d0302ec2e731
  110  ls
  111  cd 01-Docker/
  112  ls
  113  mkdir 02-Dockerfile 
  114  ls
  115  cd 02-Dockerfile/
  116  ls
  117  mkdir apache 
  118  ls
  119  cd apache/
  120  ls
  121  vim Dockerfile 
  122  ls
  123  s
  124  docker attach  d0302ec2e731
  125  cat Dockerfile 
  126  docker run -it ubuntu:16.04 
  127  docker ps 
  128  docker inspect 44d0eb2aa999
  129  curl 172.17.0.2
  130  docker ps 
  131  ls
  132  docker build -t test-apache:v1 .
  133  docker images 
  134  docker run -d --name apache-1 test-apache:v1
  135  docker run -d --name apache-2 test-apache:v1
  136  docker ps 
  137  docker ps -a
  138  docker logs apache-2
  139  vim Dockerfile 
  140  ls
  141  docker build -t test-apache:v1 .
  142  docker run -d --name apache-3 test-apache:v1
  143  docker ps 
  144  docker run -d --name apache-4 test-apache:v1
  145  docker ps 
  146  docker inspect apache-3
  147  curl 172.17.0.3
  148  curl 172.17.0.4
  149  curl 172.17.0.5
  150  docker ps 
  151  docker inspect 44d0eb2aa999
  152  curl "172.17.0.2"
  153  docker run -it ubuntu:16.04 
  154  docker ps 
  155  docker inspect 740766e3d3df
  156  curl "172.17.0.5"
  157  ls
  158  docker images 
  159  docker ps 
  160  curl 172.17.0.4
  161  ls
  162  cat Dockerfile 
  163  curl 172.17.0.4
  164  ls
  165  vim index.html
  166  ls
  167  vim Dockerfile 
  168  ls
  169  docker build -t test-apache:v2 .
  170  ls
  171  docker images 
  172  docker run -d --name apache-5 test-apache:v2
  173  docker ps 
  174  curl 172.17.0.4
  175  curl 172.17.0.5
  176  curl 172.17.0.6
  177  ls
  178  docker ps 
  179  curl 172.17.0.6
  180  curl 172.17.0.6:80
  181  ls
  182  vim Dockerfile 
  183  ls
  184  vim index.html 
  185  ls
  186  docker build -t test-apache:v3 .
  187  docker images 
  188  docker ps 
  189  docker run -d --name apache-6 test-apache:v3
  190  docker ps 
  191  curl 172.17.0.7
  192  curl 172.17.0.6
  193  curl 172.17.0.4
  194  ls
  195  cd ..
  196  ls
  197  cd ..
  198  ls
  199  cd 01-Docker_Into/
  200  ls
  201  history > README.md 
```
