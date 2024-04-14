# AWS ELB: Elastic Load Balancing

## ELB

**ELB** is a server that forward traffic to multiple EC2 servers.

## ELB: ALB (Application Load Balancer)

**ALB** is a load balancer designed for **HTTP requests**.

## ELB: NLB (Network Load Balancer)

**NLB** is a load balancer designed for **TCP / UDP**.

## ELB: GLB (Gateway Load Balancer)

**GLB** is a load balancer designed for GENEVE Protocol on IP packets.  
Used for **packet inspection, intrusion detection**.

# AWS ASG: Auto Scaling Groups

## ASG

**ASG** automatically scales your infrastructure based on the received load.  
Ensure we have a **min / max number** of instances running.  
**Terminate** not responding instances.  
Should be used with a load balancer.

## Manual Scaling

Update the size of an ASG manually. Usually a redflag.

## Dynamic Scaling

Respond to changing demand.  
- **Step scaling:** **CloudWatch** alarm triggered (CPU > 70%) => Add or remove instances.
- **Target Tracking Scaling:** Target CPU usage around 40%, scale accordingly.
- **Scheduled Scaling:** Anticipate based on known usage patterns.
- **Predictive Scaling:** Uses Machine Learning to predict future traffic ahead of time.
