# Laboratory 07: Cloud Operations Engineer

## Mission Overview

In this laboratory activity, I took the role of a Cloud Operations Engineer (Site Reliability Engineer) at CloudNova Technologies. The mission was to run a baseline health check on a Linux server ahead of a large marketing campaign. I checked the host's resources, deployed a containerized Nginx web server, generated test traffic, and used application logs and real-time container metrics to show that the infrastructure is healthy.

## Objectives

- Use native Linux command-line tools to monitor host CPU, memory, and disk capacity.
- Deploy a web container and track its real-time performance using Docker metrics.
- Generate web traffic and extract application access logs for analysis.
- Translate raw performance data into a readable technical report using Markdown.
- Continue expanding a professional GitHub Cloud Computing Portfolio.

## Monitoring Commands Executed

| Command | Purpose |
|---------|---------|
| `free -h` | Check total, used, and available memory (RAM) |
| `df -h` | Check disk capacity and usage of each file system |
| `top` | View running processes and live CPU load |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy the Nginx container in the background on port 8080 |
| `docker ps` | Confirm the container is running |
| `curl http://localhost:8080` | Simulate normal user visits (HTTP 200) |
| `curl http://localhost:8080/hidden-admin-page` | Simulate a request for a missing page (HTTP 404) |
| `docker logs client-website` | Retrieve the container's application logs |
| `docker stats` / `docker stats --no-stream` | View the container's CPU, memory, and network usage |

## Skills Learned

- Reading host memory, disk, and CPU output to establish a performance baseline.
- Deploying and naming a containerized web server with port mapping.
- Generating HTTP 200 and 404 responses and finding them in application logs.
- Reading Docker metrics (CPU %, memory usage, network I/O) to judge container efficiency.
- Documenting system health and evidence clearly in Markdown and organizing it in a GitHub repository.

## Repository Contents

- `system-baseline-report.md`: host RAM and storage baseline
- `container-observability.md`: 404 log line and container metrics
- `reflection.md`: mission reflection
- `screenshots/`: evidence for each checkpoint
