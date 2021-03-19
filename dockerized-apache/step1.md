To run a prebuilt image run

`docker run -d -p 8080:80 --name my-apache-php-app -v "$PWD/src:/var/www/html" php:7.2-apache`{{execute}}

This will start a apache server on port [8080](https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katacoda.com) and mounts the content of your local `src` folder to the container.

To view your running container

`docker ps`{{execute}}
