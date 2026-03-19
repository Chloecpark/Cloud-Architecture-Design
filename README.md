# Cloud-Architecture-Design
AWS architecture design for a scalable and highly available startup environment using Elastic Beanstalk, Auto Scaling, and Multi-AZ RDS.
Scalable & High-Availability Cloud Architecture on AWS

📌 Project Overview
This project focuses on designing and implementing a robust, scalable, and highly secure cloud infrastructure for a startup using Amazon Web Services (AWS). The primary goal was to build an environment capable of handling rapid growth, ensuring 24/7 availability, and maintaining high performance under fluctuating traffic patterns.

🏗️ Architecture Diagram

🛠️ Key Tech Stack
Compute: AWS Elastic Beanstalk, Amazon EC2 
Database: Amazon RDS (Multi-AZ MySQL) 
Networking: Custom VPC, Public Subnets (Multi-AZ), Elastic Load Balancer (ELB) 
Scaling & Reliability: Auto Scaling, Route 53 (Logic), Multi-AZ Deployment 
Security: Custom Security Groups, Key Pairs 
Monitoring: CloudWatch (Alarms), Email Notifications (SNS) 

🚀 Key Features & Implementation
1. High Availability & Disaster Recovery
Deployed resources across multiple Availability Zones (Multi-AZ) to eliminate single points of failure.
Utilized a Multi-AZ RDS setup for automated failover and data redundancy.
2. Elasticity & Scalability
Configured Auto Scaling policies triggered by network output thresholds (Upper: 60%, Lower: 30%) to dynamically adjust resources based on demand.
Used Elastic Load Balancer (ELB) to distribute incoming traffic efficiently across EC2 instances.
3. Security & Networking
Established a Custom VPC with isolated public subnets for controlled traffic flow.
Implemented Custom Security Groups restricting access to essential ports (HTTP 80, SSH 22).
4. Efficient Management
Leveraged AWS Elastic Beanstalk for automated application deployment and simplified capacity provisioning.
Created Custom AMIs to ensure environment consistency and rapid scaling.

📈 Business Impact
Cost-Efficiency: Automated scaling ensures the startup only pays for the resources it actually uses.
Reliability: The architecture maintains responsiveness even during traffic spikes or unexpected failures.
Future-Proof: Designed to support seamless business expansion and increasing operational demands.
