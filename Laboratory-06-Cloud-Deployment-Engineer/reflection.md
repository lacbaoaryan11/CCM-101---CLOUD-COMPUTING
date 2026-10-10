# Mission 6 Reflection: The Cloud Deployment Engineer

In this laboratory activity, I learned how Docker Compose can make deploying cloud applications easier and more organized. Instead of starting each container manually and configuring them one by one, I used a `docker-compose.yml` file to define Nextcloud and MariaDB. With one command, I could start the services together. This approach saves time, reduces repeated work, and makes the deployment easier to reproduce.

I also learned that YAML indentation is very important. If I accidentally use a Tab instead of spaces or place a line at the wrong indentation level, Docker Compose may fail to read the configuration. This can prevent the application from starting. Because of this, I realized that I must carefully check the structure of my YAML file before deploying it.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` help configure the application and database. They allow the containers to use matching database settings without manually entering them inside each container. However, I also learned that passwords written directly in a Compose file are not ideal for production because anyone who can access the file may see them. Real deployments should use a safer method for managing sensitive credentials.

Deploying Nextcloud felt rewarding because I was able to create a private cloud storage environment within a few minutes. I understood how the web application and database work together to provide a service. I also practiced checking the running containers, opening the web interface, viewing logs when needed, and shutting down the application properly.

Since Mission 1, my understanding of cloud computing has grown from learning basic concepts to performing practical deployment tasks. I now understand that cloud engineering is not only about running servers or containers. It also involves planning an architecture, configuring services, managing resources, troubleshooting problems, and documenting the process.

Overall, this mission helped me understand Infrastructure as Code and showed me how automation makes cloud deployments more consistent and manageable. These skills will help me in future cloud computing laboratories and real-world IT projects.
