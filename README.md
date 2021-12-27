# docker-php-mariadb-phpmyadmin
Docker-Compose file template for Apache 2 + PHP + MariaDB + phpMyAdmin
## Usage
Run containers
> docker-compose up -d
Stop containers
> docker-compose down
Clean unused
> docker system prune -a
## Remarks
- Adapt PHP version and extensions to use in Dockerfile-web
- Remove IP 127.0.0.1 on ports to allow remote access to services (leave 127.0.0.1 to work with an nginx reverse-proxy for instance)
- Logs are located in *log*
- Apache files folder is *web*
- Database files are placed in *mariadb*
- Use *db* as host for mysql connection in php