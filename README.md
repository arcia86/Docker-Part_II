# Docker-Part_II
Deploy nginx container using docker-compose/Dockerfile   

## Getting Started

I ran this code in a Mac-OS. with docker installed. 

### Prerequisites

Docker 

## Running the tests

Initial docker containers repository for test. just run 

```
docker-compose up -d
```


### verifying container is running

Open the browser url= localhost:8080

stop it
```
docker stop app
```

### additional commands

start it
```
docker start 
```
search in docker hub filter start five 
```
docker search --filter=start=3 nginx
```
Run nginx with run commands mapping port 5000 and mapping volumen pwd to /usr/share/nginx/html/
```
docker run -d -p 5000:80 --name=webserver -v "$PWD":/usr/share/nginx/html/ nginx
```
