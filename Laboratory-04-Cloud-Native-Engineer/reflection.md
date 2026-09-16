Mission Reflection

Docker containers are faster and simpler to start compared with traditional Virtual Machines. A VM requires a complete operating system and virtual hardware, while containers share the host system's kernel. Because of this, an Nginx container can be created and started within a few seconds without installing a separate operating system.

I also learned how port mapping works using -p 8080:80. This connects port 8080 of the host system to port 80 inside the Nginx container. It allowed me to access the web server through http://localhost:8080 and verify that the deployment was working.

The container lifecycle commands helped me understand how Docker manages applications. I was able to start the Nginx container, check its status, stop it, and remove it completely. I also learned that data stored only inside a removed container will not remain unless it is saved using a volume or bind mount.

This activity also showed me how containers can support a DevOps workflow. Applications and their required dependencies can be packaged together in a container, making them easier to move and deploy across different environments.

Overall, the activity gave me practical experience with Docker and container management. It also helped me understand how cloud-native technologies can be used for faster and more consistent application deployment.
