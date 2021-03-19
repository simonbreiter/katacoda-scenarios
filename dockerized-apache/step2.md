To see what is going on in your container you can run

`docker logs my-apache-php-app`{{execute}}

The `-f` follows the log and prevents it from closing. This is usefull if you want to monitor something continous.

You can stop your container

`docker stop my-apache-php-app`{{execute}}

and start them again.

`docker start my-apache-php-app`{{execute}}

If you want to get rid of a container run

`docker stop my-apache-php-app; docker rm my-apache-php-app`{{execute}}

This will delete your container and everything in it! Docker containers are considered ephemeral and can be deleted and created again any time. If you want to keep persistent data you need to store it outside the container (e.g. volumes).


