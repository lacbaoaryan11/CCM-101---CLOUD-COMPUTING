# Multi-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is an application design that separates an application into two main parts: the web/application tier and the database tier. These tiers work together to provide services to users and manage application data.

In this laboratory activity, Nextcloud is the application tier, while MariaDB is the database tier.

## The Web/Application Tier

The web/application tier handles user requests and displays the application's interface in a web browser. It processes HTTP requests and allows users to interact with the application.

In our deployment, Nextcloud runs inside a Docker container and provides the private cloud storage interface. It communicates with MariaDB when it needs to store or retrieve information.

## The Database Tier

The database tier stores and manages the application's structured data. It can contain user account information, file metadata, settings, and other information required by the application.

In our deployment, MariaDB runs in a separate container. Nextcloud connects to it using the database name, username, password, and hostname defined in the Docker Compose configuration.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, update, and troubleshoot. Each service can be configured and maintained independently, and the architecture makes it easier to scale services when needed. It also keeps the responsibilities of the application and database separate, although security still requires proper network configuration, access controls, and credential management.

## Architecture Summary

**User's Browser → Nextcloud Application → MariaDB Database**

The browser accesses Nextcloud through port 8080, and Nextcloud communicates with the database service using the hostname `database` on Docker's internal network.
