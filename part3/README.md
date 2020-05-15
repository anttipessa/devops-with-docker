# Part 3 Exercises

## 3.1 

Initial size with `node:10`:

```
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
examples_front      latest              ce3dccef02b3        About an hour ago   1.29GB
examples_back       latest              ad0e6c2e0380        About an hour ago   986MB
```

With `ubuntu:16.04`:

```
REPOSITORY          TAG                 IMAGE ID            CREATED              SIZE
examples_front      latest              9f60431ce651        18 seconds ago       479MB
examples_back       latest              ddaa4ff6a19d        About a minute ago   309MB
```

## 3.2 

Dockerfile and the circleci config can be found in 3.2 folder.

https://hub.docker.com/r/anttipessa/heroku-circleci

https://heroku-circleci.herokuapp.com/


## 3.4

Dockerfiles in the 3.4 folder.

## 3.5 

Before:
```
examples_front      latest              6aa30db47805        51 minutes ago      675MB
examples_back       latest              4eae762978c1        57 minutes ago      335MB
```

After using `node:alpine`:

```
examples_front      latest              e3534ae21d73        About a minute ago   508MB
examples_back       latest              525e5a9c6104        5 minutes ago        168MB
```

## 3.6

Dockerfile in the 3.6 folder.

## 3.7
I chose the spring example project, heres the original image:
```
spring              latest              64c5665c99ea        2 minutes ago       596MB
```

With multi-stage build and using `alpine` variant:
```
spring              latest              a69644008494        About a minute ago   121MB
```

## 3.8

![Kubernetes](./3.8/Kubernetes.png)