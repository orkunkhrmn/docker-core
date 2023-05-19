# docker-core

docker build -f .\Dockerfile -t docker-app-proj .

docker run -d -p 80:80 docker-app-proj

ex:int

docker ps --all "show all conteiners"
docker rm <id> "remove container"

docker exec -it <id> bash "connect to container on bash"
