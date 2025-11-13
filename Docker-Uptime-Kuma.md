# Docker + Docker Compose Assignment
## Deploying Uptime Kuma on an Arch Linux VM in VMware Workstation
**User:** Jake
**GitHub Account:** jrs7961

---

## Overview
For this assignment, I used Docker and Docker Compose to deploy Uptime Kuma, a self-hosted uptime monitoring dashboard. My host machine is Windows, but the deployment occurs inside my Arch Linux VM running in VMware Workstation. This documentation explains every command and file I created so another student could reproduce the setup.

---

## Steps

1. Install Docker and Docker Compose:
sudo pacman -Syu
sudo pacman -S docker docker-compose
sudo systemctl enable docker.service
sudo systemctl start docker.service
sudo usermod -aG docker Jake

2. Start the container:
docker compose up -d

3. Verify container is running:
docker ps

4. Access Uptime Kuma from Windows:
Open http://<VM-IP>:3001 in a browser, complete setup.

5. Manage the container:
docker compose down
docker compose up -d
docker compose pull
docker compose up -d

6. Project files:
compose.yaml
docker-uptime-kuma.md

7. Publish to GitHub Pages:
Copied these files to my GitHub Page repo, commit, and push.

