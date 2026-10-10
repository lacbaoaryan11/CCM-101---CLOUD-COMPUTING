# Mission 6: The Cloud Deployment Engineer

**Course:** CCM 101 - Cloud Computing  
**Student:** Aryan Lacbao  
**Section:** BSIT 4-F  
**Institution:** University of Eastern Pangasinan

## Mission Overview

In this laboratory activity, I deployed a multi-tier private cloud storage application using Docker Compose. The application uses Nextcloud as the web application and MariaDB as its database. Both containers are configured through a YAML file, allowing the application stack to be deployed and managed with simple commands.

## Objectives

- Understand two-tier application architecture.
- Learn the structure and purpose of a `docker-compose.yml` file.
- Create a YAML configuration using the nano editor.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Access the Nextcloud setup page through port 8080.
- Document Infrastructure as Code (IaC) and cloud deployment procedures.

## Commands Executed

```bash
docker --version
docker-compose --version
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose config
docker-compose up -d
docker-compose ps
docker-compose logs
docker-compose down
```

## Skills Learned

- Writing and editing YAML configuration files.
- Deploying multiple containers as one application stack.
- Understanding communication between an application and a database.
- Using Docker Compose to start and stop services.
- Troubleshooting container deployment using logs.
- Documenting cloud computing activities using Markdown.

## Screenshots

The deployment evidence is stored in the `screenshots/` folder.

- `compose-deployment.png` — Running containers.
<img width="1917" height="726" alt="image" src="https://github.com/user-attachments/assets/8f832ac2-9b1d-46f4-9943-72de7f335f7c" />

- `nextcloud-web.png` — Nextcloud setup page.
<img width="1912" height="931" alt="image" src="https://github.com/user-attachments/assets/a0269af2-403b-4a9a-ad2b-b677eb70952c" />

- `compose-teardown.png` — Container teardown.
<img width="1917" height="210" alt="image" src="https://github.com/user-attachments/assets/c5dc6415-ab81-4e94-a5b7-713a186dbd7e" />


## Related Documentation

- [Multi-Tier Architecture](multi-tier-architecture.md)
- [Docker Compose Guide](docker-compose-guide.md)
- [Mission Reflection](reflection.md)
