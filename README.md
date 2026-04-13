# Containerized Application Deployment with Docker Compose

## Overview
This project deploys a simple containerized web application on a Linux VM using Docker Compose, with Nginx acting as a reverse proxy in front of the app container.

## Tools Used
- Docker
- Docker Compose
- Nginx
- Ubuntu Linux
- Azure VM

## Architecture
Browser → Nginx Container → App Container

## Project Structure
docker-project/
├── app/
│   ├── index.html
│   └── Dockerfile
├── nginx/
│   └── default.conf
└── docker-compose.yml

## What It Does
- Builds a custom app image from a Dockerfile
- Runs the app container
- Runs an Nginx reverse proxy container
- Forwards browser traffic from Nginx to the app
- Supports rebuild and redeploy after updates

## Key Command
```bash
docker compose up -d --build
Project screenshots will be added to the 'screenshots/' folder.
