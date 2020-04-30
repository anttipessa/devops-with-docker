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
