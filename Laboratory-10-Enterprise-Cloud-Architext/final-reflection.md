1. Executive Summary & Project Overview

During Laboratory 10, the main goal was to design, set up, secure, and automate a private cloud web application on an Ubuntu Server. This final project combines key skills in server setup, Docker containers, network firewall security, and daily backup automation to build a solid foundation for enterprise cloud systems.

2. Key Technical Achievements & Implementation Details

Container Setup: Built a two-tier app using Docker Compose. Separated the Nextcloud web app (cloudnova-nextcloud) from the MariaDB database (cloudnova-database) so each runs independently and securely on its own network layer.

Data Storage: Created two Docker volumes (cloudnova_cloud_data and cloudnova_db_data) to make sure all user files, system settings, and database records remain safe even if containers are restarted or updated.

Firewall & Security: Secured the system using UFW (Uncomplicated Firewall). Set the firewall to block all incoming traffic by default, only allowing SSH access on port 22 and web traffic on port 8080.

Automated Backups: Wrote a simple Bash script (automation-script.sh) that exports the MariaDB database and compresses Nextcloud files into dated archive files. Set up a daily Cron job to run this backup automatically every night at 2:00 AM.

3. Challenges Addressed & Troubleshooting Insights

Fixing Database Startup Errors: Fixed an issue where the MariaDB container showed up as "unhealthy" on startup. Updated docker-compose.yml to give the database 30 seconds to start up fully before checking its health status.

Container Communication: Solved database connection issues by using Docker's internal hostnames (db:3306), letting Nextcloud talk directly to MariaDB without relying on changing IP addresses.

Correct File Paths: Used exact file paths (/opt/cloudnova/backups/) in the backup script and Cron schedule to prevent silent errors and keep clear backup logs in backup.log.

4. Conclusion & Readiness for Lab Defense

This project demonstrates practical experience in building and managing secure, containerized server environments. The final setup is fully tested, secure, and automated, satisfying all client requirements for the CloudNova deployment for CEO Joneth Costales.
