# mariadb
[![Docker Stars](https://img.shields.io/docker/stars/takeyamajp/mariadb.svg?style=flat-square)](https://hub.docker.com/r/takeyamajp/mariadb/)
[![Docker Pulls](https://img.shields.io/docker/pulls/takeyamajp/mariadb.svg?style=flat-square)](https://hub.docker.com/r/takeyamajp/mariadb/)
[![license](https://img.shields.io/github/license/u6k/plantuml-image-generator.svg)](https://github.com/u6k/plantuml-image-generator/blob/master/LICENSE)

FROM mariadb  
MAINTAINER "Hiroki Takeyama"

ENV TZ Asia/Tokyo

ENV MYSQL_CHARSET utf8mb4  
ENV MYSQL_COLLATION utf8mb4_general_ci

ENV MYSQL_ROOT_PASSWORD root  
ENV MYSQL_DATABASE db  
ENV MYSQL_USER user  
ENV MYSQL_PASSWORD user

VOLUME /var/lib/mysql

EXPOSE 3306
