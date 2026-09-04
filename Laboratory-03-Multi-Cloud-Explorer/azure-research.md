# Microsoft Azure — Research

## Brief Overview
Microsoft Azure is Microsoft's public cloud platform, launched in 2010 (originally as "Windows Azure"). Azure is especially strong for organizations already invested in Microsoft products — Windows Server, Active Directory, Microsoft 365, and .NET — because it integrates tightly with them. It is generally considered the second-largest cloud provider by market share after AWS.

## Global Infrastructure
Azure infrastructure is built around **Regions**, grouped into **Geographies** (for data residency/compliance boundaries), with **Availability Zones** providing fault isolation within a region. Azure also has a large number of **Azure Region Pairs** for disaster recovery, and its own global edge network for content delivery (Azure CDN / Azure Front Door). Azure has one of the largest region footprints of any provider, with 60+ announced regions worldwide.

## Cloud Management Console
The **Azure Portal** is the primary web-based dashboard for managing resources. Azure also provides the **Azure CLI**, **Azure PowerShell**, **Azure Cloud Shell** (browser-based), and **Azure Resource Manager (ARM) templates** / **Bicep** for infrastructure-as-code deployments.

*(Insert screenshot: `screenshots/azure-homepage.png`)*

## Four (4) Core Services
1. **Azure Virtual Machines** — On-demand, scalable compute instances (Windows or Linux).
2. **Azure Blob Storage** — Object storage service for unstructured data, similar to AWS S3.
3. **Azure SQL Database** — Fully managed relational database built on Microsoft SQL Server engine.
4. **Azure Active Directory (Microsoft Entra ID)** — Identity and access management service, tightly integrated with Windows Server AD and Microsoft 365.

## Three (3) Advantages
1. **Best-in-class integration with Microsoft products** — seamless connection to Windows Server, Active Directory, Microsoft 365, and .NET applications.
2. **Strong hybrid cloud support** — tools like Azure Arc and Azure Stack let organizations extend on-premises infrastructure into the cloud smoothly.
3. **Enterprise trust and compliance** — widely adopted by large enterprises and government due to Microsoft's long-standing enterprise relationships and compliance certifications.

## Typical Enterprise Use Cases
- Migrating on-premises Windows Server / Active Directory environments to the cloud.
- Hosting .NET and enterprise line-of-business applications.
- Hybrid cloud deployments that mix on-premises and cloud resources.
- Identity and access management for organizations already using Microsoft 365.
