# docker-core

docker build -f .\Dockerfile -t docker-app-proj .
docker run -d -p 8080:80 docker-app-proj

docker build -f .\Dockerfile -t docker-client-app-proj .
docker run -d -p 80:80 docker-client-app-proj

host_port:container_port

docker ps --all "show all conteiners"
docker rm <id> "remove container"

docker exec -it <id> bash "connect to container on bash"

docker exec -it <id> //bin//sh "connect to container on shell"

---

docker-compose build
docker-compose up -d "tüm serviceler ayağa kaldırır" ağer "service_name verirse" sadece o service ayağa kalkar

