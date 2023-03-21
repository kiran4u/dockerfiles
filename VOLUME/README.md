### VOLUMES
Docker continers are ephemeral, when you remove container by default it will delete the data.

# Docker Volumes
/var/lib/docker/volumes

docker volume create [name-of-volume]

# docker run -d -v nginx: -p host-port:continerport -v host-path:container-path 

docker run -d -v nginx:/usr/share/nginx/html -p 80:80 nginx

