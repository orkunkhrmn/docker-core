#stage 1
FROM node:latest as node
WORKDIR /app

EXPOSE 80

#docker-compose ile build edildiği için böyle. eğer docker ile build edilecekse . . yazılmalı
COPY . . 
RUN npm install
RUN npm run build --prod
#stage 2
FROM nginx:alpine
COPY --from=node /app/dist/docker-app /usr/share/nginx/html