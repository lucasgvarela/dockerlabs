```
docker-compose exec --index=1 webserver  sh -c "echo 'Welcome to webserver1' > /usr/share/nginx/html/index.html"
docker-compose exec --index=2 webserver  sh -c "echo 'This is webserver2' > /usr/share/nginx/html/index.html"
docker-compose exec --index=3 webserver  sh -c "echo 'Webserver3 is up' > /usr/share/nginx/html/index.html"
while true; do curl http://localhost; sleep 2; done
```