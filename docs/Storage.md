# AWS S3: Simple Storage Service

## S3

Allow you to store your data (**objects**) in **buckets**.  
**Global naming**, but defined at **region level**.

## S3 Bucket Policy

**Bucket wide rules across accounts**. Used to make a bucket public.  
Use the sames format as policies.

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject", // Optional
      "Effect": "Allow",
      "Principal": "*", // Target users
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::example-bucket/*" // Target files
    }
  ]
}
```

## S3 Website

An option to **turn a Bucket into a website** to handle HTTP requests and codes.

## S3 Versioning

Store multiple versions in a bucket. Like a **git history**.

## S3 Replication

**Asynchronously synchronizes bucket content.**  
Work across regions. Like `rsync`. Need versioning enabled.

## S3 Storage Classes

- **Standard - General Purpose**: Highly accessed data.
- **Standard - Infrequent Access**: Less accessed but rapid access if needed.
- **One Zone - Infrequent Access**: Data resides only in one zone. Only for secondary copies.
- **Glacier - Instant Retrieval**: Millisecond retrieval, min duration of 90 days.
- **Glacier - Flexible Retrieval**: 3 offers (1/5min, 3/5h or 5/12h) for accessing data. Min 90 days.
- **Glacier - Deep Archive**: 2 offers (12h / 48h) for accessing data. Min 180 days.
- **Intelligent Tiering**: Move your files if they haven't been accessed in X days.

## S3 Encryption

**Server side encryption is enabled by default**.

## Snow Family

**Physical transport of data.**  
Used for **edge-computing or for migrating a huge amount of data**.  
Should be used when the transfer time is above 1 week.

## Snowcone

**Small, portable solution for data transfer**. Up to 14TB of storage.  
Can be shipped.

## Snowball Edge

Bigger. Used to move TBs or PBs of data in or out AWS.  
Provides compute units for EC2 & Lambda.
- **Storage Optimized:** A lot of HDD capacity (80TB).
- **Compute Optimimzed:** 40TB of HDD or 28TB NVMe. Optimized for local EC2 and Lambda usage.

## Snowmobile

A **HUGE truck**. Used only if you need to transfer **more than 10PB**.

## AWS Storage Gateway

**Remote access to AWS filesystem**. Used for hybrid cloud setups.
