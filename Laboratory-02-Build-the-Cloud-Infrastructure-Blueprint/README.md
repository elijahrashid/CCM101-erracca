# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

CloudNova Technologies assigned this mission as the first official cloud infrastructure project. The purpose of the laboratory is to investigate the components of cloud infrastructure, understand how compute, storage, networking, and identity services work together, and document the findings as technical documentation.

The laboratory uses a Linux server in the KillerCoda Playground, Linux tools, official cloud documentation, and a GitHub Cloud Computing Portfolio. The overall goal is to prepare an infrastructure assessment and a simple cloud architecture blueprint before cloud services are deployed.

## Objectives

At the end of this laboratory activity, the objectives are to:

- Explain the major components of cloud infrastructure.
- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components

The laboratory focuses on the following major infrastructure components:

### Compute Resource

A compute resource provides processing capability for running applications, services, and workloads. In the cloud infrastructure blueprint, the compute resource represents the server or virtual machine that performs processing tasks.

### Storage Resource

A storage resource provides a location for storing data, files, and other information. Storage is an important part of cloud infrastructure because applications need persistent data storage.

### Network

A network provides connectivity between users and cloud resources. It allows the compute and storage resources to communicate and enables users to access cloud services.

### User

The user represents the person accessing the cloud infrastructure. The user connects to the cloud environment through an Internet connection.

### Internet Connection

The Internet connection provides the communication path between the user and the cloud infrastructure.

### Infrastructure Relationship

The basic relationship represented in the cloud architecture is:

```text
User
  |
  v
Internet Connection
  |
  v
Network
  |
  +------------------+
  |                  |
  v                  v
Compute Resource   Storage Resource
```

## Tools Used

The laboratory activities require and use the following resources and tools:

- KillerCoda Playground
- GitHub Account
- Modern Web Browser
- Stable Internet Connection
- Linux command-line tools
- Markdown
- A diagramming tool such as Draw.io, Excalidraw, Figma, or Microsoft PowerPoint
- PNG format for the cloud architecture diagram

## Linux Commands Executed

The technical investigation was performed using the **KillerCoda Playground**. The following Linux commands were executed to investigate the server environment:

```bash
cat /etc/os-release
uname -r
lscpu | grep "Model name"
nproc
lsblk
df -h
hostname
hostname -I
```

These commands were used to collect information about the operating system, kernel, CPU model, number of CPU cores, disk and mounted file systems, hostname, and IP address.

### Key Findings from the Investigation

- **Operating System:** Ubuntu 24.04.4 LTS (Noble Numbat)
- **Kernel:** 6.8.0-138-generic
- **CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
- **CPU Cores:** 1
- **Disk:** 20 GB virtual disk (`vda`)
- **Root Partition:** 19 GB mounted at `/`
- **Hostname:** `ubuntu`
- **IP Address:** `172.30.1.2` and `172.17.0.1`

## Skills Learned

The laboratory developed the following skills:

- Understanding major cloud infrastructure components.
- Investigating a Linux server running in a cloud environment.
- Identifying compute, storage, networking, and operating-system resources.
- Understanding the relationship between cloud infrastructure components.
- Creating a simple cloud infrastructure diagram.
- Using Linux tools to investigate a cloud environment.
- Creating professional technical documentation using Markdown.
- Organizing and maintaining a structured GitHub Cloud Computing Portfolio.
- Documenting infrastructure findings clearly and professionally.

## Challenges Encountered

One challenge in this laboratory was understanding how different infrastructure components work together as part of a cloud environment. The investigation of the Linux server required identifying the available compute, storage, networking, and operating-system resources.

Another challenge was organizing technical findings into professional documentation and representing the infrastructure clearly in a cloud architecture diagram. The laboratory also required maintaining the GitHub portfolio, taking screenshots as evidence, and committing and pushing work after each checkpoint.

These activities helped reinforce the importance of documenting and justifying infrastructure design decisions before deployment.

## Checkpoint 5 – Cloud Architecture Diagram

The simple cloud infrastructure diagram was created for a fictional company and includes the required components:

- One Compute Resource
- One Storage Resource
- One Network
- One User
- One Internet Connection

The exported diagram is saved as:

```text
screenshots/cloud-architecture.png
```

## Repository Evidence

The laboratory instructions require screenshots as evidence for completed checkpoints and require work to be committed and pushed to GitHub after each checkpoint.
