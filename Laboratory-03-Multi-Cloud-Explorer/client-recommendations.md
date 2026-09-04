# Client Recommendations

## Client A — Startup Company
**Recommended Platform: Amazon Web Services (AWS)**

AWS is the best fit for a startup with a limited budget that expects rapid growth. Its **AWS Free Tier** and **pay-as-you-go pricing** let the startup launch with minimal upfront cost, while services scale automatically as user demand grows. AWS's serverless offerings remove the need to manage servers at all, which suits a small team without dedicated DevOps staff. The startup could use **AWS Lambda** for serverless backend logic, **Amazon S3** for storing app assets and user uploads, and **Amazon DynamoDB** for a low-maintenance, auto-scaling NoSQL database.

## Client B — University
**Recommended Platform: Microsoft Azure**

Since the university already relies on Windows Server, Microsoft 365, and Active Directory, Azure is the natural migration path because it integrates directly with these existing systems. Using **Azure AD Connect**, the university can sync its on-premises Active Directory with the cloud without rebuilding its identity infrastructure. This reduces both migration risk and staff retraining time. Recommended services include **Azure Virtual Machines** (to migrate existing Windows Server workloads), **Azure Active Directory (Microsoft Entra ID)** for unified identity management, and **Azure Files** for shared file storage compatible with existing Windows file-sharing protocols.

## Client C — AI Research Company
**Recommended Platform: Google Cloud Platform (GCP)**

GCP is the strongest choice for a company building AI and machine learning applications that need high-performance computing. Google created and still leads development on many of the underlying tools used in modern ML workflows, including TensorFlow and Kubernetes. GCP's infrastructure is optimized for large-scale data processing and model training with specialized hardware accelerators. The company could use **Vertex AI** for building and deploying ML models, **BigQuery** for large-scale data analytics, and **Google Kubernetes Engine (GKE)** to orchestrate containerized training workloads across GPU/TPU-backed clusters.

## Client D — Global E-Commerce Company
**Recommended Platform: Amazon Web Services (AWS)**

For a multinational e-commerce company needing high availability and automatic scaling, AWS's mature global infrastructure and auto-scaling tools are the strongest fit. With the largest number of regions and availability zones among the three providers, AWS lets the company place resources close to customers worldwide, reducing latency. Its auto-scaling and load-balancing services are also proven at massive scale by companies like Amazon.com itself. Recommended services include **Amazon EC2 Auto Scaling** to handle traffic spikes automatically, **Elastic Load Balancing (ELB)** to distribute traffic across servers, and **Amazon CloudFront** as a global CDN to speed up content delivery to customers everywhere.

---

## Multi-Cloud Decision Matrix (Checkpoint 6)

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | AWS | Free Tier + serverless options minimize cost while allowing fast scaling as the user base grows. |
| Enterprise Organization | AWS | Broadest service catalog and proven track record supporting large, complex enterprise workloads. |
| Microsoft Environment | Azure | Native integration with Windows Server, Active Directory, and Microsoft 365 reduces migration friction. |
| AI / Machine Learning | GCP | Leading AI/ML tooling (Vertex AI, TensorFlow) and infrastructure optimized for data-heavy workloads. |
| Kubernetes Deployment | GCP | Google originated Kubernetes; GKE is widely regarded as the most mature managed Kubernetes service. |
| Global Web Application | AWS | Largest global region/AZ footprint plus mature auto-scaling and CDN tools for worldwide low-latency access. |
