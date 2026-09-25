# Docker Compose Guide

## What does the `services:` block do?
The `services:` block defines the containers that Docker Compose will create 
and run, such as the `app` and `database` services. Each service specifies 
which image to use and how it should be configured.

## How did the Nextcloud app container know how to find the database container?
The `app` finds the `database` using the `MYSQL_HOST` environment variable, 
which points to the service name `database`. Docker Compose allows containers 
in the same stack to communicate using their service names as hostnames.

## `docker run` vs `docker-compose up -d`
`docker run` starts one container at a time with commands and options 
provided manually. `docker-compose up -d` starts all the services defined 
in the Compose file together and runs them in the background, handling 
networking between them automatically.
