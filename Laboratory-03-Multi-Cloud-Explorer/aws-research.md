# Amazon Web Services (AWS) — Research

## Brief Overview
Amazon Web Services (AWS) is the cloud computing platform launched by Amazon in 2006. It is the oldest and, by most market-share measures, the largest public cloud provider, offering over 200 fully featured services from data centers worldwide. AWS is widely used across startups, enterprises, and government agencies for hosting applications, storing data, and running large-scale infrastructure without owning physical hardware.

## Global Infrastructure
AWS infrastructure is organized into **Regions** (separate geographic areas, e.g., `us-east-1`, `ap-southeast-1`) and **Availability Zones (AZs)** — isolated data centers within a region (usually 3+ per region) connected by low-latency links. AWS also operates a global network of **Edge Locations** used by its CDN (CloudFront) to cache content closer to end users. As of recent years, AWS has 30+ regions and 90+ availability zones worldwide.

## Cloud Management Console
The **AWS Management Console** is the web-based dashboard for provisioning and monitoring resources. It also offers the **AWS CLI** (command-line interface) and **AWS SDKs** for programmatic access, plus **AWS CloudShell**, a browser-based shell pre-authenticated with your account credentials.

*(Insert screenshot: `screenshots/aws-homepage.png`)*

## Four (4) Core Services
1. **Amazon EC2 (Elastic Compute Cloud)** — Resizable virtual machines (compute instances) for running applications.
2. **Amazon S3 (Simple Storage Service)** — Object storage for files, backups, static websites, and data lakes, with high durability (11 nines).
3. **Amazon RDS (Relational Database Service)** — Managed relational databases (MySQL, PostgreSQL, SQL Server, etc.) with automated backups and scaling.
4. **Amazon VPC (Virtual Private Cloud)** — Networking service to create isolated virtual networks with subnets, route tables, and security groups.

## Three (3) Advantages
1. **Largest service catalog and market maturity** — the broadest range of tools, meaning almost any workload has a matching managed service.
2. **Extensive global infrastructure** — more regions/AZs than most competitors, useful for low-latency, geographically distributed applications.
3. **Strong ecosystem and community** — abundant documentation, third-party integrations, certifications, and a large talent pool familiar with AWS.

## Typical Enterprise Use Cases
- Hosting scalable web and mobile application backends (e-commerce, SaaS platforms).
- Big data processing and analytics pipelines (using services like EMR, Redshift, Glue).
- Disaster recovery and backup storage using S3 and cross-region replication.
- Enterprise migration of on-premises workloads via lift-and-shift or re-architecting to serverless (Lambda).
