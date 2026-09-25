# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview
This lab deploys a two-tier private cloud storage application (Nextcloud 
and MariaDB) using Docker Compose. Instead of manually starting each 
container with separate docker run commands, the entire stack is defined 
in a single docker-compose.yml file and deployed with one command, 
demonstrating the Infrastructure as Code (IaC) approach.

## Objectives
- Explain the concept of a multi-tier application architecture
- Understand the purpose and structure of a docker-compose.yml file
- Use the nano text editor to create configuration files on the Linux 
  command line
- Deploy a multi-container application (Nextcloud + MariaDB) using 
  Docker Compose
- Document deployment procedures and IaC principles using Markdown
- Continue building a professional GitHub Cloud Computing Portfolio

## Commands Executed
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned
- Writing a docker-compose.yml file with multiple linked services
- Understanding how Docker Compose resolves service names for 
  container-to-container communication
- Deploying and tearing down a multi-container stack with a single command
- Documenting Infrastructure as Code (IaC) concepts in Markdown
- Managing project files and configuration in a Linux CLI environment
