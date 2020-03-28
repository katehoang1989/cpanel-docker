Docker
----------
- Apache
- PHP
- MySQL
- phpMyAdmin
- Redis

Build
----------
docker-compose up --build --no-start --remove-orphans

Other commands
----------
- List: docker ps
- Login: docker exec -it <container> /bin/bash
- Start: docker-compose start
- Stop: docker-compose stop
- Stop all: docker stop $(docker ps -a -q)
- Force stop all: docker kill $(docker ps -q)
- Remove all containers: docker rm $(docker ps -a -q)
- Remove all docker images: docker rmi $(docker images -q)
- Purge: docker system prune --all --force --volumes

SSL
----------
sudo openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -keyout local.app.key -out local.app.crt -config local.app.conf

Enjoy!!