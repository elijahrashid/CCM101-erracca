# Cloud Infrastructure Components

## Checkpoint 3 – Identify Cloud Infrastructure Components

This report identifies the cloud infrastructure components observed in the Linux environment provided by KillerCoda. The components include compute resources, storage resources, networking resources, and the operating system.

## 1. Compute Resources

**Example:** Intel Xeon E312xx (Sandy Bridge, IBRS update) with 1 CPU core.

### Purpose

The compute resource provides the processing power needed to execute programs, run commands, and perform tasks within the Linux environment.

### Importance in Cloud Computing

Compute resources are essential in cloud computing because they allow applications, services, and workloads to run on cloud servers without requiring users to own and maintain physical hardware. Cloud providers can allocate CPU resources based on the requirements of different workloads.

### Relation to the KillerCoda Linux Environment

The KillerCoda environment provides a virtual cloud server with an Intel Xeon E312xx processor and one CPU core. The CPU is used whenever commands and applications are executed in the Linux terminal.

## 2. Storage Resources

**Example:** 20 GB virtual disk (`/dev/vda`).

### Purpose

Storage resources provide space for storing the operating system, applications, configuration files, and user data.

### Importance in Cloud Computing

Storage is important in cloud computing because applications and operating systems need persistent space to store data. Cloud storage also allows resources to be managed and allocated without requiring users to physically maintain storage devices.

### Relation to the KillerCoda Linux Environment

The KillerCoda server has a 20 GB virtual disk named `/dev/vda`. The main partition, `/dev/vda1`, has a capacity of 19 GB and is mounted at `/`. Additional partitions are used for `/boot` and `/boot/efi`.

## 3. Networking Resources

**Example:** IP addresses `172.30.1.2` and `172.17.0.1`.

### Purpose

Networking resources allow the cloud server to communicate with other systems, services, and networks.

### Importance in Cloud Computing

Networking is essential in cloud computing because cloud servers need network connectivity to communicate with users, other servers, applications, and cloud services. IP addresses help identify systems within a network and allow network communication to take place.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux environment has the IP addresses `172.30.1.2` and `172.17.0.1`. These addresses demonstrate that the virtual server is connected to internal networks. The `172.17.0.1` address is commonly associated with a Docker network.

## 4. Operating System

**Example:** Ubuntu 24.04.4 LTS (Noble Numbat).

### Purpose

The operating system manages the computer's hardware and software resources. It provides the environment needed to run applications and execute commands.

### Importance in Cloud Computing

An operating system is important in cloud computing because it provides the software environment in which cloud applications and services operate. It also manages resources such as CPU, memory, storage, processes, and networking.

### Relation to the KillerCoda Linux Environment

The KillerCoda environment uses Ubuntu 24.04.4 LTS with the `6.8.0-138-generic` Linux kernel. Users interact with this operating system through the terminal to manage files, processes, networking, and other system resources.

## Summary

The KillerCoda environment demonstrates the major components of cloud infrastructure. The Intel Xeon CPU provides compute resources, the 20 GB virtual disk provides storage, the IP addresses provide networking resources, and Ubuntu 24.04.4 LTS provides the operating system. Together, these components allow the virtual cloud server to execute workloads and provide a functional Linux computing environment.

