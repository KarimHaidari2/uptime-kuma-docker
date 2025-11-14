📘 Uptime Kuma – Docker Compose Project

CYB 3353 – Karim Haidari

📌 Overview

This repository contains a functional Docker Compose setup for Uptime Kuma, a self-hosted monitoring tool that provides uptime checks, response tracking, notifications, and dashboards.

The project demonstrates the ability to:
✔ Install & use Docker on macOS
✔ Write a working docker-compose.yml
✔ Pull and run images from Docker Hub
✔ Manage containers and volumes
✔ Access the service via browser (localhost:3001)
✔ Configure monitors inside Uptime Kuma
✔ Push the project to GitHub using Git commands

 How to Run This Project
1. Clone the Repository
git clone https://github.com/KarimHaidari2/uptime-kuma-docker.git
cd uptime-kuma-docker

2. Start Uptime Kuma
docker compose up -d

3. Access the Dashboard

Open your web browser and go to:

 http://localhost:3001

You will see the Uptime Kuma setup page.

 docker-compose.yml Used in This Project
version: "3.9"

services:
  uptime-kuma:
    image: louislam/uptime-kuma:latest
    container_name: uptime-kuma
    ports:
      - "3001:3001"
    volumes:
      - uptime-kuma-data:/app/data
    restart: always

volumes:
  uptime-kuma-data:

 Features Configured

Inside Uptime Kuma, I completed the following:

✔ Created Admin Account
✔ Added a monitor (Google.com)

HTTP(s) monitor type

60-second interval

Status shows UP

Response times displayed

Uptime history logged

✔ Verified Container in Docker Desktop

Correct image

Container running

Volume created

Port mapped correctly

Logs showing activity

Project Files
File	Description
docker-compose.yml	Main configuration file for running Uptime Kuma
(Screenshots available in Word report)	

 Author

Karim Haidari
University of Tulsa – CYB 3353
Docker Project: Uptime Kuma Deployment

