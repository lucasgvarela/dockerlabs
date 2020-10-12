```
Creating a bridge network
docker network create --driver=bridge --subnet=192.168.1.0/24 --gateway=192.168.1.250 my_bridge

Running a nginx server in user defined network
docker container run -d --rm --name usr_ntwrk --network my_bridge nginx:alpine
```