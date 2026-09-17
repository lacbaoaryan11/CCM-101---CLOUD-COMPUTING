# Mission 4 Reflection

Docker containers are faster and easier to set up compared to a Virtual Machine. When using a VM, we need to install and start a complete operating system before we can use an application. This can take several minutes and also uses more RAM and storage. With Docker, we can use an existing image and start a container in only a few seconds. This makes it easier to deploy applications.

Port mapping is needed because the Nginx web server is running inside the container. Nginx uses port `80` inside the container, while we use port `8080` on the host. The command `-p 8080:80` connects the host port `8080` to the container port `80`. Because of this, we can open and test the Nginx server using `http://localhost:8080`.

When we use the `docker rm` command, the container is completely deleted. Any data that was stored only inside that container can also be lost. This means that important data should be stored outside the container if we need to keep it.

Containerization can also improve the way developers and IT teams work together. Developers can put their application and its needed files inside a container. The IT team can then use the same container for testing and deployment. This can make the process easier because the application can work in the same way in different environments.

My GitHub portfolio is also improving as I complete more cloud computing activities. In this laboratory, I learned how to use Docker, run an Nginx web server, manage containers, and use port mapping. I also added my documentation and screenshots to GitHub. This helps show my progress and the new skills I have learned in cloud computing.
