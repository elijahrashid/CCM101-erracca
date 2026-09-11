# Docker Deployment Log

## Verification Commands
| Command | Explanation |
|---|---|
| `docker --version` | Displays the installed Docker version to confirm Docker is present. |
| `docker info` | Shows detailed status of the Docker daemon, including running/stopped container counts and system resources. |

## Deployment Commands
| Command | Explanation |
|---|---|
| `docker pull nginx` | Downloads the official Nginx image from Docker Hub to the local machine. |
| `docker run -d -p 8080:80 --name my-nginx nginx` | Runs a new container from the Nginx image in detached mode, mapping host port 8080 to the container's port 80. |
| `curl http://localhost:8080` | Sends an HTTP request to the mapped port to confirm the Nginx web server is responding. |

## Lifecycle Commands
| Command | Explanation |
|---|---|
| `docker ps` | Lists all currently running containers. |
| `docker stop my-nginx` | Gracefully stops the running `my-nginx` container. |
| `docker ps -a` | Lists all containers, including stopped ones, to confirm the container has stopped. |
| `docker rm my-nginx` | Permanently deletes the stopped container and its writable layer. |
