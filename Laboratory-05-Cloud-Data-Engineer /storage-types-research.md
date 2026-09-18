# Storage Types Research

**Laboratory Activity 5 — Mission 5: The Cloud Data Engineer**
**CCM101 – Cloud Computing**

## Comparison of Cloud Storage Types

| Storage Type | Description (How does it store data?) | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Data is split into fixed-size blocks, each with a unique address but no descriptive metadata. The operating system attaches the volume and applies its own filesystem on top, so the OS is what decides where files begin and end. | Low-latency, high-performance workloads that need constant reading and writing: operating system boot volumes, virtual machine disks, and transactional databases. | AWS EBS (Elastic Block Store) — also Azure Managed Disks, Google Persistent Disk |
| **File Storage** | Data is stored as files arranged in a hierarchy of directories and subdirectories. It is accessed by file path over a network using protocols such as NFS or SMB, the same way a shared network drive works. | Shared access to the same set of files by multiple users or servers at once: department file shares, home directories, and content management systems. | AWS EFS (Elastic File System) — also Azure Files, Google Filestore |
| **Object Storage** | Each item is stored as a self-contained object containing the data, extensive metadata, and a unique identifier, all held in a flat namespace rather than a folder tree. Objects are accessed over HTTP through an API instead of being mounted as a drive. | Storing massive volumes of unstructured data that is written once and read many times: images, videos, backups, logs, and static website assets. | AWS S3 (Simple Storage Service) — also Azure Blob Storage, Google Cloud Storage |

## Recommendation to the Client

For a photo-sharing application holding millions of user-uploaded images, Object Storage is the right choice. It uses a flat namespace that scales to virtually unlimited numbers of objects, so it will not run into the directory and volume size limits that a block or file system eventually hits, and its cost per gigabyte is significantly lower at that scale. Each image is also reachable through its own HTTP URL, which means photos can be served directly to browsers or through a CDN without routing every request through the application server, and the metadata stored alongside each object can carry details such as the uploader, upload date, and image dimensions.
