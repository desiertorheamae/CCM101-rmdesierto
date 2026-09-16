# Docker Container Lifecycle Documentation

## Lifecycle Commands and Descriptions

1. `docker run -d --name nginx-server -p 8080:80 nginx`
    - Created and started an Nginx container named `nginx-server` in detached mode. Port 8080 on the host was mapped to port 80 inside the container.

2. `docker ps`
    - Displayed the running Nginx container and confirmed that it was active with port 8080 mapped to port 80.

3. `docker stop nginx-server`
    - Stopped the running Nginx container successfully.

4. `docker ps`
    - Confirmed that there were no running containers after stopping `nginx-server`.

5. `docker ps -a`
    - Displayed all containers, including the stopped Nginx container, which appeared with an `Exited (0)` status.

6. `docker rm nginx-server`
    - Removed the stopped Nginx container from the Docker environment.

7. `docker ps -a`
    - Confirmed that the Nginx container had been completely removed and no containers remained.
