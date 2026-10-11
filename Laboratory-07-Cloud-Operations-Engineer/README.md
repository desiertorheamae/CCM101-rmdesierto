# Laboratory 07: Cloud Operations Engineer

## Mission Overview

This laboratory focuses on monitoring host resources, deploying an Nginx web server in Docker, generating HTTP traffic, analyzing application logs, and checking real-time container metrics.

## Objectives

- Establish a baseline for host memory and disk usage.
- Deploy and test an Nginx container.
- Generate successful HTTP requests and a 404 error.
- Analyze container logs to identify failed requests.
- Monitor CPU and memory consumption.

## Monitoring Commands Executed

- `free -h` – Check memory usage.
- `df -h /` – Check root filesystem capacity.
- `top` – Observe CPU activity and running processes.
- `docker ps` – List running containers.
- `curl` – Generate HTTP requests.
- `docker logs clientwebsite` – Review application logs.
- `docker stats clientwebsite` – Monitor container resources.

## Skills Learned

This laboratory developed my skills in Linux system monitoring, Docker container deployment, HTTP testing, log analysis, and resource monitoring. It also demonstrated how application logs and performance metrics support troubleshooting and service reliability.
