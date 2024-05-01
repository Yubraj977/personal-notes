## The Docker File
```
FROM node:17-alpine
WORKDIR /app
COPY . .
RUN npm install
EXPOSE 4000
CMD ["node","index.js"]
```

## Build the Docker File
```
 docker build -t myapp .
```
## Stopping and Starting the containers
```
docker images
docker run --name mycontainer Idimage
docker ps
docker ps -a
docker stop containerID
docker run --name ContainerName -p 3000:3000 -d Idimage
docker stop mycontainer
docker start mycon

```
