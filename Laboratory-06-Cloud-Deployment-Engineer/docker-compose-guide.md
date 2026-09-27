# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` section lists the containers needed for the application. In this project, there are two services: `database`, which uses MariaDB, and `app`, which uses Nextcloud. Each service contains the settings needed for its container to run properly.

## How Does the Nextcloud App Find the Database?

The Nextcloud container finds the MariaDB container through the `MYSQL_HOST` setting. The value is set to `database`, which is the name given to the MariaDB service in the Compose file. Docker Compose allows the two containers to communicate using this service name.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is used to create and start a Docker container individually. In the previous laboratory, it was used to run a single container and specify its settings directly in the command.

On the other hand, `docker-compose up -d` uses the `docker-compose.yml` file to start several related containers at the same time. For this project, it starts both the Nextcloud and MariaDB containers and connects them through the Docker network. The `-d` option allows the containers to run in the background while the terminal remains available.
