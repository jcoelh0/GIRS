test locally:

docker-compose up down

test with swarm:

swarm init

docker stack deploy --compose-file docker-compose.yml stack_name

docker stack rm stack_name

debug:

docker ps

docker exec stack_inspircd1.1.wuzkzw7saf3jvjikmsz8kfzbl ...

docker logs stack_inspircd1.1.wuzkzw7saf3jvjikmsz8kfzbl

i.e. docker exec stack_inspircd1.1.wuzkzw7saf3jvjikmsz8kfzbl /conf/links.sh LINK1

docker inspect id_container
