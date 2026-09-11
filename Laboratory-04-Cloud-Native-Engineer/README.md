# Laboratory 4: The Cloud-Native Engineer

## Mission Overview
This lab covers the shift from traditional VM-based infrastructure to
containerization. Using a KillerCoda Docker-enabled playground, an Nginx web
server was pulled, deployed, and managed through its full lifecycle to
demonstrate container operations to a client evaluating Docker.

## Objectives
- Differentiate between traditional Virtual Machines (VMs) and Containers
- Access a Docker-enabled cloud environment using KillerCoda
- Execute fundamental Docker CLI commands
- Pull, run, manage, and terminate a containerized application (Nginx)
- Create professional technical documentation using Markdown
- Continue developing a well-organized GitHub Cloud Computing Portfolio

## Docker Commands Executed
\`\`\`bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx
\`\`\`

## Skills Learned
- Verifying a Docker installation and checking daemon status
- Pulling images from Docker Hub
- Running containers in detached mode with port mapping
- Managing the full container lifecycle (list, stop, verify, remove)
- Writing structured technical documentation in Markdown

## Challenges Encountered
- Confirming the container was actually reachable required understanding how
  host-to-container port mapping (`-p 8080:80`) works
- Needed to check container status with `docker ps -a` since stopped
  containers don't appear in the default `docker ps` output
