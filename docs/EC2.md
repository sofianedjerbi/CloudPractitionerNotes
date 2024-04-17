# AWS Elastic Cloud Computing

## EC2

**EC2** is used to create **virtual machines**. 

## EC2 Instance types

- **General Purpose**: Well balanced.
- **Compute Optimized**: CPU focused machines.
- **Memory Optimized**: RAM focused machines.
- **Storage Optimized**: IO focused machines.

## EC2 Security Groups

A group of instances that share **the same firewall rules**.  
A security group is a firewall.

## EC2 Instance Connect

**Online SSH access** to an instance.

## EC2 Instance Store

**Real hardware drives** attached to an instance for **IO performance**.  
Risk of data loss if hardware fails.
They **lose their storage if the instance is stopped**.

## EBS: Elastic Block Storage

A "network" **USB key**. Should be in the same AZ.  
Could be attached to **only one instance**. (In the exam)

## EBS Snapshot

A **snapshot of the EBS data**.  
Allow copy through AZ / Regions.

## AMI: Amazon Machine Image

A **customized EC2 instance**. Likely a Docker Image.  
You can get AMIs **provided by AWS** or in the **Marketplace** or build your **own** images.  
**They are built for a specific region.**

## EC2 Image Builder

Automates the creation and management of EC2 machine images.  
Provides **pipelines for updating and testing images**, ensuring they meet compliance standards before deployment.

## EFS: Elastic File System

**A shared NFS** that can be mounted to 100s of EC2 instances.  
Only with Linux & Multi AZ.

## FSx

- **FSx for Lustre:** HPC on Linux. High-performance I/O.
- **FSx for Windows File Server:** NFS for Windows. Supports SMB and NTFS.

## Shared responsibility model

- **AWS: Infrastructure**, Hardware, Vulnerability analysis, Compliance Validation, Isolation.
- **User: Internal security**, Software, Permissions, OS management, Data.
