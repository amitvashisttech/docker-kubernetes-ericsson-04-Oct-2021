```
 35  docker ps 
   36  docker network  ls 
   37  docker network inspect 2d2b8519950e
   38  docker images 
   39  docker run -d --name apache-t-1 test-apache:v3 
   40  docker network inspect 2d2b8519950e
   41  ip addr 
   42  curl  172.17.0.3
   43  ls
   44  docker ps 
   45  curl  172.17.0.3
   46  docker run -d --name apache-t-2 -p 8080:80 test-apache:v3 
   47  docker ps 
   48  curl  172.17.0.3
   49  curl  172.17.0.4
   50  curl localhost:80 
   51  curl localhost:8080
   52  ip addr 
   53  ls
   54  cd docker-kubernetes-ericsson-04-Oct-2021/
   55  ls
   56  cd 01-Docker/
   57  ls
   58  cd 02-Dockerfile/
   59  ls
   60  cd apache/
   61  ls
   62  docker run -d --name apache-t-3 -v ~/docker-kubernetes-ericsson-04-Oct-2021/01-Docker/02-Dockerfile/apache:/var/www/html/amit -p 8081:80 test-apache:v3 
   63  docker ps 
   64  cd ..
   65  ls
   66  cd ..
   67  ls
   68  docker run -d --name apache-t-4 -v ~/docker-kubernetes-ericsson-04-Oct-2021/:/var/www/html/amit -p 8082:80 test-apache:v3 
   69  docker ps 
   70  ls
   71  chmod 777 -R * 
   72  docker ps 
   73  ls
   74  docker ps 
   75  ls
   76  docker ps 
   77  docker network  ls 
   78  systemctl status docker 
   79  netstat -tulnp
   80  docker run -d --name apache-t-5 -p 8080:80 test-apache:v3 
   81  docker run -d --name apache-t-6 -P  test-apache:v3 
   82  docker run -d --name apache-t-7 -P  test-apache:v3 
   83  docker run -d --name apache-t-8 -P  test-apache:v3 
   84  docker ps 
   85  docker network ls 
   86  docker network create --driver --help
   87  docker network create --help
   88  docker network create --driver=bridge --subnet=172.28.0.0/16 --ip-range=172.28.5.0/24 --gateway=172.28.5.254 mybr0 
   89  docker network ls 
   90  docker network inspect mybr0
   91  docker run -d --name apache-t-10 --network mybr0 -P  test-apache:v3 
   92  docker run -d --name apache-t-11 --network mybr0 -P  test-apache:v3 
   93  docker ps 
   94  docker inspect apache-t-11
   95  docker inspect apache-t-10
   96  ip addr 
   97  curl 172.28.5.0 
   98  curl 172.28.5.1
   99  docker ps 
  100  docker network inspect mybr0 
  101  ls
  102  docker ps -a
  103  docker kill $(docker ps -aq)
  104  docker rm $(docker ps -aq)
  105  ls
  106  cd 01-Docker/
  107  ls
  108  cd ..
  109  ls
  110  chmod 755 -R * 
  111  ls
  112  cd 01-Docker/
  113  ls
  114  mkdir 04-DockerNetwork
  115  ls
  116  cd 04-DockerNetwork/
  117  s
  118  ls
  119  docker ps 
  120  docker network ls 
  121  docker network rm mybr0
  122  docker network ls 
  123  ls
  124  history > README.md

```
