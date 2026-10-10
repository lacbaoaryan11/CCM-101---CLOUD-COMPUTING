# Docker Compose Guide

## Introduction

Docker Compose is a tool for defining and managing multi-container applications. It uses a YAML file to describe the services, images, ports, and environment variables needed by an application.

For this mission, Docker Compose is used to deploy Nextcloud and MariaDB together.

## The `services:` Block

The `services:` block defines the containers that make up the application. In our YAML file, there are two services:

- **database:** Uses the `mariadb:10.6` image to provide the database.
- **app:** Uses the `nextcloud` image to provide the web application.

Docker Compose creates and manages the containers based on these definitions.

## Database Configuration

The database service uses environment variables to configure MariaDB.

- `MYSQL_ROOT_PASSWORD` sets the database root password.
- `MYSQL_DATABASE` specifies the database name.
- `MYSQL_USER` specifies the application database username.
- `MYSQL_PASSWORD` specifies that user's password.

These settings configure the database when its data directory is initialized for the first time.

## How Does Nextcloud Find the Database?

The Nextcloud service uses the environment variable:

```yaml
- MYSQL_HOST=database
```

The value `database` matches the name of the database service in the Compose file. Docker Compose provides service-name-based DNS on its application network, allowing Nextcloud to locate MariaDB using that name.

The database and application must also be running and correctly configured for the connection to succeed.

## Port Mapping

The following configuration publishes the application on port 8080:

```yaml
ports:
  - 8080:80
```

Port 8080 on the host is mapped to port 80 inside the Nextcloud container. Users can then access the web interface through the environment's exposed port.

## Docker Run vs. Docker Compose

### Docker Run

The `docker run` command is commonly used to create and start an individual container. When an application requires multiple containers, the engineer may need to configure and manage each one separately.

### Docker Compose

The `docker-compose up -d` command starts the services defined in the Compose file in detached mode. It is useful for multi-container applications because their configuration is kept together in one file.

The `docker-compose down` command stops and removes the Compose-managed containers and network. It does not normally remove named volumes unless the `-v` option is used.

## Commands Used

```bash
docker-compose config
docker-compose up -d
docker-compose ps
docker-compose logs
docker-compose down
```

If the installed environment uses the newer Compose plugin, use `docker compose` instead of `docker-compose`.

## Conclusion

Docker Compose simplifies the deployment of applications that depend on multiple services. By defining Nextcloud and MariaDB in one YAML file, engineers can deploy, inspect, and remove the application stack with fewer manual commands.
