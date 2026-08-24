# Cloud Provider Comparison

## Checkpoint 4 – Research the Major Cloud Providers

This comparison examines the core infrastructure services offered by Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP). Although the providers use different service names, they provide similar infrastructure capabilities for computing, storage, networking, and identity and access management.

## Cloud Infrastructure Service Comparison

| Infrastructure Component                 | AWS                                                                                                                                        | Microsoft Azure                                                                                                                                     | Google Cloud Platform (GCP)                                                                                                     |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| **Compute**                              | **Amazon EC2 (Elastic Compute Cloud)** – Provides scalable virtual servers for running applications and workloads.                         | **Azure Virtual Machines** – Provides on-demand, scalable virtual machines for Windows and Linux workloads.                                         | **Compute Engine** – Provides virtual machines that run on Google's infrastructure.                                             |
| **Storage**                              | **Amazon S3 (Simple Storage Service)** – Provides object storage for storing and retrieving data. AWS also provides EBS for block storage. | **Azure Blob Storage** – Microsoft's object storage solution for large amounts of unstructured data.                                                | **Cloud Storage** – Managed object storage for storing unstructured data using buckets and objects.                             |
| **Networking**                           | **Amazon VPC (Virtual Private Cloud)** – Provides logically isolated virtual networks where AWS resources can be deployed.                 | **Azure Virtual Network (VNet)** – Provides private networking for Azure resources and communication with the internet or on-premises networks.     | **Virtual Private Cloud (VPC)** – Provides networking for Compute Engine VMs, GKE clusters, and other cloud workloads.          |
| **Identity and Access Management (IAM)** | **AWS IAM (Identity and Access Management)** – Controls authentication and authorization through users, roles, and policies.               | **Azure RBAC (Role-Based Access Control)** with **Microsoft Entra ID** – Controls who can access Azure resources and what actions they can perform. | **Google Cloud IAM (Identity and Access Management)** – Uses roles and permissions to control access to Google Cloud resources. |

### Official Documentation

* **AWS:** [AWS Documentation](https://docs.aws.amazon.com/?utm_source=chatgpt.com)
* **Microsoft Azure:** [Microsoft Azure Documentation](https://learn.microsoft.com/en-us/azure/?utm_source=chatgpt.com)
* **Google Cloud:** [Google Cloud Documentation](https://cloud.google.com/docs?utm_source=chatgpt.com)

## Guide Questions

### 1. Which cloud provider offers the broadest range of services? Explain your answer.

AWS is generally recognized as having one of the broadest selections of cloud services, covering computing, storage, networking, databases, analytics, security, AI, and many other areas. Its large service portfolio allows organizations to build different types of applications and infrastructure using services from a single cloud provider.

### 2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?

Microsoft Azure would be a strong recommendation for an organization that primarily uses Microsoft products. Azure integrates closely with Microsoft technologies such as Windows Server, Microsoft Entra ID, Microsoft 365, and other Microsoft enterprise services, making it easier to manage existing Microsoft-based environments.

### 3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?

Google Cloud is widely recognized for its AI, Machine Learning, and Kubernetes capabilities. Google Cloud provides AI-focused infrastructure and accelerators through its Compute Engine offerings, while Google Kubernetes Engine (GKE) provides a managed Kubernetes platform for deploying and managing containerized applications.

### 4. What similarities did you observe among the three cloud providers?

All three cloud providers offer equivalent core infrastructure services for compute, storage, networking, and identity and access management. They also provide scalable, on-demand resources that allow organizations to deploy applications without purchasing and maintaining all of the underlying physical infrastructure.

