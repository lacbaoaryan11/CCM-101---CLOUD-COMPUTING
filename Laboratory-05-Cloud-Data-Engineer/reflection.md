# Mission Reflection

This laboratory activity helped me understand the importance of object storage in cloud computing. Object storage is better suited for storing millions of photos because it is designed to handle large amounts of unstructured data. Photos can be stored as objects inside a bucket, and more files can be added as the application grows. This makes object storage useful for a photo-sharing application because users can upload many images without filling the web server's local storage.

Docker made it easier to deploy the MinIO storage server because I did not need to install every part of the software manually. I only needed to use a Docker command with the image, ports, username, and password. Docker then created the container and ran the MinIO service. This showed me that containers can make software deployment faster and easier.

A bucket is a storage container used to organize objects in object storage. In this activity, I created a bucket named `client-photos`. I then uploaded a sample file into the bucket. The bucket makes it easier to organize files that belong to the photo-sharing application.

Large enterprise companies can protect their object storage data by making backups and copies of their data. They can also store copies in different servers or locations. If one physical server crashes, another copy can still be available. These methods help reduce the chance of permanently losing important data.

My confidence in using the Linux command line is also growing. At first, Docker commands looked difficult because they contained many options. After using commands such as `docker --version`, `docker pull`, `docker run`, and `docker ps`, I became more comfortable with the terminal. I learned how to download an image, create a container, check if it is running, and access a service through a port. This activity gave me useful hands-on experience with Linux, Docker, containers, and cloud storage.
