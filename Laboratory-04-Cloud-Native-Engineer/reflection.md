# Mission Reflection

The difference between deploying a Docker container and setting up a
traditional VM is stark. Installing an operating system on a VM involves
downloading an ISO, configuring virtual hardware, walking through an OS
installer, and then installing and configuring the actual web server — a
process that can easily take fifteen minutes or more. Deploying Nginx in
Docker took a single `docker run` command and was live in seconds, because
the container reuses the host's kernel instead of booting its own OS.

Port mapping with `-p 8080:80` is necessary because a container's internal
network is isolated from the host by default. Nginx inside the container
listens on port 80, but that port isn't automatically exposed to the outside
world. The `-p 8080:80` flag creates a bridge so that requests to port 8080
on the host machine are forwarded to port 80 inside the container, which is
why `curl http://localhost:8080` was able to reach the web server.

When `docker rm` is used, any data that existed only inside the container's
writable layer is permanently deleted along with the container. Containers
are meant to be ephemeral — unless data is stored in a mounted volume or
bind mount outside the container, it does not persist once the container is
removed. This is an important distinction from VMs, where the entire disk
image typically persists until explicitly deleted.

Containerization changes how developers and operations teams collaborate by
removing a major source of friction: environment inconsistency. Because a
container image bundles the application with all its dependencies, a
developer can be confident that what runs on their machine will run
identically in staging and production. This shrinks the gap between "it
works for me" and "it works in production," letting Dev and Ops move faster
together and enabling practices like CI/CD pipelines that build, test, and
deploy container images automatically.

My GitHub portfolio is evolving from cloud fundamentals and multi-cloud
comparisons into hands-on, tool-level engineering work. Where earlier labs
focused on conceptual blueprints and provider evaluation, this lab
demonstrates practical command-line skill with Docker, along with the
ability to document technical procedures clearly enough for another
engineer, or a client's IT team, to reproduce the results.
