# Amazon Databases

## AWS RDS

Managed service to **create RDBs**: Postgres, MySQL, MariaDB...

## Aurora

A **scalable & optimized RDB**. Serverless offer available.

## AWS RDS Deployments

- **Read Replicas:** Multi-endpoint read access but a single point for read access.
- **Multi-AZ:** A failover database used only on main database failure.
- **Multi-Region:** Read Replicas across multiple regions.

## ElastiCache

**In-memory cache** database that uses **Redis** or **Memcached**.

## DynamoDB

A **scalable & optimized NoSQL database**.
Store a tuple of values with a given key.

| UserID | Name     | Email            | RegistrationDate |
|--------|----------|------------------|------------------|
| U1     | Alice    | alice@example    | 2021-01-08       |
| U2     | Bob      |                  | 2021-02-15       |
| U3     | Charlie  | charlie@example  |                  |
| U4     | Dana     | dana@example     | 2021-04-10       |
| U5     |          | eve@example      | 2021-05-21       |

## DAX: DynamoDB Accelerator

**An in-memory cache optimized for DynamoDB.**

## DynamoDB Global Tables

**Linked and synchronized DynamoDB instances** across regions or AZ

## Redshift

**A database for analyzing data.** Serverless offer available. A **data warehouse**.

## EMR: Elastic Map Reduce

Create Hadoop clusters to analyze and process high amount of data.
**Create a lot of EC2 instances to analyze your data.**

## Athena

**Perform analytics in S3** objects with SQL queries. For CSV, JSON, Parquet files. **Always serverless**.

## QuickSight

Serverless ML-powered tool to **create cool graphs / charts** :D

## DocumentDB

**Like Aurora but with MongoDB**. Automatically scales.

## Neptune

A fully-managed **graph-database**.

## Timestream

**Time series database**. Cheaper and faster for time series.

## QLDB: Quantum Ledger Database

Record **all changes you made to your application data**. **IMMUTABLE!**  
Cryptographically verifiable. Can be used for finance.

## Managed Blockchain

Like QLDB but **decentralized**. Used with **etherium** or **hyperledger fabric**.

## Glue

**Used to transform data for analytics**. Serverless.
Will load data into redshift, as example.

## DMS: Database Migration Service

Used to **transfer data from a DB to another**.  
Homogenous or heterogenous migrations.


