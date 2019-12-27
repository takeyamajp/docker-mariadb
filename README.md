# mariadb
[![Docker Stars](https://img.shields.io/docker/stars/takeyamajp/mariadb.svg)](https://hub.docker.com/r/takeyamajp/mariadb/)
[![Docker Pulls](https://img.shields.io/docker/pulls/takeyamajp/mariadb.svg)](https://hub.docker.com/r/takeyamajp/mariadb/)
[![license](https://img.shields.io/github/license/takeyamajp/docker-mariadb.svg)](https://github.com/takeyamajp/docker-mariadb/blob/master/LICENSE)

### Supported tags and respective Dockerfile links  
- [`latest`, `mariadb10`](https://github.com/takeyamajp/docker-mariadb/blob/master/mariadb10/Dockerfile)

### Image summary
    FROM mariadb:10  
    MAINTAINER "Hiroki Takeyama"
    
    ENV TZ Asia/Tokyo
    
    ENV MYSQL_CHARSET utf8mb4  
    ENV MYSQL_COLLATION utf8mb4_general_ci
    
    ENV MYSQL_ROOT_PASSWORD password  
    ENV MYSQL_DATABASE db  
    ENV MYSQL_USER user  
    ENV MYSQL_PASSWORD password
    
    VOLUME /mysql
    
    EXPOSE 3306
