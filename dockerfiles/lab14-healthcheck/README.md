```
docker image build -t nginx:1.18 .

docker run --name=nginx-proxy -d --health-cmd='stat /etc/nginx/nginx.conf || exit 1' nginx:1.18
docker inspect --format='' nginx-proxy | grep health -C5

docker exec nginx-proxy rm /etc/nginx/nginx.conf
docker inspect --format='' nginx-proxy | grep health -C5

docker exec nginx-proxy touch /etc/nginx/nginx.conf
docker inspect --format='' nginx-proxy | grep health -C5
```