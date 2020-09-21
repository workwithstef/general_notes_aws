# AWS Developer - Getting Started

### Resources
Examples:
- EC2 Elastic Compute Cloud
- VPC
- S3
- etc

### AWS CLI
Usage:
- configure local dev env
- alternative to console

### AWS SDKs
SDK languages:
- Java
- .NET
- Ruby

<!-- working with a node.js app so we'll need a javascript SDK  -->

### Pizza luvers

EC2 for pizza luvrs app
S3 for images & assets
DynamoDB for user data & pizza toppings
ElastiCache for saving session cache
RDS for pizzas
<!-- (RDS = relational database service) -->

### Cloudwatch
Used to monitor and notify of any events in AWS.
Set alarms based on Service metric thresholds

- CPU usage on EC2 instances
- Estimated billing charges
- DynamoDB Read/Write throughput

10p/per month/alarm
<!-- REMEMBER TO SET BILLING ALERTS!! -->

- Can trigger actions e.g auto scaling

#### Simple Notification Service (SNS)
- Can set 'Topics' so that when an event occurs, related to that 'topic', the notification will be sent to your SMS/Email.

This allows you to organise notifications.


### IAM - Identity & Access Management
User access management.

#### IAM Policy

- Policy groups - set permissions to a set of users

#### Multi-Factor Authentication
Duomobile app

#### Users

Best practise is to create users which have given permissions
Never work directly from root (Rule of Least Privileged)

After creating user and assigning to a policy group:
- Set user password Access
- Set password
- Go to 'Dashboard', then copy account ID from top of page
- Now user can login with username, password & account id 
