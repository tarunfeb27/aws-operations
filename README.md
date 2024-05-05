# aws-operations
Notes for some general operational tasks in AWS

> Note - All tasks may be explained in context of doing via AWS console but preferbly via IaC tools. Choose one and stick with it, Terraform, CloudFormation or CDK.

- AWS Account management
	- [Creating and managing accounts](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_best-practices_mgmt-acct.html)
	-

- AWS Governance
    - Tagging of resources (At the time of creation)
        - (Several ways to governing this , preferred is IaC i.e., Terraform etc)
        - Types of tags - Business Unit, Cost-Center, Tech Owner, Data Owner, Creation date etc
    - [IAM](https://www.geeksforgeeks.org/identity-and-access-management-iam-in-amazon-web-services-aws/) roles and policies
        - [Policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html#access_policy-types)
        - Create IAM roles and policies to manage access to AWS resources.
        - Enable multi-factor authentication (MFA) for user accounts.

- Cost Management:
    - Utilize AWS Cost Explorer to analyze spending patterns.
    - Purchase Reserved Instances for predictable workloads.
    - Optimize S3 storage costs using storage classes like S3 Standard-IA.
    - Tag resources for cost allocation and tracking.
    - Set up AWS Budgets to monitor spending and receive alerts.

- Infrastructure Provisioning and Management:
    - Launch EC2 instances to host applications.
    - Configure security groups to control inbound and outbound traffic.
    - Create S3 buckets to store static files and backups.
    - Configure VPCs and subnets for network isolation.
    - Allow a new VPC in VPN Gateway
    - etc


- Monitoring and Performance Optimization:
    - Set up CloudWatch alarms to monitor CPU utilization, memory usage, etc.
    - Create CloudWatch dashboards to visualize performance metrics.
    - Use AWS Trusted Advisor to identify performance optimization opportunities.
    - Implement auto-scaling policies based on CloudWatch metrics.
    - Analyze logs using Amazon CloudWatch Logs Insights.


- Backup and Disaster Recovery:
    - Configure automated backups for RDS databases.
    - Enable versioning and lifecycle policies for S3 buckets.
    - Set up cross-region replication for critical data.
    - Create EBS snapshots for data volumes.
    - Test disaster recovery plans regularly using AWS services like AWS Disaster Recovery.

- Some operational tasks related to Git, CI/CD pipeline if possible