### Run unicorn rails container
```
$ docker run -d --name unicorn [docker_image]
```

### Run nginx container with link
```
$ docker build -t nginx .
$ docker run -d -p 80:80 --link unicorn:app --name nginx nginx
```
