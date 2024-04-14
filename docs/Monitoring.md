# Monitoring

## CloudWatch

**Metrics for every service in AWS.**  
Example: Billing metric, CPU Usage, Network... (Not RAM)  
You can define **custom metics**.

## CloudWatch Alarms

Define **a notification for any metric threshold**.  
Auto Scaling, take EC2 actions, SNS notifications...

## CloudWatch Logs

**Real-time analysis of log files.**
You need CloudWatch agent to grab logs on EC2 instances.  
It can be used on-premises.

## EventBridge (old name = CloudWatch Events)

Schedule Cron jobs, use **events** to trigger something.  
Sources could be anything: EC2 instances, CloudTrail...  
You can define **your own events** or use partner events.

## CloudTrial

**An history of everything that happen in your AWS account** (API calls, Console actions...).  
Used for governance, compliance, audit..

## CloudTrial Insights

Automated activity analysis.

## AWS X-Ray

**Visual analysis** of applications. Used to troubleshoot performance.

## CodeGuru

- **Reviewer:** **Automated code reviews** powered by ML. Sonarqube-ish thing
- **Profiler:** **Suggest improvements**, log performances, memory profiling... Low overhead.

## Health Dashboard: Service History (AWS Health Dashboard)

Show **AWS services health** per region and per service.  
You can open issues to AWS.

## Health Dashboard: Your Account (Service Health Dashboard)

Show **your own services** health. Used to monitor and plan maintenances.



