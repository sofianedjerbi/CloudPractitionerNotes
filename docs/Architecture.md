# Architecture

## Well Architected Framework

### Principles
- **Scalability:** Horizontal & Vertical
- **Disposable resources:** servers should be disposable & easily configured
- **Automation:** IaaS, Auto Scaling
- **Loose Coupling:** Reduce dependencies
- **Services, not Servers:** Don't mimic on-premises configuration

### 6 Pillars

- Operational Excellence
- Security
- Reliability
- Performance Efficiency
- Cost Optimization
- Sustainability

## 1/ Operational Excellence

**Run and monitor systems** and **continually improve** (CI/CD).  
Reduce manual interventions.
*Infrastructure as code, good documentation, frequent, small, reversible changes, anticipate failure...*
*(CloudForm, Config, CloudTrial, CloudWatch, X-Ray, CI/CD tools...)*

## 2/ Security

**Protect information**, systems and assets. Migration strategies, **least privilege**, traceability.  
*Encrypt in-transit data...*
*(IAM, STS, MFA, Organizations, Config, CloudTrial, CloudWatch, Inspector, Shield, WAF, CloudFront, VPC...)*

## 3/ Reliability

**Availability**, recover from failures, acquire resources, meet demand, mitigate disruptions.
*(Scaling, Route53, Backups, CloudFormation, S3, CloudWatch, CloudTrial, Config, Service Quotas, Trusted Advisor)*

## 4/ Performance Efficiency

**Democratize advanced technologies**, serverless architecture, **experimenting more often**.  
*Be aware of options...*
*(ASG, Lambda, EBS, S3, RDS, CloudFormation, News Blog, CloudWatch, Caches...)*

## 5/ Cost optimization

Use **scalability to reduce unused resources**. Pay for only what you use.
*(Cost Explorer, Cost & Usage Reports, Glacier, ASG, Lambda, Budgets, CloudWatch, EventBridge...)*

## 6/ Sustainability

Minimizes the environmental impact of running cloud workloads.  
**Use the right amount of computing resources.**
*(ASG, CloudWatch, Lambda, Fargate, Spot Instances, Cold storage, Lifecycles, Read Replicas...)*

## Well-Architected Tool

A free tool to **review architectures** against the 6 pillars of the well-architected framework.  
*You select your workload and answer questions...*

## Cloud Adoption Framework

Help build and execute a comprehensive plan for digital transformation.  
It groups capabilities in six perspectives:

- **Business:** Investments are worth it
- **People:** Bridge between technology and business
- **Governance:** Manage and monitoring resources to ensure that we maximize benefits and minimize risks.
- **Platform:** Build an entreprise-grade, scalable hybric cloud platform.
- **Security:** Achieve confidentiality, integrity and availability.
- **Operations:** Ensure cloud services are continually delivered and we continually improve.

## AWS Right Sizing

The process of **matching the instance size and type** to find the **lowest possible cost**.

## AWS Ecosystem

### Community / Free
Blogs, forums, Whitepapers & Guides, Partner Solutions (optimized CloudFormation templates), Solutions

### Support
See billing section.

### Other

- **Marketplace:** Sell / Buy softwares, templates, containers, AMIs...  
- **Training:** Digital & classroom trainings, private training, certifications...  
- **Professional Services:** A global team of experts that will work in your team

## AWS IQ

Quickly **find professional help** for your projects. **Connect to experts**.

## AWS re:Post

A free forum. A Q&A service.

## Knowledge center

Answers to common questions & best practices on AWS.

## AWS Managed Services

A team of people that **help managing & supporting** applications on AWS.  
They maintain your infrastructure & implement best practices.

