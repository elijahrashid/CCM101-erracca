
# Mission 8: The Cloud Security Engineer

## Mission Overview

This laboratory focuses on securing a cloud server using UFW (Uncomplicated Firewall). I deployed an Nginx web application using Docker and configured firewall rules to block incoming connections by default while allowing the necessary services.

## Objectives

- Understand the Principle of Least Privilege and the Attack Surface.
- Deploy and test an Nginx web application.
- Configure UFW with a Default Deny policy.
- Allow SSH access on port 22.
- Allow TCP traffic on port 8080.
- Verify firewall rules and document the security configuration.

## Commands Executed

    docker run -d --name secure-web-app -p 8080:80 nginx
    curl http://localhost:8080
    sudo ufw allow ssh
    sudo ufw default deny incoming
    sudo ufw default allow outgoing
    sudo ufw enable
    sudo ufw status verbose
    sudo ufw allow 8080/tcp
    sudo ufw status numbered

## Skills Learned

- Deploying a web server using Docker.
- Testing web connectivity using curl.
- Configuring a Linux firewall using UFW.
- Applying the Default Deny policy.
- Managing network ports and firewall rules.
- Documenting technical procedures using Markdown.
- Maintaining a GitHub cloud computing portfolio.

