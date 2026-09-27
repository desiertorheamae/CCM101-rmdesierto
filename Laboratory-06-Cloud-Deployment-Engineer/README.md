# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory focused on deploying a private cloud storage system using Docker Compose. The system consisted of a Nextcloud web application and a MariaDB database. The two services were configured separately and connected to work together as a two-tier application.

## Objectives

* Understand the basic concept of a two-tier application architecture.
* Create a Docker Compose configuration using YAML.
* Deploy Nextcloud and MariaDB in separate containers.
* Use Docker Compose to manage multiple containers.
* Access the Nextcloud web interface through port 8080.
* Understand how Infrastructure as Code can be used to organize and simplify deployment.

## Commands Executed

The following commands were used during the laboratory activity:

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

This laboratory helped me learn how to create and use a Docker Compose file for a multi-container application. I also learned how the Nextcloud application communicates with the MariaDB database through Docker networking. In addition, I gained a better understanding of how Infrastructure as Code can make the deployment process more organized and easier to repeat.
