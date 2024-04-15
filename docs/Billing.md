# Billing

## Organizations

**Manage multiple AWS accounts.** (per department, per cost center, like directories..)   
**Restrict account privileges with Service Control Policies.**  
Can create **consolidated billing**.  
Pricing benefits from aggregated usage.

## SCP: Service Control Policies

**Whitelist/blacklist IAM actions**.  
Nothing is allowed by default, *you should allow everything to the root account so the others will inherit.*  
There is **a hierarchy**.

## AWS Control Tower

**Setup and govern** a **multi-account environment**.  
It **automatically setup organizations and OUs.** *(deny regions...)*

## RAM: Resource Access Manager

**Share AWS resources with other accounts** *(VPC, instances..)*

## AWS Service Catalog

**Automated service usage with templates**.
You can create **your own services into the catalog**.

## Pricing

- **Pay-as-you-go:** For what you use. Agile, responsive.
- **Save when you reserve:** Minimize risks, predictive budget. Pay less.
- **Pay less by using more**
- **Pay less as AWS grows**

## EC2 Pricing

- On-demand: Minimum 60s, pay second.
- Reserved instances: 1 or 3 year commitment.
- Dedicated Hosts: Dedicated on-demand or with reservation.
- Spot instances: Unused instances but can be deleted at any moment.
- Savings plans: Commit do spending a certain $ per hour for 1/3 years.
  - Up to 72% discount
  - Compute savings plan allow to change EC2 offer
  - Savings plan is available for ML services

## Compute Optimizer

**Recommend optimal AWS resources for your workload.**

## Billing and Costing tools

**IMPORTANT:**

**- Estimating cost:**
  - **Pricing calculator:** Compute future cost and usage

**- Tracking cost:**  
  - **Billing dashboard:** Main dashboard with graphs
  - **Cost allocation tags:** Tags to group costs
  - **Cost and usage reports:** Report to CSV files, databases..
  - **Cost explorer:** More precise graphs & prediction

**- Monitoring against costs plans:**
  - **Billing alarms:** Alarm on high usage. Simple threshold.
  - **Budgets:** Send alarm when usage or forecast exceeds the budget.

## Cost Anomaly Detection

**Detect unusual spends.**

## Service Quotas

Notify you when certain services hit a threshold *(ex: lambda 900 concurrent executions)*

## Trusted Advisor

**General AWS suggestions.** Business & Enterprise support plan for all checks.
There are cost optimization checks, performance, security, service limit checks...

## Support plans

- **Basic Plan:**
  - **Customer service** & **communities**.
  - **Trusted advisor** basic (7 checks)

- **Developer Plan:**
  - **Business hours email access** to **Cloud Support Associates**
  - Unlimited cases, 1 primary contact
  - **< 24h** for general guidance
  - **< 12h** response on system impaired

- **Business Support Plan:**
  - **24/7 phone, mail + chat access** to Cloud Support Engineers
  - Unlimited cases & contacts
  - Full trusted advisor
  - **< 4h** on production system impaired
  - **< 1h** on production system down

- **Enterprise On-Ramp Support Plan:**
  - **Access to a pool of technical account managers**
  - **Concierge Support Team** (billing best practices)
  - Architecture, infrastructure management reviews
  - **< 30 min** on business critical system down

- **Enterprise Support Plan:**
  - **< 15 min** on business critical system down
