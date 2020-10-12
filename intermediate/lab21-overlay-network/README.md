```
docker network create --driver=overlay --subnet=192.168.1.0/24 --gateway=192.168.1.100 myoverlay0
OR
docker network create -d overlay --opt encrypted encrypted_overlay

docker network inspect myoverlay0
```