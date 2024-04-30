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
