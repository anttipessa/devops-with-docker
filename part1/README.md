# Part 1 Exercises

## 1.1
```
C:\Users\Antti>docker ps -as
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS                     PORTS               NAMES                SIZE
5ccd7091e9ec        nginx               "nginx -g 'daemon of…"   7 minutes ago       Exited (0) 6 minutes ago                       crazy_nobel          0B (virtual 127MB)
bdab3f2debde        nginx               "nginx -g 'daemon of…"   7 minutes ago       Exited (0) 6 minutes ago                       mystifying_edison    0B (virtual 127MB)
a474f3af78a9        nginx               "nginx -g 'daemon of…"   7 minutes ago       Up 7 minutes               80/tcp              romantic_sanderson   2B (virtual 127MB)
```

## 1.2
```
C:\Users\Antti>docker ps -a
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

C:\Users\Antti>docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
```

## 1.3
```
docker run -it devopsdockeruh/pull_exercise
Give me the password: basics
You found the correct password. Secret message is:
"This is the secret message"
```
## 1.4
```
root@cc5dc66dd17c:/usr/app# cat logs.txt
Thu, 30 Apr 2020 11:52:55 GMT
Thu, 30 Apr 2020 11:52:58 GMT
Secret message is:
"Docker is easy"
```

## 1.5
```
docker run -it --name exe1.5 ubuntu:16.04 sh -c 'echo "Website?"; read website; echo "Searching.."; sleep 1; curl http://$website;'
Open a second cmd and type:
docker exec exe1.5 apt-get update
docker exec exe1.5 apt-get install -y curl wget 
Now input the url.
```

## 1.6
Dockerfile in 1.6 folder
```
docker build -t docker-clock .
docker run docker-clock
```

## 1.7

Dockerfile and script in 1.7 folder

```
docker build -t curler .
docker run -it curler
```

## 1.8

Create a empty logs textfile
```
docker run -v %cd%/logs.txt:/usr/app/logs.txt devopsdockeruh/first_volume_exercise
```

## 1.9

```
docker run -p 3000:80 devopsdockeruh/ports_exercise
```
"Ports configured correctly!!" in localhost:3000


## 1.10

Dockerfile in 1.10 folder
```
docker build -t e10 .
docker run -p 5000:5000 e10
```

## 1.11
Dockerfile in 1.11 folder
```
docker build -t e11 .
docker run -p 8000:8000 -v %cd%/logs.txt:/app/logs.txt e11
```

## 1.12

Dockerfiles in 1.12 folder<br>
Frontend:
```
docker build -t front .
docker run -p 5000:5000 front
```
Backend:
```
docker build -t back .
docker run -p 8000:8000 -v %cd%/logs.txt:/app/logs.txt back
```

## 1.13

Dockerfile in 1.13 folder
```
docker build -t spring .
docker run -p 8080:8080 spring
```
Button appears at localhost:8080

## 1.14

Dockerfile in 1.14 folder
```
docker build -t ruby .
docker run -p 3000:3000 ruby
```
Works in localhost:3000

## 1.15

https://hub.docker.com/r/anttipessa/terminal

## 1.16

https://heroku-esim.herokuapp.com/


## 1.17

https://hub.docker.com/r/anttipessa/python

Python interactive shell