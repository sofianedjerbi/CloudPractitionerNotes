# Sharing data across apps

## SQS: Simple Queue Service

A **queue, producer / consumer system**. Oldest service. Serverless.  
Max retention 4 days up to 14 days. **FIFO option available**, but **no default order**.
Decouple applications.

## Kinesis

Real-time **big data streaming**.  

- **Data Streams:** **Low latency streaming** to ingest data from A LOT of different sources.
- **Data Analytics:** Real-time analysis for ML...
- **Data Firehose:** Load streams into S3, Redshift, ElasticSearch...
- **Video Streams:** Monitor real-time video streams for analytics or ML.

*Streams -> Analytics -> Firehose (-> Redshift)*

## SNS: Simple Notification Service

**Publisher/Subscriber** integration. Send a message to **many receivers**.
**Example subscribers:** SQS, Lambda, Kinesis Data Firehose, Emails, HTTP...
Decouple applications.

## Amazon MQ: Message Queue

Wrapper around **RabbitMQ and ActiveMQ**.  
Used only when migrating to the cloud. **You better use SNS or SQS**.
