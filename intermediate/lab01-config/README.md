#validate the config is ok
docker-compose config

#make a wrong config and test
change services: to service:
docker-compose config