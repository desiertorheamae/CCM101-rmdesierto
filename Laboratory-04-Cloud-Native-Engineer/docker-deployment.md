## Container Lifecycle

1. `docker ps`  
   Lists the containers that are currently running, along with their status, ports, and names.

2. `docker stop nginx-server`  
   Stops the Nginx container that is currently running in the background.

3. `docker ps -a`  
   Displays all containers, including stopped ones, to confirm that the Nginx container is no longer running.

4. `docker rm nginx-server`  
   Removes the stopped Nginx container from the Docker environment.
