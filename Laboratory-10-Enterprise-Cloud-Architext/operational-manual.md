# Operational & Disaster Recovery Manual

## 1. Stack Deployment & Configuration
1. Clone the repository into `/opt/cloudnova`.
2. Configure `.env` with database and administrator secrets.
3. Start the containers:
   ```bash
   sudo docker compose up -d
2. Security Configuration
UFW Status: Default Deny incoming, Allow outgoing.

Open Ports: Port 22/tcp explicitly permitted for SSH.

Firewall Command:

Bash
sudo ufw status verbose
3. Maintenance & Disaster Recovery
Manual Backup: Run sudo /opt/cloudnova/automation-script.sh.

Automated Schedule: Configured in root crontab (0 2 * * *).

Database Restoration:

Bash
sudo docker exec -i cloudnova-database mariadb -u root -p"$MYSQL_ROOT_PASSWORD" nextc
