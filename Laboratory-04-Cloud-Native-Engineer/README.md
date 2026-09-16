# Laboratory 04: Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I explored the use of containers as an alternative to traditional Virtual Machines (VMs). Using the KillerCoda Playground, I learned the basic concepts of containerization and practiced using Docker commands. I also deployed an Nginx web server in a Docker container and verified that it was working through a local HTTP request.

## Mission Objectives

At the end of this laboratory activity, I was able to:

- Identify the main differences between Virtual Machines and Containers.
- Use a Docker-enabled environment through KillerCoda.
- Perform basic Docker commands using the command line.
- Pull and run an Nginx container.
- Verify a running web server using `curl`.
- Stop and remove a Docker container.
- Document Docker operations using Markdown.
- Add the completed laboratory to my GitHub Cloud Computing Portfolio.

## Skills Learned

- Basic Docker container management
- Using Docker commands through the Linux terminal
- Mapping host ports to container ports using `-p 8080:80`
- Checking a web server using `curl`
- Managing the container lifecycle
- Writing technical documentation using Markdown

## Challenges Encountered

One challenge I encountered was understanding how port mapping works between the host system and the Docker container. I also had to become familiar with the difference between running a container in detached mode and working with it directly through the terminal.

## Docker Commands Executed

The following Docker commands were used during the laboratory activity:

```bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
docker ps
docker stop nginx-server
docker ps -a
docker rm nginx-server
