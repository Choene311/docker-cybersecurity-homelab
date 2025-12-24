# docker-cloud computing & cybersecurity-homelab
Docker-based cybersecurity homelab using Ubuntu and MySQL
# Docker-based Cybersecurity Homelab

## Overview
This project documents a Docker-based homelab built on Windows to practice Linux administration,
containerization, and basic service deployment in an isolated environment.

The lab simulates a small multi-service setup commonly found in enterprise environments and focuses
on hands-on learning and troubleshooting.

## Technologies Used
- Docker Desktop (Windows)
- Ubuntu Linux container
- MySQL database container
- PowerShell
- Linux CLI tools

## Lab Architecture
Windows Host  
→ Docker Engine  
→ Ubuntu (admin / analyst container)  
→ MySQL (database service)

## Skills Demonstrated
- Docker container lifecycle management (pull, start, stop, attach)
- Linux command-line usage (ls, cat, nano, apt)
- Managing exited and running containers
- Understanding container persistence
- Basic container networking concepts
- Troubleshooting Docker Engine and WSL backend issues

## Troubleshooting Experience
- Recovered from Docker Engine hangs on Windows
- Resolved WSL backend desynchronisation
- Managed interrupted image downloads
- Restarted and reattached exited containers safely

## Project Status
Work in progress – the lab will be expanded with additional services
(e.g. Nginx, security tooling, and Docker Compose).
![Docker Containers](screenshots/Screenshot(2).png)

# Dockerized Cloud Web Application (Azure)

This project demonstrates a cloud-ready, containerized web application using Docker and Microsoft Azure.

The lab simulates how modern cloud services deploy and expose applications securely using containers. It also highlights practical cybersecurity awareness in cloud deployments.

### Project Highlights

- **Containerization**: Deployed an Nginx web server using Docker containers.
- **Cloud Deployment**: Deployed the container to Azure Container Instances (ACI) with a public DNS endpoint.
- **Cybersecurity Awareness**:
  - Applied minimal exposure by only opening required ports (port 80 TCP)
  - Demonstrated safe resource management to avoid unintended charges
  - Documented the deployment process and screenshots for transparency
- **Documentation & Portfolio**: Includes screenshots of the container instance, the deployed web app, and resource group overview.

### Technologies Used

- Docker Desktop
- Nginx (containerized web server)
- Microsoft Azure (ACI, Resource Groups)
- Windows PowerShell
- GitHub (version control & documentation)

### How to Run Locally (Optional)

```bash
docker run -d -p 8080:80 --name cloud-web nginx
