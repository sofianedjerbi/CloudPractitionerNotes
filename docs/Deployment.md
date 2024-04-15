# Deployment and Infrastructure

## CloudFormation

**Automatically creates your instances**, their security groups, load balancers, buckets..  
An infrastructure as code service. Offer cost estimation.  
Can easily delete / recreate infrastructure.  
JSON / YAML documents are named **templates**.

## CDK (Cloud Development Kit)

**Allow you to use python, js.. to define CloudFormation templates.**  
Allowing us to deploy infrastructure and app together. Objects might contain their own infrastructure.

## Elastic Beanstalk

**Automatically create an architecture for your app**: instances, load balancers..
A PaaS tool that allow us to worry only about the code.

## CodeDeploy

Hybrid service to internally **deploy application upgrades automatically**.

## CodeCommit

A **git repo** integrated with AWS.

## CodeBuild

**Compile & test** your software.

## CodePipeline
 
**Orchestration layer** over *CodeCommit -> CodeBuild -> CodeDeploy (-> BeanStalk)*

## CodeArtifact

**Upload Artifacts** online. (Maven, npm, yarn, pip..)

## CodeStar / CodeCatalyst

**An UI** to manage software development and code pipeline. Allow cloud code editing.  
*Quickly develop build and deploy*

## Cloud9

An **online IDE**. Allow code collaboration.

## SSM: Systems Manager

An agent to install on your on-premise VM.  
Patch & Run commands across **an entire fleet of servers** (EC2 & On-premises).  
Give **insights about the infrastructure** since the agent is installed everywhere.  
Designed for **hybrid cloud**.

## SSM: Session Manager

**Start a shell** with the SSM agent. **Without SSH.**

## SSM: Parameter Store

Allow to store **configuration and secrets**: API keys, passwords..
