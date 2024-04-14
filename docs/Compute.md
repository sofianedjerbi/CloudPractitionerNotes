# Misc Compute Services

## Information: Docker

A platform to **deploy apps packaged in containers**. Avoid compatibility issues.  
A docker image is a packaged application with all dependencies for consistent, portable execution.  
Resources are shared with the host server. It's lighter than VMs.

## ECS: Elastic Container Service

Used to launch **Docker containers on AWS**.  
You should start EC2 instances in advance and maintain them.

## Fargate

Used to launch **Docker containers**, but without any requirements.  
It's a serverless service.

## ECR: Elastic Container Registry

Used to **store container images**.

## Lambda

Lambda is just "**Functions As A Service**".  
**Automatically scales** the resources given to a function.  
**Automatically trigger** functions.  
Pay per calls and **milliseconds**. **Max 15 minutes.**

## API Gateway

**Expose Lambda function through REST APIs / WebSocket APIs.** Used to create serverless APIs.  
It support **security**, **authentication**, API throttling, API **keys**, monitoring...

## AWS Batch

Fully managed **batch processing** at any scale.  
Will dynamically launch **EC2 Instances**.  
Defined as **Docker Images** that will run on **EC2**.  
*(Difference with lambda: no time limit, managed by AWS)*

## AWS Lightsail

**A mini-AWS for beginners.**
