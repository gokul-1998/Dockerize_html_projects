# Dockerize_html_projects

This repo will help you to dockerize your html projects.

## Steps to follow

1) in your html project folder create a file named Dockerfile
2) copy the following code in the Dockerfile

```
FROM nginx:alpine
COPY . /usr/share/nginx/html
```

3) open terminal and run the following commands

```
docker build -t <image_name> .
docker run -d -p 8080:80 <image_name>
```

4) open your browser and type localhost:8080

## Steps to follow if you want to use docker-compose

1) in your html project folder create a file named Dockerfile
2) copy the following code in the Dockerfile

```
FROM nginx:alpine
COPY . /usr/share/nginx/html
```

3) in your html project folder create a file named docker-compose.yml
4) copy the following code in the docker-compose.yml

```
version: '3'
services:
  web:
    build: .
    ports:
      - "8080:80"
```

5) open terminal and run the following commands

```
docker-compose build
docker-compose up
```

6) open your browser and type localhost:8080

## Steps to follow if you want to use this repo




1. Clone this repo
2. Copy your html project in the cloned repo
3. Open terminal and run the following commands

```
docker build -t <image_name> .
docker run -d -p 8080:80 <image_name>
```

4) open your browser and type localhost:8080

## Steps to follow if you want to use docker-compose and this repo

1. Clone this repo
2. Copy your html project in the cloned repo
3. Open terminal and run the following commands

```
docker-compose build
docker-compose up
```

4) open your browser and type localhost:8080
```

