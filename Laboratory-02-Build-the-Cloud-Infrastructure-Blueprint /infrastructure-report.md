# Infrastructure Report

## Checkpoint 2 – Investigate the Cloud Server

This report documents the investigation of the Linux cloud server environment using the KillerCoda terminal.

### 1. Operating System

**Operating System:** Ubuntu 24.04.4 LTS (Noble Numbat)

### 2. Kernel Version

**Kernel Version:** 6.8.0-138-generic

### 3. CPU Model

**CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update)

### 4. Number of CPU Cores

**Number of CPU Cores:** 1

### 5. Total RAM

**Total RAM:** To be determined using the `free -h` command.

### 6. Disk Capacity

**Disk Capacity:** 20 GB

### 7. Mounted File Systems

| File System  | Size |  Used | Available | Mount Point |
| ------------ | ---: | ----: | --------: | ----------- |
| tmpfs        | 191M | 1000K |      190M | `/run`      |
| `/dev/vda1`  |  19G |  5.4G |       13G | `/`         |
| tmpfs        | 952M |   84K |      952M | `/dev/shm`  |
| tmpfs        | 5.0M |     0 |      5.0M | `/run/lock` |
| `/dev/vda16` | 881M |  117M |      703M | `/boot`     |
| `/dev/vda15` | 105M |  6.2M |       99M | `/boot/efi` |

### 8. Hostname

**Hostname:** ubuntu

### 9. IP Address

**IP Addresses:**

* `172.30.1.2`
* `172.17.0.1`

## Commands Used

```bash
cat /etc/os-release
uname -r
lscpu | grep "Model name"
nproc
free -h
lsblk
df -h
hostname
hostname -I
```

## Conclusion

The KillerCoda cloud server was successfully investigated using Linux terminal commands. The server runs Ubuntu 24.04.4 LTS with a 6.8.0-138-generic kernel. It uses an Intel Xeon E312xx processor with one CPU core and a 20 GB virtual disk. The hostname is `ubuntu`, and the detected IP addresses are `172.30.1.2` and `172.17.0.1`.

