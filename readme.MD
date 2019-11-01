Docker:


src/index.php

```
<?php

echo "Hello World";
```


Dockerfile

```
FROM php:7.0-apache
COPY src/ /var/www/html
EXPOSE 80
```
#build

`$ docker build -t hello-world .`

#run container port host:container

`$ docker run -p 80:80 hello-world`


#volumes

`$ docker run -p 80:80 -v /Users/langelhc/Documents/docker/src:/var/www/html/ hello-world` 



Docker-Compose:

