# Global Infrastructure (Latency section)

*Notes: It's always about data recovery strategies and reducing latency... Just understand how the cloud works.*

## Route 53

It is a **managed DNS**. You can register domain names.

## Route 53 Routing Policies

- **Simple routing policy:** Go to one IP
- **Weighted routing policy:** Share the traffic between IPs 
- **Latency Routing Policy:** Send the closest IP
- **Failover routing policy:** Send the IP that works in case of an unhealthy server

## CloudFront

**CDN**: Cache your website and **reduce latency with edge locations**.  
Also provides **DDOS protection**.  
Can take S3 or any custom origin as input.

## WAF: Web Application Firewall

A web application firewall that helps protect web applications from **common web exploits** and bots, allowing users to control traffic access.

## Shield

A managed **Distributed Denial of Service (DDoS) protection**.

## S3 Transfer Acceleration

Upload/Download files to/from **edge locations** that will interact with S3 for you.  
It will reduce **latency**.

## Global Accelerator

Use **edge locations** as proxies. that will use the **private AWS network**.  
Reduce **Latency**. No caching.

## AWS Outposts

**Server racks** that offer the **same AWS infrastructure for your own servers**.  
Designed for hybrid clouds.

## AWS WaveLength

Reduce latency for **5G networks** with special places that serve directly to the 5G network.

## AWS Local Zones

Precise places that serve AWS services for app that requires very **low latency**.

## Global App Architecture

- **Single Region, Single AZ:** Simple to setup but only available in one physical place
- **Single Region, Multi AZ:** Not optimized for latency but OK for recovery
- **Multi Region, Active-Passive:** Optimize the read latency with passive instances. Improves recovery.
- **Multi Region, Active-Active:** Optimize the r/w latency with active instances. Improves recovery.
