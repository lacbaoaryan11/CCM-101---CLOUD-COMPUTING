# Laboratory Activity 04: The Cloud-Native Engineer

**Course:** CCM 101 - Cloud Computing Architecture & System Administration  
**Author:** Aryan Lacbao  
**Section:** BSIT 4-F  
**Institution:** University of Eastern Pangasinan

---

## Mission Overview

This laboratory activity introduces cloud-native containerization principles by transitioning from traditional Virtual Machine (VM) infrastructure to lightweight container deployments using Docker on the KillerCoda platform.

In this activity, I researched the differences between Virtual Machines and Containers, verified the Docker environment, deployed an Nginx web server using Docker, tested the server using a local HTTP request, and practiced basic container lifecycle management.

## Objectives

- Differentiate the architecture, performance, and resource utilization between Virtual Machines and Containers.
- Access and navigate a Docker-enabled cloud playground environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull, deploy, test, and manage an Nginx containerized web server.
- Create structured technical documentation using Markdown.
- Continue developing an organized GitHub Cloud Computing Portfolio.

---

## Technical Reports & Documents

- **VMs vs. Containers:** [virtualization-vs-containers.md](virtualization-vs-containers.md)
- **Docker Deployment & Lifecycle:** [docker-deployment.md](docker-deployment.md)
- **Mission Reflection:** [reflection.md](reflection.md)

---

## Docker Commands Executed

### 1. Environment Verification

- `docker --version` — Displayed the installed Docker version.
- `docker info` — Verified the Docker environment and confirmed that Docker was running.

### 2. Deployment & Testing

- `docker pull nginx` — Downloaded the official Nginx container image from Docker Hub.
- `docker run -d --name nginx-server -p 8080:80 nginx` — Deployed an Nginx container in detached mode and mapped host port `8080` to container port `80`.
- `docker ps` — Listed the active running containers.
- `curl http://localhost:8080` — Verified that the Nginx web server was accessible and running successfully.

### 3. Lifecycle Operations

- `docker stop nginx-server` — Stopped the running Nginx container.
- `docker ps -a` — Listed all containers, including stopped containers.
- `docker rm nginx-server` — Permanently removed the Nginx container.
- `docker ps -a` — Verified that the removed container no longer appeared.

---

## Evidence Screenshots

The command output screenshots are stored inside the `screenshots/` directory:

- **Docker Verification:** `screenshots/docker-version.png`
- **Nginx Deployment:** `screenshots/nginx-running.png`
- **Container Lifecycle:** `screenshots/container-lifecycle.png`

---

## Skills Learned

- Basic Docker Command Line Interface operations.
- Understanding the differences between Virtual Machines and Containers.
- Pulling and managing Docker images.
- Deploying an Nginx web server using Docker.
- Understanding host-to-container port mapping.
- Managing container lifecycle operations.
- Using Linux terminal commands.
- Writing technical documentation using Markdown.
- Organizing and maintaining a GitHub Cloud Computing Portfolio.

## Challenges Encountered

One challenge I encountered was understanding the difference between a Docker image and a Docker container. I learned that an image is a template used to create containers, while a container is an instance created from that image. Another challenge was understanding port mapping, particularly the meaning of `8080:80`. After testing the Nginx server using curl, I understood that port `8080` on the host connects to port `80` inside the container.
