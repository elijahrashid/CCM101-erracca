# Google Cloud Platform (GCP) — Research

## Brief Overview
Google Cloud Platform (GCP) is Google's public cloud offering, launched in 2008 (initially with App Engine). GCP leverages the same global infrastructure that powers Google Search, YouTube, and Gmail. It is widely recognized as a leader in data analytics, machine learning/AI, and container orchestration, since Google originally created Kubernetes.

## Global Infrastructure
GCP infrastructure is organized into **Regions** and **Zones** (isolated locations within a region). GCP also owns and operates one of the largest private global networks of any cloud provider, connecting its data centers via undersea cables, which helps reduce latency for global applications. GCP has 40+ regions worldwide.

## Cloud Management Console
The **Google Cloud Console** is the web-based dashboard for managing GCP resources. It also provides the **gcloud CLI**, **Cloud Shell** (a free browser-based terminal with pre-installed tools), and **Terraform**/**Deployment Manager** for infrastructure-as-code.

*(Insert screenshot: `screenshots/gcp-homepage.png`)*

## Four (4) Core Services
1. **Compute Engine** — Scalable virtual machines, GCP's equivalent to EC2/Azure VMs.
2. **Cloud Storage** — Object storage for unstructured data (equivalent to S3/Blob Storage).
3. **Cloud SQL** — Managed relational database service (MySQL, PostgreSQL, SQL Server).
4. **Google Kubernetes Engine (GKE)** — Fully managed Kubernetes service; GCP is considered the leader in container orchestration since Google created Kubernetes.

## Three (3) Advantages
1. **Leading AI/ML and data analytics tools** — services like BigQuery, Vertex AI, and TensorFlow integration make GCP a top choice for data-heavy and AI workloads.
2. **Best-in-class Kubernetes/container support** — GKE is considered the most mature managed Kubernetes offering, since Google originated Kubernetes.
3. **High-performance, low-latency global network** — Google's private fiber backbone often gives GCP an edge in network speed and reliability.

## Typical Enterprise Use Cases
- Big data analytics and business intelligence using BigQuery.
- Machine learning model training and deployment (Vertex AI, TensorFlow).
- Containerized and microservices-based application deployment using GKE.
- High-performance computing workloads requiring fast networking between nodes.
