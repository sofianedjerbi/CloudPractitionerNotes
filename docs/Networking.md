# Networking

## VPC: Virtual Private Cloud

A **private network** to group our instances and set rules **within a region**.

## Elastic IP

**A fixed IP address** for an EC2 instance. IPv6 are free.

## Subnet

**Tied to an AZ**.

- **Public subnet:** Accessible from the internet through an **Internet Gateway**.
- **Private subnet:** .. Not accessible from the internet.

We use **routing tables** for communication.  
Private subnets access the internet through **NAT gateways**.  
[cidr.xyz](https://cidr.xyz)

## NACL (Network Access Control List)

A firewall that control the traffic from and to the **subnet**. `ALLOW` and `DENY` rules.  
Can be associated with multiple subnets.

## Security Group

At **instance** level. Not at subnet level. Can only have `ALLOW` rules.

## VPC Flow Logs

The **log of all the IP traffic** within subnets.

## VPC Peering

Used to **connect multiple VPCs** without IP overlapping.  
Is **cross-account** and **cross-region**.

## VPC Endpoints

**Allow connection to AWS services** using a **private network** instead of the public network.  
Provides better security and latency.

**- Gateway:** For S3 & DynamoDB **only**.
**- Interface:** The rest.

## PrivateLink

Allow to connect a VPC to other VPCs **while supporting scaling**.  
Requires a **Network Load Balancer in service VPC** and a **Elastic Network Interface for client VPC**.

## ENI: Elastic Network Interface

**A virtual network card** for instances in the cloud.  
It allows a server to have multiple network connections.  
See this as a virtual ethernet cable to other networks...?

# Site-to-site VPN

Use our **on-premise VPN** to access AWS. Uses **public internet**.
Requires a **CGW** (Customer Gateway) on-premises and a **VGW** (Virtual Private Gateway) on AWS.

# DX: Direct Connect

A **physical connection** between on-premise datacenter and AWS.

## AWS Client VPN

**VPN to AWS Private Network**.  
Will also allow access to on-premises servers if site-to-site VPN is setup.

## Transit Gateway

**A mediator** around Direct Connect, Gateway, VPN Connections.
Allow connection to **100s of VPC connections, on-premise infrastructure**.
