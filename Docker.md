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
 docker build -t myapp:v1 .
```
## Stopping and Starting the containers
```
docker images
docker run --name mycontainer Idimage
docker ps
docker ps -a
docker stop containerID
docker run --name ContainerName -p 3000:3000 -d Idimage
docker run --name ContainerName -p 3000:3000 -d Idimage:v1
docker stop mycontainer
docker start mycon

```

## Managing Image and containers

```
docker image rm imageName
docker image rm imageName -f
docker container rm mycontainer
docker system prune -a

 ```

## Volumes == Directry mapping
```bash
docker run --name myapp_c_nodemon -p 3000:3000 --rm -v C:\Users\yubraj\Desktop\Coding\Docker:/index -v /Docker/node_modules myapp:nodemon

```

## Docker compose
```yaml

version: '3.8'
services:
  api:
    build: ./api
    container_name: api_c
    ports:
      - "4000:4000"
    volumes:
      - ./api:/index
      - ./app/node_modules
```
```
docker system prune
```


  

