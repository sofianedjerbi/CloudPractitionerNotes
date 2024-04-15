# Security

## WAF: Web Application Firewall

Protect web applications from **common web exploits** and bots.  
Allow users to control traffic access.
- **Web ACL:** Block IPs, geo-match...

## Shield

A managed **Distributed Denial of Service (DDoS) protection**.
- **Shield Standard:** No cost.
- **Shield Advanced:** Premium protection & 24/7 support.

## AWS Network Firewall

**Protect the entire VPC**, any direction, everything.

## AWS Firewall Manager

Manage all **security rules across multiple accounts** of an organization.
Applies to security groups, WAF rules, AWS Shield, Network Firewall...

## Pentesting

**Allowed for a few services** (EC2, RDS, CloudFront..).   
**Not allowed for some others** (DDoS, Flooding..).
You need to contact the security simulated event @ amazon.com

## AWS KMS: Key Management Service

**Manage keys for us.** Used on many services. **Software Level**  
Example: EBS volume encryption.. Sometimes automatically enabled.

## CloudHSM

A **dedicated keystore hardware device** to manage **encryption keys**.  
It will manage encryption / decryption.

## KMS Keys

- **Customer Managed Key:** Created, Managed and Used by Customer.
- **AWS Managed Key:** Created, Managed and Used by AWS.
- **AWS Owned Key:** Owned by a service and used in many different account. Inaccessible.
- **CloudHSM Key:** Created by CloudHSM device for operation within the CloudHSM cluster.

## ACM: AWS Certificate Manager

Allow to **manage and deploy SSL / TLS** certificates.  
Provide **HTTPS encryption**. TLS

## AWS Secrets Manager

Used to **store secrets**. Supports rotation.

## Artifact

- **Artifact Reports:** Download security and compliance reports.  
- **Artifact Agreements:** Allow to review, accept and track agreements.  

## GuardDuty 

Uses **ML to detect anomalies**. **Analyzes logs**, events...  
*GuardDuty -> EventBridge -> SNS*

## Inspector

Automated **security assessments** of your app settings.  
Analyzes code in **lambda** functions, **EC2 OS vulnerabilities** with SSM and **Container images** only.  
Gives a risk score.

## AWS Config

**Record, change and assess configuration changes** over time. Per-region service.  
Contains a set of recommended rules to verify.  
*"Is there unrestricted SSH access to my security group?"*  
*"Does my bucket are accessible from the public?"*

## Macie

**Uses ML to discover and protect sensitive data.**  
Can alert you if there's sensitive data such as Personally Identifiable Information.

## SecurityHub

**Centralizes security** alerts across all security services and compliance status.  
Works across AWS accounts.

## Detective

Used to find **how an issue in GuardDuty, Macie happens**. Uses **ML and Graphs**.  
Processes logs and events to find the issue.

## AWS Abuse

**Report illegal & abusive usage of AWS.**

## Root User Privileges

**He can do everything.**
Especially:
- Change account settings
- Close account
- Restore IAM permissions
- Change support plan
- Register as seller in the marketplace
- Enable MFA for S3 buckets
- Signup to govcloud..

## IAM Access Analyzer

**Analyzes policies** to identify resources that are **shared with external entities**.  
Allow to **define a zone of trust**.
