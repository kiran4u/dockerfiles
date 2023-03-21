### VOLUMES
Docker continers are ephemeral, when you remove container by default it will delete the data.

# Docker Volumes
/var/lib/docker/volumes

docker volume create [name-of-volume]

# docker run -d -v nginx: -p host-port:continerport -v host-path:container-path 

docker run -d -v nginx:/usr/share/nginx/html -p 80:80 nginx

Inside host you will have a directory for volume.

This directory can be mounted with any path inside the container.

/var/lib/docker/volumes/nginx_data: /usr/share/nginx/html

# mysql
/var/lib/docker/volumes/mysql-data/_data
docker run -d -v mysql-data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=XXX mysql




