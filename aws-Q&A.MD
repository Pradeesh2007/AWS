# AWS Interview Questions and Answers (Beginner to Expert)

---

# Amazon EC2 Interview Questions (1–50)


### 1. What is Amazon EC2?

Amazon EC2 (Elastic Compute Cloud) is a web service that provides scalable virtual servers in the AWS cloud.

---

### 2. What are the benefits of EC2?

* Scalable
* Flexible
* Pay-as-you-go pricing
* Secure
* Highly available

---

### 3. What is an AMI?

AMI (Amazon Machine Image) is a template used to launch EC2 instances.

---

### 4. What are instance types in EC2?

Instance types define CPU, memory, storage, and networking capacity.

Examples:

* T2/T3 → General purpose
* C5 → Compute optimized
* R5 → Memory optimized

---

### 5. What is a Security Group?

Security Group acts as a virtual firewall for EC2 instances.

---

### 6. What is a Key Pair?

A key pair is used to securely connect to EC2 instances.

---

### 7. Difference between public and private IP?

* Public IP → Internet accessible
* Private IP → Internal VPC communication

---

### 8. What is an Elastic IP?

Static public IPv4 address in AWS.

---

### 9. What is User Data?

A startup script executed during instance launch.

Example:

```bash
#!/bin/bash
yum install httpd -y
systemctl start httpd
```

---

### 10. What are EBS-backed instances?

Instances using EBS volumes as root storage.

---

## Intermediate Level

### 11. Difference between Stop and Terminate?

* Stop → Instance can restart
* Terminate → Permanently deleted

---

### 12. What is EC2 Auto Recovery?

Automatically recovers unhealthy EC2 instances.

---

### 13. What are Spot Instances?

Unused AWS capacity offered at low prices.

---

### 14. What are Reserved Instances?

Long-term discounted EC2 pricing model.

---

### 15. What is placement group?

Logical grouping of instances for performance.

Types:

* Cluster
* Spread
* Partition

---

### 16. What is ENI?

Elastic Network Interface for network connectivity.

---

### 17. What is hibernation in EC2?

Saves RAM contents to EBS and resumes later.

---

### 18. What monitoring options exist in EC2?

* Basic Monitoring
* Detailed Monitoring
* CloudWatch

---

### 19. Difference between reboot and restart?

* Reboot → Same host
* Stop/Start → New host possible

---

### 20. What is EC2 metadata?

Instance-related information accessible internally.

---

## Advanced Level

### 21. Explain EC2 lifecycle.

Pending → Running → Stopping → Stopped → Terminated

---

### 22. What is Nitro System?

AWS virtualization platform improving performance/security.

---

### 23. Difference between vertical and horizontal scaling?

* Vertical → Increase instance size
* Horizontal → Add more instances

---

### 24. Explain dedicated host.

Physical server dedicated to one customer.

---

### 25. What is capacity reservation?

Reserve EC2 capacity in a specific AZ.

---

### 26. Explain EC2 fleet.

Launches multiple instance types together.

---

### 27. What is IMDSv2?

Improved EC2 metadata service security version.

---

### 28. What is enhanced networking?

High packet-per-second performance networking.

---

### 29. What is SR-IOV?

Improves network performance using virtualization.

---

### 30. What are launch templates?

Templates for launching EC2 instances.

---

## Expert Level

### 31. How do you optimize EC2 cost?

* Spot instances
* Auto Scaling
* Reserved instances
* Rightsizing

---

### 32. How do you secure EC2?

* IAM roles
* Security Groups
* Patch management
* Encryption

---

### 33. Explain EC2 networking performance.

Depends on instance type and enhanced networking.

---

### 34. What are burstable instances?

T-series instances using CPU credits.

---

### 35. Explain CPU credits.

Credits used for temporary CPU bursting.

---

### 36. What is EC2 Image Builder?

Automates AMI creation.

---

### 37. What is AWS Systems Manager?

Management service for EC2 operations.

---

### 38. Explain instance store.

Temporary local storage attached physically.

---

### 39. Difference between EBS and Instance Store?

* EBS → Persistent
* Instance Store → Temporary

---

### 40. What is warm pool in Auto Scaling?

Pre-initialized EC2 instances ready quickly.

---

### 41. Explain EC2 rescue workflow.

Used for troubleshooting boot failures.

---

### 42. What is EC2 serial console?

Direct troubleshooting console access.

---

### 43. Explain launch configurations.

Older method to configure Auto Scaling instances.

---

### 44. What is Elastic Fabric Adapter?

High-performance networking for HPC workloads.

---

### 45. What is placement partition?

Separates workloads across partitions.

---

### 46. Explain instance refresh.

Updates Auto Scaling instances gradually.

---

### 47. What is capacity rebalance?

Handles Spot interruption proactively.

---

### 48. How does EC2 integrate with ELB?

ELB distributes traffic to EC2 instances.

---

### 49. What is CloudInit?

Instance initialization package for Linux.

---

### 50. Explain EC2 best practices.

* Use least privilege
* Enable monitoring
* Use Auto Scaling
* Patch regularly
* Encrypt storage

---

# Amazon VPC Interview Questions (1–50)


### 1. What is Amazon VPC?

Amazon VPC is a logically isolated virtual network in AWS.

---

### 2. What is a subnet?

A subnet is a segmented IP range inside a VPC.

---

### 3. Difference between public and private subnet?

* Public subnet → Internet access
* Private subnet → Internal only

---

### 4. What is CIDR notation?

Defines IP address range.

Example:

```text
10.0.0.0/16
```

---

### 5. What is Internet Gateway?

Provides internet connectivity to VPC.

---

### 6. What is a Route Table?

Controls traffic routing inside VPC.

---

### 7. What is NAT Gateway?

Allows outbound internet access from private subnet.

---

### 8. What is Security Group?

Stateful firewall at instance level.

---

### 9. What is NACL?

Stateless firewall at subnet level.

---

### 10. Difference between SG and NACL?

| Security Group | NACL         |
| -------------- | ------------ |
| Stateful       | Stateless    |
| Allow only     | Allow & Deny |

---

## Intermediate Level

### 11. What is VPC peering?

Private connection between two VPCs.

---

### 12. What is Transit Gateway?

Central hub connecting multiple VPCs.

---

### 13. Explain VPC Flow Logs.

Captures network traffic metadata.

---

### 14. What is DHCP option set?

Controls DNS and domain settings in VPC.

---

### 15. What is endpoint in VPC?

Private connection to AWS services.

---

### 16. Types of VPC endpoints?

* Gateway Endpoint
* Interface Endpoint

---

### 17. What is VPN Gateway?

Connects VPC to on-premises network.

---

### 18. What is Direct Connect?

Dedicated private network connection to AWS.

---

### 19. Explain route propagation.

Automatically updates route tables dynamically.

---

### 20. What is elastic network adapter?

Enhanced networking interface.

---

## Advanced Level

### 21. Difference between NAT Instance and NAT Gateway?

* NAT Instance → Self-managed
* NAT Gateway → Managed AWS service

---

### 22. Explain AWS PrivateLink.

Private access to services without internet.

---

### 23. What is shared VPC?

Multiple accounts share one VPC.

---

### 24. Explain hybrid cloud networking.

AWS integrated with on-premises network.

---

### 25. What is egress-only internet gateway?

Outbound IPv6 internet access only.

---

### 26. Explain VPC Reachability Analyzer.

Network troubleshooting tool.

---

### 27. What are secondary CIDR blocks?

Additional IP ranges added to VPC.

---

### 28. Explain subnet sizing.

Determines available IP addresses.

---

### 29. What is asymmetric routing?

Traffic enters and exits differently.

---

### 30. Explain DNS resolution in VPC.

Uses Route 53 Resolver internally.

---

## Expert Level

### 31. VPC design best practices?

* Multi-AZ
* Private subnets
* Least privilege
* Segmentation

---

### 32. Explain centralized networking.

Shared network architecture using TGW.

---

### 33. What is AWS Network Firewall?

Managed firewall service.

---

### 34. Explain VPC traffic mirroring.

Copies traffic for analysis/security.

---

### 35. What are elastic IP limitations?

Limited static public IPs per account.

---

### 36. Explain jumbo frames.

Larger MTU packets for performance.

---

### 37. What is carrier gateway?

Connects VPC to telecom provider.

---

### 38. Explain DNS hostnames in VPC.

Assigns DNS names to instances.

---

### 39. What is subnet isolation?

Restricting subnet communication.

---

### 40. Explain multi-region networking.

Connectivity between AWS regions.

---

### 41. Explain hub-and-spoke architecture.

Centralized routing design.

---

### 42. What are route priorities?

Determines routing path selection.

---

### 43. Explain blackhole routes.

Invalid/unreachable routes.

---

### 44. What is IPv6 in VPC?

128-bit addressing support.

---

### 45. Explain overlapping CIDR issue.

Conflicting IP ranges between networks.

---

### 46. What is VPC Lattice?

Application networking service.

---

### 47. Explain packet fragmentation.

Breaking large packets into smaller ones.

---

### 48. What is AWS Global Accelerator?

Improves global application performance.

---

### 49. Explain TGW peering.

Transit Gateway connection between regions.

---

### 50. VPC troubleshooting steps?

* Check routes
* SG/NACL
* DNS
* Flow logs
* Connectivity

---
# AWS Interview Questions and Answers (Beginner to Expert)

# Table of Contents

1. EC2
2. VPC
3. Auto Scaling
4. Load Balancer
5. EBS
6. EFS
7. S3
8. Route 53
9. CloudFront (CDN)
10. FSx
11. Lambda
12. Elastic Beanstalk

---

# Amazon EC2 Interview Questions and Answers (1–50)


### 1. What is Amazon EC2?

Amazon EC2 (Elastic Compute Cloud) is a scalable virtual server service in AWS.

### 2. What are the benefits of EC2?

* Scalable
* Pay-as-you-go
* Flexible
* Secure
* Highly available

### 3. What is an AMI?

AMI (Amazon Machine Image) is a template used to launch EC2 instances.

### 4. What is an EC2 instance type?

Defines CPU, RAM, storage, and networking capacity.

### 5. What are common EC2 instance families?

* T → Burstable
* M → General purpose
* C → Compute optimized
* R → Memory optimized

### 6. What is a key pair?

Used to securely connect to Linux EC2 instances.

### 7. What is a Security Group?

A virtual firewall attached to instances.

### 8. Difference between public and private IP?

* Public → Internet accessible
* Private → Internal communication

### 9. What is Elastic IP?

Static public IPv4 address.

### 10. What is User Data?

Startup script executed during launch.

```bash
#!/bin/bash
yum install httpd -y
systemctl start httpd
```

## Intermediate Level

### 11. Difference between Stop and Terminate?

* Stop → Can restart
* Terminate → Permanently deleted

### 12. What are Spot Instances?

Unused AWS capacity at discounted price.

### 13. What are Reserved Instances?

Discounted pricing for long-term usage.

### 14. What is placement group?

Controls instance placement strategy.

### 15. Types of placement groups?

* Cluster
* Spread
* Partition

### 16. What is EC2 metadata?

Information about instance configuration.

### 17. What is an ENI?

Elastic Network Interface for networking.

### 18. What is hibernation?

Stores RAM data to EBS before stopping.

### 19. What is detailed monitoring?

1-minute CloudWatch monitoring.

### 20. Difference between reboot and restart?

* Reboot → Same host
* Stop/Start → New host possible

## Advanced Level

### 21. Explain EC2 lifecycle.

Pending → Running → Stopping → Stopped → Terminated

### 22. What is Nitro System?

AWS virtualization platform improving performance.

### 23. What is EC2 Auto Recovery?

Automatically recovers failed instances.

### 24. Difference between vertical and horizontal scaling?

* Vertical → Bigger server
* Horizontal → More servers

### 25. What is instance store?

Temporary local storage.

### 26. Difference between EBS and Instance Store?

* EBS → Persistent
* Instance Store → Temporary

### 27. What are burstable instances?

T-series instances using CPU credits.

### 28. What are CPU credits?

Used for temporary CPU bursting.

### 29. What is launch template?

Reusable EC2 launch configuration.

### 30. What is launch configuration?

Older Auto Scaling configuration method.

## Expert Level

### 31. How do you optimize EC2 costs?

* Reserved Instances
* Spot Instances
* Auto Scaling
* Rightsizing

### 32. How do you secure EC2?

* IAM roles
* Security Groups
* Patch management
* Encryption

### 33. What is enhanced networking?

High-performance networking support.

### 34. What is IMDSv2?

Improved metadata security version.

### 35. What is EC2 Fleet?

Launches multiple instance types together.

### 36. What is capacity reservation?

Reserves compute capacity in AZ.

### 37. What is dedicated host?

Physical server dedicated to one customer.

### 38. What is Elastic Fabric Adapter?

Networking for HPC workloads.

### 39. What is instance refresh?

Gradual replacement of ASG instances.

### 40. What is warm pool?

Pre-initialized EC2 instances.

### 41. How does EC2 integrate with ELB?

ELB distributes traffic to EC2.

### 42. What is Systems Manager?

AWS management and automation tool.

### 43. What is CloudInit?

Linux initialization package.

### 44. What is serial console?

Direct troubleshooting console.

### 45. Explain EC2 rescue workflow.

Used for boot failure recovery.

### 46. What is capacity rebalance?

Proactive Spot replacement.

### 47. Explain placement partition.

Separates workloads for resilience.

### 48. What are EC2 best practices?

* Least privilege
* Monitoring
* Encryption
* Auto Scaling

### 49. How do you monitor EC2?

Using CloudWatch and CloudTrail.

### 50. Common EC2 interview scenario?

Design scalable web application using:

* EC2
* ALB
* Auto Scaling
* RDS

---

# Amazon VPC Interview Questions and Answers (1–50)


### 1. What is VPC?

Virtual Private Cloud is an isolated AWS network.

### 2. What is subnet?

Segmented IP range inside VPC.

### 3. Difference between public and private subnet?

* Public → Internet access
* Private → Internal only

### 4. What is CIDR?

Defines IP address range.

Example:

```text
10.0.0.0/16
```

### 5. What is Internet Gateway?

Enables internet connectivity.

### 6. What is Route Table?

Controls traffic routing.

### 7. What is NAT Gateway?

Allows outbound internet from private subnet.

### 8. What is Security Group?

Stateful firewall.

### 9. What is NACL?

Stateless subnet firewall.

### 10. Difference between SG and NACL?

* SG → Stateful
* NACL → Stateless

## Intermediate Level

### 11. What is VPC peering?

Private communication between VPCs.

### 12. What is Transit Gateway?

Central hub connecting networks.

### 13. What is VPC Flow Log?

Captures network traffic metadata.

### 14. What is DHCP option set?

Controls DNS/domain settings.

### 15. What is VPC endpoint?

Private AWS service access.

### 16. Types of endpoints?

* Gateway
* Interface

### 17. What is VPN Gateway?

Connects AWS to on-premises.

### 18. What is Direct Connect?

Dedicated private AWS connection.

### 19. What is route propagation?

Dynamic route updates.

### 20. What is elastic network adapter?

Enhanced networking adapter.

## Advanced Level

### 21. Difference between NAT Instance and NAT Gateway?

* NAT Instance → Self-managed
* NAT Gateway → AWS managed

### 22. What is AWS PrivateLink?

Private service access without internet.

### 23. What is shared VPC?

Multiple accounts sharing VPC.

### 24. What is hybrid cloud networking?

AWS connected with data center.

### 25. What is egress-only IGW?

IPv6 outbound-only internet.

### 26. What is Reachability Analyzer?

Connectivity troubleshooting tool.

### 27. What are secondary CIDRs?

Additional IP ranges.

### 28. Explain subnet sizing.

Defines usable IP addresses.

### 29. What is asymmetric routing?

Different ingress/egress paths.

### 30. What is Route 53 Resolver?

DNS service for VPC.

## Expert Level

### 31. VPC best practices?

* Multi-AZ
* Private subnets
* Least privilege

### 32. What is centralized networking?

Hub-and-spoke architecture.

### 33. What is AWS Network Firewall?

Managed firewall service.

### 34. What is VPC traffic mirroring?

Copies traffic for analysis.

### 35. What are Elastic IP limits?

Limited public IPs per account.

### 36. What are jumbo frames?

Large MTU packets.

### 37. What is carrier gateway?

Telecom connectivity gateway.

### 38. What are DNS hostnames?

Automatic internal DNS names.

### 39. What is subnet isolation?

Restricting subnet communication.

### 40. What is multi-region networking?

Connectivity across AWS regions.

### 41. Explain hub-and-spoke design.

Centralized network architecture.

### 42. What are route priorities?

Determines routing preference.

### 43. What are blackhole routes?

Invalid/unreachable routes.

### 44. What is IPv6 in VPC?

128-bit addressing support.

### 45. What is overlapping CIDR?

Conflicting IP ranges.

### 46. What is VPC Lattice?

Application networking service.

### 47. What is packet fragmentation?

Splitting large packets.

### 48. What is AWS Global Accelerator?

Improves global application performance.

### 49. What is TGW peering?

Transit Gateway connection between regions.

### 50. VPC troubleshooting steps?

* Check routes
* SG/NACL
* DNS
* Flow logs

---

# Auto Scaling Interview Questions and Answers (1–50)

## Beginner

### 1. What is Auto Scaling?

Automatically adjusts EC2 capacity based on demand.

### 2. What is an Auto Scaling Group?

Group of EC2 instances managed together.

### 3. Components of Auto Scaling?

* Launch Template
* ASG
* Scaling Policy

### 4. What is desired capacity?

Target number of instances.

### 5. What is minimum capacity?

Minimum instances maintained.

### 6. What is maximum capacity?

Maximum allowed instances.

### 7. What is dynamic scaling?

Scaling based on metrics.

### 8. What is scheduled scaling?

Scaling at specific times.

### 9. What is predictive scaling?

Uses ML to forecast traffic.

### 10. What metrics trigger scaling?

* CPU
* Memory
* Request count

## Intermediate

### 11. What is scale-out?

Adding instances.

### 12. What is scale-in?

Removing instances.

### 13. What is cooldown period?

Wait time between scaling actions.

### 14. What is health check?

Determines instance health.

### 15. Difference between EC2 and ELB health checks?

* EC2 → Instance health
* ELB → Application health

### 16. What is target tracking scaling?

Maintains target metric value.

### 17. What is step scaling?

Scaling in steps based on threshold.

### 18. What is simple scaling?

Basic alarm-triggered scaling.

### 19. What is lifecycle hook?

Custom actions during launch/terminate.

### 20. What is warm pool?

Pre-initialized standby instances.

## Advanced and Expert

### 21. What is instance refresh?

Gradually replaces instances.

### 22. What is capacity rebalance?

Handles Spot interruptions proactively.

### 23. What are mixed instance policies?

Combines instance types.

### 24. What is standby mode?

Temporarily removes instance from ASG.

### 25. What is termination policy?

Determines which instance terminates first.

### 26. What is scaling suspension?

Pauses scaling processes.

### 27. Explain Auto Scaling notifications.

SNS notifications for scaling events.

### 28. What is connection draining?

Allows active requests to finish.

### 29. Auto Scaling best practices?

* Multi-AZ
* Health checks
* Cooldown tuning

### 30. How do you optimize costs?

Use Spot and predictive scaling.

### 31. How do you secure ASG?

IAM roles and least privilege.

### 32. What is launch template versioning?

Multiple template revisions.

### 33. What is instance protection?

Prevents accidental termination.

### 34. What is ASG rollback?

Reverts failed deployment.

### 35. What is ELB integration?

Traffic distribution with ASG.

### 36. Explain scaling metrics.

CloudWatch metrics trigger actions.

### 37. What is default cooldown?

300 seconds.

### 38. What happens during AZ failure?

ASG launches replacements.

### 39. Explain scaling alarms.

CloudWatch alarm triggers scaling.

### 40. What is ASG lifecycle state?

Pending, InService, Terminating.

### 41. What is graceful termination?

Safe shutdown before removal.

### 42. Explain Auto Scaling troubleshooting.

Check alarms, health checks, IAM.

### 43. What is launch failure?

Instance creation failure.

### 44. What is ELB deregistration delay?

Wait before disconnecting instance.

### 45. What are ASG tags?

Metadata automatically applied.

### 46. Explain ASG scaling activities.

History of scaling events.

### 47. What is predictive scaling benefit?

Reduces latency and cost.

### 48. Explain Spot interruption handling.

Lifecycle hooks and rebalance.

### 49. Common Auto Scaling scenario?

Web app scaling during traffic spike.

### 50. Auto Scaling interview architecture?

ALB + ASG + EC2 + CloudWatch.

---

# AWS CLI Interview Questions and Answers (1–50)


### 1. What is AWS CLI?

AWS Command Line Interface (CLI) is a tool to manage AWS services using commands.

---

### 2. Why use AWS CLI?

* Automation
* Faster operations
* Scripting
* Infrastructure management

---

### 3. How do you install AWS CLI?

Download installer from AWS official website.

Linux Example:

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
```

---

### 4. How do you configure AWS CLI?

```bash
aws configure
```

---

### 5. What details are required during configuration?

* Access Key
* Secret Key
* Region
* Output format

---

### 6. How do you check CLI version?

```bash
aws --version
```

---

### 7. How do you list S3 buckets?

```bash
aws s3 ls
```

---

### 8. How do you list EC2 instances?

```bash
aws ec2 describe-instances
```

---

### 9. What are profiles in AWS CLI?

Multiple AWS account configurations.

---

### 10. How do you use a profile?

```bash
aws s3 ls --profile dev
```

---

## Intermediate Level

### 11. What is JMESPath in CLI?

Query language for filtering JSON output.

---

### 12. Example of filtering EC2 instances?

```bash
aws ec2 describe-instances --query "Reservations[*].Instances[*].InstanceId"
```

---

### 13. How do you copy files to S3?

```bash
aws s3 cp file.txt s3://mybucket/
```

---

### 14. How do you sync folders with S3?

```bash
aws s3 sync ./data s3://backup-bucket
```

---

### 15. Difference between cp and sync?

* cp → Copies files
* sync → Synchronizes changes

---

### 16. How do you create an EC2 instance?

```bash
aws ec2 run-instances
```

---

### 17. How do you terminate an instance?

```bash
aws ec2 terminate-instances --instance-ids i-123456
```

---

### 18. How do you create an S3 bucket?

```bash
aws s3 mb s3://mybucket
```

---

### 19. How do you delete an S3 bucket?

```bash
aws s3 rb s3://mybucket
```

---

### 20. How do you enable debug mode?

```bash
aws s3 ls --debug
```

---

## Advanced Level

### 21. What is AWS CLI v2?

Latest AWS CLI version with improved features.

---

### 22. What is auto-prompt mode?

Interactive command assistance.

---

### 23. What is pagination in CLI?

Large results split into pages.

---

### 24. How do you disable pagination?

```bash
aws s3 ls --no-paginate
```

---

### 25. How do you output JSON format?

```bash
aws ec2 describe-instances --output json
```

---

### 26. Supported output formats?

* JSON
* Table
* Text
* YAML

---

### 27. What is AWS STS?

Temporary credential service.

---

### 28. How do you assume IAM role?

```bash
aws sts assume-role
```

---

### 29. How do you configure MFA with CLI?

Using STS temporary tokens.

---

### 30. What is CLI credential file?

Stores AWS credentials locally.

---

## Expert Level

### 31. How do you automate AWS tasks?

Using shell scripts and cron jobs.

---

### 32. How do you secure CLI credentials?

* IAM roles
* MFA
* Secrets Manager
* Avoid hardcoding

---

### 33. What is SSO in AWS CLI?

Single Sign-On authentication support.

---

### 34. How do you troubleshoot CLI errors?

* Debug mode
* IAM permissions
* Network checks

---

### 35. What is waiter command?

Waits until resource reaches desired state.

---

### 36. Example of waiter command?

```bash
aws ec2 wait instance-running --instance-ids i-123456
```

---

### 37. What is CLI auto-completion?

Tab completion for commands.

---

### 38. How do you use environment variables?

```bash
export AWS_ACCESS_KEY_ID=xxxx
```

---

### 39. What is AWS CLI best practice?

Use least privilege IAM access.

---

### 40. How do you monitor CLI activity?

Using CloudTrail logs.

---

### 41. Difference between CLI and SDK?

* CLI → Command-based
* SDK → Programming libraries

---

### 42. What are common CLI errors?

* AccessDenied
* InvalidRegion
* ExpiredToken

---

### 43. How do you rotate credentials?

Update IAM access keys periodically.

---

### 44. How do you upload multipart files to S3?

Using AWS CLI multipart upload.

---

### 45. How do you create CloudFormation stack via CLI?

```bash
aws cloudformation create-stack
```

---

### 46. What is dry-run mode?

Tests permissions without execution.

---

### 47. Example dry-run command?

```bash
aws ec2 run-instances --dry-run
```

---

### 48. How do you automate backups using CLI?

Using scripts with snapshots and S3 sync.

---

### 49. What is AWS CLI scripting use case?

Automated deployment and monitoring.

---

### 50. AWS CLI best practices?

* Use profiles
* Enable MFA
* Use least privilege
* Automate tasks

---

# AWS CloudFormation Interview Questions and Answers (1–50)


### 1. What is CloudFormation?

Infrastructure as Code (IaC) service in AWS.

---

### 2. Benefits of CloudFormation?

* Automation
* Repeatability
* Version control
* Reduced manual work

---

### 3. Supported template formats?

* YAML
* JSON

---

### 4. What is a stack?

Collection of AWS resources managed together.

---

### 5. What is a template?

Blueprint describing infrastructure.

---

### 6. Main sections in template?

* Parameters
* Resources
* Outputs
* Mappings

---

### 7. What is resource section?

Defines AWS resources.

---

### 8. What are parameters?

Dynamic user inputs.

---

### 9. What are outputs?

Export values after deployment.

---

### 10. What are mappings?

Static key-value pairs.

---

## Intermediate Level

### 11. What is stack update?

Modify existing infrastructure.

---

### 12. What is change set?

Preview infrastructure changes.

---

### 13. What is rollback?

Reverts failed deployments.

---

### 14. What is nested stack?

Stack inside another stack.

---

### 15. What is drift detection?

Detects manual infrastructure changes.

---

### 16. What are pseudo parameters?

AWS predefined parameters.

---

### 17. Example pseudo parameter?

```yaml
AWS::Region
```

---

### 18. What is DependsOn?

Defines resource dependency.

---

### 19. What is stack policy?

Protects stack resources.

---

### 20. What is deletion policy?

Controls resource deletion behavior.

---

## Advanced Level

### 21. What is CloudFormation StackSets?

Deploy stacks across accounts/regions.

---

### 22. What is custom resource?

User-defined functionality via Lambda.

---

### 23. What is intrinsic function?

Built-in template functions.

---

### 24. Examples of intrinsic functions?

* Ref
* GetAtt
* Join
* Sub

---

### 25. What is Fn::Sub?

String substitution function.

---

### 26. What is Fn::Join?

Joins string values.

---

### 27. What is Export/Import?

Share outputs across stacks.

---

### 28. What is stack termination protection?

Prevents accidental deletion.

---

### 29. What is cfn-init?

Instance initialization helper.

---

### 30. What is cfn-signal?

Signals stack creation status.

---

## Expert Level

### 31. How do you secure CloudFormation?

* IAM policies
* Stack policies
* Parameter encryption

---

### 32. What are CloudFormation best practices?

* Modular templates
* Version control
* Reusable components

---

### 33. What is blue-green deployment?

Deploy new environment alongside old.

---

### 34. What is immutable infrastructure?

Replace instead of modifying servers.

---

### 35. What is drift remediation?

Fix configuration drift.

---

### 36. What is macro in CloudFormation?

Custom template processing.

---

### 37. Difference between Terraform and CloudFormation?

* Terraform → Multi-cloud
* CloudFormation → AWS native

---

### 38. What is SAM?

Serverless Application Model.

---

### 39. What is CDK?

Cloud Development Kit for IaC.

---

### 40. How do you troubleshoot failed stack?

* Events tab
* Logs
* IAM permissions

---

### 41. What is stack export limitation?

Export names must be unique.

---

### 42. What is resource import?

Bring existing resources into stack.

---

### 43. What is stack drift?

Manual changes outside CloudFormation.

---

### 44. What are wait conditions?

Pause stack until signal received.

---

### 45. What is retain policy?

Preserves resource after deletion.

---

### 46. What is cloud-init?

Linux initialization process.

---

### 47. What is rollback trigger?

CloudWatch alarm based rollback.

---

### 48. CloudFormation use cases?

Infrastructure automation and deployment.

---

### 49. What are nested stack benefits?

Reusability and modularity.

---

### 50. CloudFormation best practices?

* Use parameters
* Modular templates
* Enable rollback
* Version control

---

# Amazon RDS Interview Questions and Answers (1–50)


### 1. What is Amazon RDS?

Managed relational database service in AWS.

---

### 2. Supported RDS engines?

* MySQL
* PostgreSQL
* MariaDB
* Oracle
* SQL Server
* Aurora

---

### 3. Benefits of RDS?

* Automated backups
* Patching
* Scaling
* High availability

---

### 4. What is Multi-AZ deployment?

Synchronous standby replica for HA.

---

### 5. What is Read Replica?

Read-only copy for scaling reads.

---

### 6. Difference between Multi-AZ and Read Replica?

| Multi-AZ    | Read Replica |
| ----------- | ------------ |
| HA          | Read scaling |
| Synchronous | Asynchronous |

---

### 7. What is DB subnet group?

Subnets for RDS deployment.

---

### 8. What is parameter group?

Database engine configuration settings.

---

### 9. What is option group?

Additional database features configuration.

---

### 10. What is automated backup?

Automatic scheduled database backup.

---

## Intermediate Level

### 11. What is snapshot?

Manual database backup.

---

### 12. What is point-in-time recovery?

Restore database to specific time.

---

### 13. What is storage autoscaling?

Automatically increases storage.

---

### 14. What is failover?

Switch to standby during failure.

---

### 15. What is Aurora?

AWS cloud-native relational database.

---

### 16. Aurora advantages?

* Faster performance
* Auto scaling
* High availability

---

### 17. What is encryption in RDS?

Encrypts data at rest.

---

### 18. What is IAM authentication?

Use IAM users for DB access.

---

### 19. What is enhanced monitoring?

OS-level metrics monitoring.

---

### 20. What is Performance Insights?

Database performance analysis tool.

---

## Advanced Level

### 21. What is RDS Proxy?

Connection pooling service.

---

### 22. What is Blue/Green deployment?

Low-downtime database upgrade.

---

### 23. What is cross-region replica?

Replica in another AWS region.

---

### 24. What is storage type in RDS?

* gp2/gp3
* io1/io2

---

### 25. What is maintenance window?

Scheduled maintenance period.

---

### 26. What is backup retention period?

Backup storage duration.

---

### 27. What is RDS event notification?

SNS alerts for DB events.

---

### 28. What is Aurora Serverless?

On-demand auto-scaling Aurora.

---

### 29. What is cluster endpoint?

Shared endpoint for Aurora cluster.

---

### 30. What is reader endpoint?

Endpoint for read replicas.

---

## Expert Level

### 31. How do you secure RDS?

* Encryption
* IAM
* Private subnets
* SG restrictions

---

### 32. How do you optimize RDS cost?

* Reserved instances
* Stop unused DBs
* Right-size instances

---

### 33. How do you troubleshoot high CPU?

* Query tuning
* Indexing
* Scaling

---

### 34. What is replication lag?

Delay between primary and replica.

---

### 35. What is binlog replication?

Binary log-based replication.

---

### 36. What is database migration?

Moving DB between environments.

---

### 37. What is DMS?

Database Migration Service.

---

### 38. What is failover priority?

Determines promotion order.

---

### 39. What is RPO and RTO?

Recovery objectives for DR.

---

### 40. What is Aurora Global Database?

Cross-region disaster recovery.

---

### 41. What is connection pooling?

Reuse database connections.

---

### 42. How do you monitor RDS?

CloudWatch and Performance Insights.

---

### 43. What is slow query log?

Captures slow SQL queries.

---

### 44. What is DB parameter tuning?

Optimizing database settings.

---

### 45. What is storage optimization?

IOPS and storage performance tuning.

---

### 46. What is vertical scaling in RDS?

Increasing DB instance size.

---

### 47. What is horizontal scaling?

Adding read replicas.

---

### 48. RDS best practices?

* Enable backups
* Multi-AZ
* Monitoring
* Encryption

---

### 49. Common RDS interview scenario?

Design HA production database.

---

### 50. Difference between RDS and DynamoDB?

* RDS → Relational
* DynamoDB → NoSQL

---

# AWS IAM Interview Questions and Answers (1–50)


### 1. What is IAM?

Identity and Access Management service.

---

### 2. What are IAM users?

Individual AWS identities.

---

### 3. What are IAM groups?

Collection of IAM users.

---

### 4. What is IAM role?

Temporary access identity.

---

### 5. What is IAM policy?

Permission document in JSON.

---

### 6. What is root user?

Primary AWS account owner.

---

### 7. Why avoid using root account?

Full unrestricted access.

---

### 8. What is MFA?

Multi-Factor Authentication.

---

### 9. Types of IAM policies?

* Managed
* Inline

---

### 10. What is least privilege?

Minimum required permissions.

---

## Intermediate Level

### 11. What is trust policy?

Defines who can assume role.

---

### 12. What is permission policy?

Defines allowed actions.

---

### 13. What is STS?

Security Token Service.

---

### 14. What are temporary credentials?

Short-term access credentials.

---

### 15. What is role assumption?

Temporary role access.

---

### 16. What is federated access?

External identity provider login.

---

### 17. What is SAML federation?

Enterprise authentication integration.

---

### 18. What is IAM Identity Center?

AWS Single Sign-On service.

---

### 19. What is policy simulator?

Tests IAM permissions.

---

### 20. What is explicit deny?

Overrides allow permissions.

---

## Advanced Level

### 21. What is resource-based policy?

Policy attached directly to resource.

---

### 22. What is SCP?

Service Control Policy in AWS Organizations.

---

### 23. What is permission boundary?

Maximum allowed permissions limit.

---

### 24. What is session policy?

Temporary policy during role session.

---

### 25. What is ABAC?

Attribute-Based Access Control.

---

### 26. What is RBAC?

Role-Based Access Control.

---

### 27. What is cross-account access?

Access between AWS accounts.

---

### 28. What is IAM Access Analyzer?

Analyzes external access permissions.

---

### 29. What is condition block?

Conditional permission control.

---

### 30. What are IAM tags?

Metadata for IAM resources.

---

## Expert Level

### 31. IAM best practices?

* Least privilege
* MFA
* No root usage
* Rotate keys

---

### 32. How do you secure IAM?

* Strong password policy
* MFA
* Monitoring

---

### 33. What is credential rotation?

Regularly changing access keys.

---

### 34. What is CloudTrail integration?

Tracks IAM API activity.

---

### 35. What is IAM policy evaluation logic?

Determines final access decision.

---

### 36. What is explicit deny precedence?

Deny overrides all allows.

---

### 37. What is role chaining?

Assuming role from another role.

---

### 38. What is session duration?

Temporary credential validity.

---

### 39. What is permission escalation?

Gaining higher privileges improperly.

---

### 40. What is IAM troubleshooting?

Check policy, trust, SCP, boundaries.

---

### 41. What is identity federation use case?

Corporate SSO integration.

---

### 42. What are access advisors?

Shows service access history.

---

### 43. What is policy versioning?

Multiple policy revisions.

---

### 44. What is IAM JSON structure?

Version, Statement, Action, Resource.

---

### 45. Example IAM policy?

````json
{
  \"Version\": \"2012-10-17\",
  \"Statement\": [
    {
      \"Effect\": \"Allow\",
      \"Action\": \"s3:*\",\n      \"Resource\": \"*\"\n    }\n  ]\n}\n```\n\n---\n\n### 46. What is service-linked role?\nPredefined role linked to AWS service.\n\n---\n\n### 47. What is IAM auditing?\nReviewing permissions and access.\n\n---\n\n### 48. What is AWS Organizations?\nMulti-account management service.\n\n---\n\n### 49. Common IAM interview scenario?\nSecure multi-account AWS environment.\n\n---\n\n### 50. IAM best practices summary?\n- Least privilege\n- MFA\n- Rotate credentials\n- Monitor with CloudTrail\n- Avoid root usage\n:::
````
---
# Amazon CloudWatch Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is Amazon CloudWatch?

Monitoring and observability service in AWS.

---

### 2. What does CloudWatch monitor?

* EC2
* RDS
* Lambda
* Application logs
* Metrics

---

### 3. What are CloudWatch metrics?

Performance data collected over time.

---

### 4. What are default EC2 metrics?

* CPUUtilization
* NetworkIn
* DiskReadOps

---

### 5. What is CloudWatch Logs?

Stores and monitors logs centrally.

---

### 6. What is a namespace?

Container for CloudWatch metrics.

---

### 7. What is a dimension?

Metadata for metrics.

---

### 8. What is CloudWatch Alarm?

Triggers actions based on thresholds.

---

### 9. Example alarm use case?

Alert when CPU > 80%.

---

### 10. What actions can alarms trigger?

* SNS
* Auto Scaling
* Lambda

---

## Intermediate Level

### 11. What is detailed monitoring?

1-minute EC2 metrics.

---

### 12. Difference between basic and detailed monitoring?

| Basic    | Detailed |
| -------- | -------- |
| 5-minute | 1-minute |

---

### 13. What is CloudWatch Dashboard?

Custom monitoring dashboard.

---

### 14. What is log group?

Container for log streams.

---

### 15. What is log stream?

Sequence of log events.

---

### 16. What is retention period?

Duration logs are stored.

---

### 17. What is CloudWatch Agent?

Collects OS-level metrics/logs.

---

### 18. What is unified agent?

Single agent for logs and metrics.

---

### 19. What is custom metric?

User-defined metric.

---

### 20. What is metric math?

Calculations using metrics.

---

## Advanced Level

### 21. What is anomaly detection?

ML-based abnormal activity detection.

---

### 22. What is composite alarm?

Alarm combining multiple alarms.

---

### 23. What is Contributor Insights?

Analyzes high-cardinality data.

---

### 24. What is Logs Insights?

Query logs interactively.

---

### 25. Example Logs Insights query?

```sql id="v6gk8n"
fields @message
| filter status = 500
```

---

### 26. What is CloudWatch Events?

Old name for EventBridge events.

---

### 27. What is embedded metric format?

Structured logging with metrics.

---

### 28. What is metric filter?

Creates metrics from logs.

---

### 29. What is alarm state?

* OK
* ALARM
* INSUFFICIENT_DATA

---

### 30. What is high-resolution metric?

1-second granularity metrics.

---

## Expert Level

### 31. How do you secure CloudWatch?

IAM and encryption.

---

### 32. How do you monitor memory usage?

Using CloudWatch Agent.

---

### 33. What is CloudWatch Synthetics?

Canary-based application monitoring.

---

### 34. What is ServiceLens?

Application observability tool.

---

### 35. What is X-Ray integration?

Distributed tracing support.

---

### 36. What is CloudWatch RUM?

Real User Monitoring.

---

### 37. What is metric aggregation?

Combining multiple metric data.

---

### 38. What is percentile metric?

P90/P95 latency monitoring.

---

### 39. CloudWatch best practices?

* Centralized logging
* Alarm tuning
* Retention policies

---

### 40. Common CloudWatch troubleshooting?

* Missing metrics
* Agent failure
* IAM permissions

---

### 41. What is dashboard sharing?

Share monitoring dashboards.

---

### 42. What is event-driven monitoring?

Automated actions from events.

---

### 43. How do you reduce CloudWatch cost?

Retention optimization and filtering.

---

### 44. What is cross-account monitoring?

Centralized multi-account monitoring.

---

### 45. What is CloudWatch Container Insights?

Container monitoring solution.

---

### 46. What is Lambda Insights?

Enhanced Lambda monitoring.

---

### 47. What is Application Insights?

Automated application monitoring.

---

### 48. What is CloudWatch metric stream?

Real-time metric streaming.

---

### 49. Common interview scenario?

Monitor scalable web application.

---

### 50. CloudWatch best practices summary?

* Monitoring
* Logging
* Alerting
* Automation

---

# AWS CloudTrail Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is CloudTrail?

Tracks AWS API activity.

---

### 2. What does CloudTrail record?

* Console actions
* API calls
* CLI activity

---

### 3. What is an event in CloudTrail?

Recorded AWS activity.

---

### 4. Types of events?

* Management events
* Data events

---

### 5. What are management events?

Administrative API activities.

---

### 6. What are data events?

Resource-level activities.

---

### 7. What is a trail?

Configuration delivering logs.

---

### 8. Where are logs stored?

Amazon S3.

---

### 9. What format are logs stored in?

JSON.

---

### 10. Why use CloudTrail?

Auditing and compliance.

---

## Intermediate Level

### 11. What is Event History?

90-day AWS activity history.

---

### 12. What is multi-region trail?

Tracks events across regions.

---

### 13. What is log file validation?

Detects log tampering.

---

### 14. What is CloudTrail Insights?

Detects unusual API activity.

---

### 15. What is integration with CloudWatch?

Real-time alerting.

---

### 16. What is an organization trail?

Centralized logging for AWS Organizations.

---

### 17. What are global service events?

IAM and Route53 events.

---

### 18. What is S3 bucket policy for CloudTrail?

Allows CloudTrail to write logs.

---

### 19. What is SNS integration?

Notification on log delivery.

---

### 20. What is encryption in CloudTrail?

KMS-based encryption.

---

## Advanced Level

### 21. What is trail aggregation?

Centralized multi-account logs.

---

### 22. What are CloudTrail Insights events?

Abnormal API activity patterns.

---

### 23. What is data event example?

S3 object access.

---

### 24. What is Lake in CloudTrail?

Query and analyze events.

---

### 25. What is event selector?

Controls logged event types.

---

### 26. What is advanced event selector?

Granular event filtering.

---

### 27. What is CloudTrail digest file?

Validates log integrity.

---

### 28. What is CloudTrail retention?

Depends on S3 lifecycle.

---

### 29. How do you secure CloudTrail?

Encryption and restricted access.

---

### 30. How do you monitor IAM changes?

Using CloudTrail events.

---

## Expert Level

### 31. CloudTrail best practices?

* Multi-region trails
* Encryption
* Validation enabled

---

### 32. How do you investigate security incidents?

Analyze CloudTrail logs.

---

### 33. What is unauthorized API detection?

Detect suspicious access.

---

### 34. Difference between CloudTrail and CloudWatch?

| CloudTrail | CloudWatch |
| ---------- | ---------- |
| API logs   | Monitoring |

---

### 35. What is compliance auditing?

Tracking security and access changes.

---

### 36. What is event correlation?

Relating multiple events together.

---

### 37. What is SIEM integration?

Security analysis integration.

---

### 38. What is Athena integration?

SQL querying CloudTrail logs.

---

### 39. What is GuardDuty integration?

Threat detection using logs.

---

### 40. What is forensic analysis?

Security investigation process.

---

### 41. How do you reduce CloudTrail costs?

Filter unnecessary events.

---

### 42. What is centralized logging architecture?

Central S3 logging account.

---

### 43. Common CloudTrail troubleshooting?

* Missing permissions
* S3 issues

---

### 44. What is immutable logging?

Tamper-resistant logs.

---

### 45. What are CloudTrail limitations?

Not real-time monitoring.

---

### 46. What is cross-account auditing?

Monitor multiple accounts centrally.

---

### 47. What are event categories?

Management, Data, Insights.

---

### 48. What is security governance?

Policy and audit enforcement.

---

### 49. Common interview scenario?

Track accidental resource deletion.

---

### 50. CloudTrail best practices summary?

* Centralized logs
* Encryption
* Monitoring
* Validation

---

# AWS KMS Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is AWS KMS?

Key Management Service for encryption.

---

### 2. What is a CMK?

Customer Master Key.

---

### 3. Types of KMS keys?

* AWS Managed
* Customer Managed

---

### 4. What is encryption?

Protecting data using cryptography.

---

### 5. What is symmetric encryption?

Same key for encrypt/decrypt.

---

### 6. What is asymmetric encryption?

Public/private key pair encryption.

---

### 7. What is data key?

Temporary encryption key.

---

### 8. What is envelope encryption?

Encrypting data key using master key.

---

### 9. What AWS services integrate with KMS?

* S3
* EBS
* RDS
* Lambda

---

### 10. Why use KMS?

Centralized encryption management.

---

## Intermediate Level

### 11. What is key rotation?

Automatic periodic key replacement.

---

### 12. What is key policy?

Controls access to keys.

---

### 13. What is grants in KMS?

Temporary delegated access.

---

### 14. What is alias in KMS?

Friendly name for keys.

---

### 15. What is imported key material?

Externally generated keys.

---

### 16. What is CloudHSM integration?

Dedicated hardware encryption.

---

### 17. What is key deletion waiting period?

7–30 days delay before deletion.

---

### 18. What is encryption context?

Additional authenticated metadata.

---

### 19. What is GenerateDataKey API?

Creates temporary data keys.

---

### 20. What is Decrypt API?

Decrypts encrypted data.

---

## Advanced and Expert

### 21. What is customer managed key advantage?

Full control and auditing.

---

### 22. KMS best practices?

* Least privilege
* Key rotation
* Logging enabled

---

### 23. What is multi-region key?

Replicated KMS keys across regions.

---

### 24. What is key usage?

Encrypt/decrypt or signing.

---

### 25. What is signing key?

Used for digital signatures.

---

### 26. What is external key store?

Use external HSM for keys.

---

### 27. What is key material expiration?

Expiration for imported keys.

---

### 28. What is KMS throttling?

API request limit exceeded.

---

### 29. What is envelope encryption benefit?

Efficient large-scale encryption.

---

### 30. What is audit logging in KMS?

CloudTrail integration.

---

### 31. What is key disable?

Temporarily disables key usage.

---

### 32. What is key re-encryption?

Encrypting using another key.

---

### 33. Difference between SSE-S3 and SSE-KMS?

* SSE-S3 → AWS-managed
* SSE-KMS → Customer control

---

### 34. What is KMS integration with Lambda?

Environment variable encryption.

---

### 35. What is grant token?

Immediate grant usage token.

---

### 36. What is asymmetric KMS use case?

Digital signatures and certificates.

---

### 37. What is KMS quota?

Limits on keys and requests.

---

### 38. How do you secure KMS?

Restrictive policies and IAM.

---

### 39. Common KMS troubleshooting?

* Access denied
* Disabled key

---

### 40. What is compliance encryption?

Meeting regulatory requirements.

---

### 41. What is cryptographic erasure?

Delete keys to destroy data access.

---

### 42. What is BYOK?

Bring Your Own Key.

---

### 43. What is FIPS compliance?

Federal security standards.

---

### 44. What is HSM?

Hardware Security Module.

---

### 45. What is KMS pricing based on?

Keys and API requests.

---

### 46. What is re-encrypt API?

Encrypt without exposing plaintext.

---

### 47. What is key ARN?

Unique key identifier.

---

### 48. Common interview scenario?

Secure S3 and RDS encryption.

---

### 49. What is centralized key management?

Single encryption governance model.

---

### 50. KMS best practices summary?

* Rotation
* Auditing
* Least privilege
* Monitoring

---



# Amazon EventBridge Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is Amazon EventBridge?

Serverless event bus service for application integration.

---

### 2. What was EventBridge previously called?

CloudWatch Events.

---

### 3. What is an event bus?

Channel used to route events.

---

### 4. What is an event?

A change in application or AWS service state.

---

### 5. What AWS services integrate with EventBridge?

* EC2
* Lambda
* S3
* CodePipeline

---

### 6. What is a rule in EventBridge?

Defines event matching and targets.

---

### 7. What are targets?

Services receiving events.

---

### 8. Supported targets?

* Lambda
* SNS
* SQS
* Step Functions

---

### 9. What is event pattern?

JSON filter for matching events.

---

### 10. What is scheduled event?

Cron or rate-based automation.

---

## Intermediate Level

### 11. What is custom event bus?

User-created event channel.

---

### 12. What is partner event source?

Third-party SaaS event integration.

---

### 13. What is schema registry?

Stores event schemas.

---

### 14. What is archive in EventBridge?

Stores historical events.

---

### 15. What is replay?

Reprocess archived events.

---

### 16. What is dead-letter queue?

Captures failed event deliveries.

---

### 17. What is event transformation?

Modify event before sending target.

---

### 18. What is API destination?

Send events to external APIs.

---

### 19. What is event routing?

Directing events to targets.

---

### 20. What is event filtering?

Selecting relevant events.

---

## Advanced Level

### 21. What is cross-account event bus?

Send events between AWS accounts.

---

### 22. What is event-driven architecture?

Architecture based on events.

---

### 23. What is fan-out pattern?

One event triggers multiple services.

---

### 24. What is idempotency?

Avoid duplicate processing.

---

### 25. What is event ordering?

Sequence of event processing.

---

### 26. What is retry policy?

Automatic retry on failure.

---

### 27. What is throughput limit?

Maximum event processing capacity.

---

### 28. What is event latency?

Delay in event delivery.

---

### 29. What is schema discovery?

Automatic schema identification.

---

### 30. What is event enrichment?

Adding extra information to events.

---

## Expert Level

### 31. EventBridge best practices?

* Fine-grained rules
* DLQs
* Monitoring

---

### 32. How do you secure EventBridge?

IAM and resource policies.

---

### 33. What is centralized event management?

Single event bus architecture.

---

### 34. How do you troubleshoot failed events?

Check DLQ and logs.

---

### 35. Difference between SNS and EventBridge?

| SNS                | EventBridge     |
| ------------------ | --------------- |
| Pub/Sub            | Event routing   |
| Push notifications | Event filtering |

---

### 36. What is event replay use case?

Reprocessing failed workflows.

---

### 37. What is integration with Lambda?

Serverless automation trigger.

---

### 38. What is SaaS integration use case?

Salesforce and Zendesk events.

---

### 39. How do you reduce EventBridge costs?

Filter unnecessary events.

---

### 40. What is observability in EventBridge?

Monitoring event flow.

---

### 41. What is EventBridge Scheduler?

Advanced scheduling service.

---

### 42. What is event bus policy?

Controls access permissions.

---

### 43. What is event orchestration?

Coordinating workflows.

---

### 44. What are common EventBridge scenarios?

Automated remediation.

---

### 45. What is event correlation?

Linking related events.

---

### 46. What is serverless integration?

Event-driven serverless workflows.

---

### 47. What is CloudTrail integration?

Trigger actions on API activity.

---

### 48. What are EventBridge limitations?

Payload size and quotas.

---

### 49. Common interview scenario?

Auto-stop idle EC2 instances.

---

### 50. EventBridge best practices summary?

* DLQ
* Monitoring
* Fine-grained filters
* Security

---

# Amazon Lightsail Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is Amazon Lightsail?

Simplified cloud hosting service.

---

### 2. Lightsail use cases?

* Small websites
* Blogs
* Development environments

---

### 3. What resources does Lightsail provide?

* Virtual servers
* Storage
* Databases
* Networking

---

### 4. Difference between EC2 and Lightsail?

| EC2      | Lightsail  |
| -------- | ---------- |
| Advanced | Simplified |
| Flexible | Easy setup |

---

### 5. What operating systems are supported?

Linux and Windows.

---

### 6. What is Lightsail instance?

Virtual private server.

---

### 7. What is static IP?

Persistent public IP address.

---

### 8. What is snapshot in Lightsail?

Backup of resources.

---

### 9. What databases are supported?

MySQL and PostgreSQL.

---

### 10. What is Lightsail DNS?

Managed DNS service.

---

## Intermediate Level

### 11. What is load balancer in Lightsail?

Traffic distribution service.

---

### 12. What is container service?

Simple container deployment platform.

---

### 13. What is CDN integration?

Content acceleration using CloudFront.

---

### 14. What is instance plan?

Pricing and resource allocation.

---

### 15. What is networking in Lightsail?

Simplified VPC networking.

---

### 16. What is firewall configuration?

Port-based access control.

---

### 17. What is SSH access?

Secure Linux connectivity.

---

### 18. What is RDP access?

Windows remote access.

---

### 19. What is Lightsail API?

Automation and management API.

---

### 20. What is monitoring in Lightsail?

Basic metrics and alarms.

---

## Advanced and Expert

### 21. Lightsail best practices?

* Snapshots
* Static IPs
* Monitoring

---

### 22. How do you secure Lightsail?

Firewall and SSH keys.

---

### 23. What are Lightsail limitations?

Less customization than EC2.

---

### 24. What is migration to EC2?

Move workloads to advanced AWS services.

---

### 25. What is vertical scaling?

Upgrade instance size.

---

### 26. What is horizontal scaling?

Use load balancer and multiple instances.

---

### 27. What is backup automation?

Scheduled snapshots.

---

### 28. What is high availability?

Using multiple instances.

---

### 29. What is Lightsail container deployment?

Deploy Docker containers.

---

### 30. What is DNS zone?

Domain record management.

---

### 31. What is SSL support?

HTTPS using certificates.

---

### 32. What is Lightsail object storage?

S3-like storage feature.

---

### 33. What is database HA?

Managed database redundancy.

---

### 34. What is cost optimization?

Right-size plans.

---

### 35. What is bandwidth quota?

Monthly transfer limit.

---

### 36. What is monitoring dashboard?

Resource metrics visualization.

---

### 37. What are common troubleshooting steps?

* Firewall
* DNS
* CPU/RAM

---

### 38. What is application deployment?

Hosting apps on Lightsail.

---

### 39. What is WordPress hosting?

Managed WordPress deployment.

---

### 40. What is networking isolation?

Private networking support.

---

### 41. What is Lightsail snapshot restore?

Recovering backups.

---

### 42. What is scaling limitation?

Limited enterprise features.

---

### 43. What is Lightsail pricing model?

Fixed monthly pricing.

---

### 44. What is integration with Route53?

Advanced DNS management.

---

### 45. Common interview scenario?

Deploy low-cost startup website.

---

### 46. What is Lightsail CDN use case?

Global content delivery.

---

### 47. What is managed database use case?

Simplified database hosting.

---

### 48. What is Lightsail SSH browser?

Browser-based SSH console.

---

### 49. What is monitoring limitation?

Limited compared to CloudWatch.

---

### 50. Lightsail best practices summary?

* Backups
* Monitoring
* Security
* Scaling

---

# Amazon WorkSpaces Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is Amazon WorkSpaces?

Managed virtual desktop service.

---

### 2. What operating systems are supported?

Windows and Linux.

---

### 3. What is VDI?

Virtual Desktop Infrastructure.

---

### 4. Benefits of WorkSpaces?

* Remote access
* Secure desktops
* Centralized management

---

### 5. What is bundle in WorkSpaces?

Desktop configuration package.

---

### 6. What protocols are used?

PCoIP and WSP.

---

### 7. What is persistent desktop?

User data retained permanently.

---

### 8. What is non-persistent desktop?

Temporary session-based desktop.

---

### 9. What is WorkSpaces client?

Software to access desktops.

---

### 10. What is directory integration?

Connect with Active Directory.

---

## Intermediate Level

### 11. What is Simple AD?

AWS-managed lightweight directory.

---

### 12. What is AWS Managed Microsoft AD?

Managed enterprise Active Directory.

---

### 13. What is MFA in WorkSpaces?

Additional authentication security.

---

### 14. What is AutoStop mode?

Stops desktops when idle.

---

### 15. What is AlwaysOn mode?

Desktop always running.

---

### 16. What is encryption in WorkSpaces?

Encrypts storage and data.

---

### 17. What is BYOL?

Bring Your Own License.

---

### 18. What is root volume?

OS storage volume.

---

### 19. What is user volume?

User data storage.

---

### 20. What is IP access control group?

Restricts client access IPs.

---

## Advanced and Expert

### 21. WorkSpaces best practices?

* MFA
* Encryption
* AutoStop

---

### 22. How do you secure WorkSpaces?

IAM and security groups.

---

### 23. What is monitoring in WorkSpaces?

CloudWatch integration.

---

### 24. What is image creation?

Custom desktop templates.

---

### 25. What is desktop migration?

Move user desktop data.

---

### 26. What is WorkSpaces Web?

Browser-based workspace access.

---

### 27. What is performance optimization?

Bundle sizing and latency tuning.

---

### 28. What is cost optimization?

Use AutoStop mode.

---

### 29. What is compliance use case?

Secure remote workforce.

---

### 30. What is hybrid deployment?

On-prem AD integration.

---

### 31. What is troubleshooting connectivity?

Check network and directory.

---

### 32. What is session disconnect issue?

Idle timeout or network issue.

---

### 33. What is WorkDocs integration?

File collaboration service.

---

### 34. What is patch management?

OS update management.

---

### 35. What is multi-region deployment?

Global desktop availability.

---

### 36. What is disaster recovery?

Backup and restore desktops.

---

### 37. What is storage scaling?

Increase user volume size.

---

### 38. What is roaming profile?

Portable user settings.

---

### 39. What is endpoint security?

Protect desktop endpoints.

---

### 40. What is latency optimization?

Closer AWS region usage.

---

### 41. What is SSO integration?

Single Sign-On access.

---

### 42. What is WorkSpaces Pools?

Shared desktop pools.

---

### 43. What are common interview scenarios?

Secure remote employee desktops.

---

### 44. What is compliance auditing?

User access tracking.

---

### 45. What is desktop provisioning?

Automated workspace creation.

---

### 46. What is GPU bundle?

Graphics-intensive desktop.

---

### 47. What is session persistence?

Retaining desktop state.

---

### 48. What are WorkSpaces limitations?

Higher latency for distant users.

---

### 49. What is endpoint device support?

Windows, Mac, Linux, mobile.

---

### 50. WorkSpaces best practices summary?

* MFA
* Encryption
* Monitoring
* AutoStop

---


# AWS OpsWorks Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is AWS OpsWorks?

Configuration management service using Chef and Puppet.

---

### 2. What are the types of OpsWorks?

* OpsWorks Stacks
* OpsWorks for Chef Automate
* OpsWorks for Puppet Enterprise

---

### 3. What is configuration management?

Automating server configuration and deployment.

---

### 4. What is an OpsWorks Stack?

Logical container for AWS resources.

---

### 5. What is a layer in OpsWorks?

Defines server role and configuration.

---

### 6. What are common layers?

* Web Layer
* App Layer
* Database Layer

---

### 7. What is an instance in OpsWorks?

EC2 server managed by OpsWorks.

---

### 8. What are recipes in Chef?

Automation scripts for configuration.

---

### 9. What is a cookbook?

Collection of Chef recipes.

---

### 10. What is lifecycle event?

Automatic execution stage in OpsWorks.

---

## Intermediate Level

### 11. Lifecycle events in OpsWorks?

* Setup
* Configure
* Deploy
* Undeploy
* Shutdown

---

### 12. What is Chef?

Automation framework for infrastructure management.

---

### 13. What is Puppet?

Configuration management tool.

---

### 14. What is deployment in OpsWorks?

Application release automation.

---

### 15. What is auto healing?

Automatic instance replacement.

---

### 16. What is custom cookbook?

User-created Chef cookbook.

---

### 17. What is stack scaling?

Adding/removing instances automatically.

---

### 18. What is Elastic Load Balancer integration?

Traffic distribution across instances.

---

### 19. What is IAM integration?

Permission management for OpsWorks.

---

### 20. What is monitoring in OpsWorks?

CloudWatch metrics and logs.

---

## Advanced Level

### 21. What is OpsWorks agent?

Software installed on instances.

---

### 22. What is Berkshelf?

Chef dependency management tool.

---

### 23. What is Chef Automate?

Enterprise Chef management platform.

---

### 24. What is environment variable in OpsWorks?

Configuration value for applications.

---

### 25. What is stack JSON?

Custom deployment configuration data.

---

### 26. What is application deployment lifecycle?

Process of deploying application versions.

---

### 27. What is rolling deployment?

Gradual application deployment.

---

### 28. What is immutable deployment?

Replace old instances with new ones.

---

### 29. What is AWS OpsWorks limitation?

Limited compared to CloudFormation/CDK.

---

### 30. Difference between OpsWorks and CloudFormation?

| OpsWorks          | CloudFormation         |
| ----------------- | ---------------------- |
| Config management | Infrastructure as Code |

---

## Expert Level

### 31. OpsWorks best practices?

* Use version control
* Automate deployments
* Monitor logs

---

### 32. How do you secure OpsWorks?

IAM and encrypted secrets.

---

### 33. What is secret management?

Secure handling of credentials.

---

### 34. What is encrypted data bag?

Secure Chef data storage.

---

### 35. What is centralized configuration management?

Single configuration governance.

---

### 36. What is disaster recovery in OpsWorks?

Automated infrastructure rebuild.

---

### 37. What is infrastructure drift?

Manual changes outside automation.

---

### 38. What is compliance automation?

Automated security policies.

---

### 39. What is hybrid infrastructure support?

Managing cloud and on-prem systems.

---

### 40. What is troubleshooting deployment failure?

Check logs and recipes.

---

### 41. What is scaling automation?

Dynamic infrastructure scaling.

---

### 42. What is OpsWorks integration with CodeDeploy?

Automated CI/CD deployment.

---

### 43. What is node management?

Managing server configurations.

---

### 44. What is blue-green deployment?

Deploy new environment separately.

---

### 45. What is monitoring strategy?

CloudWatch and centralized logs.

---

### 46. What is Chef cookbook versioning?

Managing recipe revisions.

---

### 47. What are common OpsWorks scenarios?

Automated web application deployment.

---

### 48. What is infrastructure consistency?

Identical server configurations.

---

### 49. What is OpsWorks migration path?

Move to SSM or CloudFormation.

---

### 50. OpsWorks best practices summary?

* Automation
* Versioning
* Monitoring
* Security

---

# AWS Systems Manager (SSM) Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is AWS Systems Manager?

AWS service for operational management.

---

### 2. What are SSM benefits?

* Centralized management
* Automation
* Patching
* Secure access

---

### 3. What is SSM Agent?

Software installed on managed instances.

---

### 4. What are managed instances?

Servers managed by SSM.

---

### 5. What is Session Manager?

Browser/CLI-based secure shell access.

---

### 6. What is Run Command?

Execute commands remotely.

---

### 7. What is Patch Manager?

Automated patching solution.

---

### 8. What is Automation?

Automated operational workflows.

---

### 9. What is Parameter Store?

Secure configuration storage.

---

### 10. What is State Manager?

Maintains desired server state.

---

## Intermediate Level

### 11. What is Inventory in SSM?

Collects server metadata.

---

### 12. What is Maintenance Window?

Scheduled operational tasks.

---

### 13. What is Distributor?

Software package deployment service.

---

### 14. What is OpsCenter?

Centralized operations dashboard.

---

### 15. What is Incident Manager?

Incident response management.

---

### 16. What is Explorer?

Multi-account operational insights.

---

### 17. What is Session Manager logging?

Audit logging for sessions.

---

### 18. What is Parameter Store encryption?

KMS encrypted parameters.

---

### 19. Difference between Parameter Store and Secrets Manager?

| Parameter Store | Secrets Manager |
| --------------- | --------------- |
| Config storage  | Secret rotation |

---

### 20. What is hybrid activation?

Manage on-prem servers.

---

## Advanced Level

### 21. What is Automation document?

JSON/YAML workflow definition.

---

### 22. What is document type in SSM?

Automation, Command, Session.

---

### 23. What is secure string parameter?

Encrypted parameter type.

---

### 24. What is Fleet Manager?

GUI-based server management.

---

### 25. What is patch baseline?

Patch approval rules.

---

### 26. What is patch group?

Logical patching target group.

---

### 27. What is SSM compliance?

Patch and configuration compliance tracking.

---

### 28. What is Session Manager port forwarding?

Secure remote port access.

---

### 29. What is Just-in-Time access?

Temporary privileged access.

---

### 30. What is SSM integration with CloudWatch?

Operational monitoring integration.

---

## Expert Level

### 31. SSM best practices?

* Enable logging
* Least privilege
* Automation

---

### 32. How do you secure SSM?

IAM, KMS, logging.

---

### 33. What is centralized server management?

Single-pane operational control.

---

### 34. What is patch compliance reporting?

Audit patch status.

---

### 35. What is server hardening automation?

Automated security configuration.

---

### 36. What is SSM troubleshooting?

* Agent offline
* IAM issue
* Connectivity issue

---

### 37. What is remote access advantage?

No inbound SSH/RDP ports needed.

---

### 38. What is automation rollback?

Revert failed workflows.

---

### 39. What is change management?

Controlled operational changes.

---

### 40. What is operational governance?

Policy-based management.

---

### 41. What is SSM integration with Lambda?

Automated remediation workflows.

---

### 42. What is disaster recovery automation?

Automated failover operations.

---

### 43. What is software inventory management?

Tracking installed software.

---

### 44. What is operational insight?

Centralized operational analytics.

---

### 45. What is cloud resource grouping?

Organized resource management.

---

### 46. What is session auditing?

Logging user sessions.

---

### 47. What is secret injection?

Passing secrets securely to apps.

---

### 48. Common SSM interview scenario?

Patch thousands of EC2 servers automatically.

---

### 49. What is compliance dashboard?

Operational compliance reporting.

---

### 50. SSM best practices summary?

* Automation
* Logging
* Secure access
* Patch management

---

# AWS Certificate Manager (ACM) Interview Questions and Answers (1–50)

## Beginner Level

### 1. What is AWS ACM?

AWS Certificate Manager manages SSL/TLS certificates.

---

### 2. Why use ACM?

Secure HTTPS communication.

---

### 3. What certificates does ACM provide?

Public and private certificates.

---

### 4. What is SSL/TLS certificate?

Encrypts network communication.

---

### 5. What services integrate with ACM?

* ALB
* CloudFront
* API Gateway

---

### 6. What is certificate validation?

Ownership verification process.

---

### 7. Types of validation?

* DNS validation
* Email validation

---

### 8. What is DNS validation?

Domain ownership verified via DNS record.

---

### 9. What is wildcard certificate?

Secures all subdomains.

Example:

```text id="4xll06"
*.example.com
```

---

### 10. What is certificate renewal?

Automatic certificate update.

---

## Intermediate Level

### 11. What is ACM Private CA?

Private certificate authority service.

---

### 12. What is certificate chain?

Hierarchy of trusted certificates.

---

### 13. What is SAN certificate?

Multiple domains in one certificate.

---

### 14. What is imported certificate?

Externally generated certificate upload.

---

### 15. What is certificate expiration?

Certificate validity end date.

---

### 16. What is TLS handshake?

Secure connection negotiation process.

---

### 17. What is HTTPS?

Secure HTTP communication.

---

### 18. What is trust store?

Collection of trusted root certificates.

---

### 19. What is mutual TLS?

Both client and server authentication.

---

### 20. What is ACM integration with ELB?

HTTPS load balancing support.

---

## Advanced Level

### 21. ACM best practices?

* Use DNS validation
* Auto renewal
* Monitor expiration

---

### 22. What is certificate transparency logging?

Public certificate audit logging.

---

### 23. What is ACM regional limitation?

Certificates region-specific except CloudFront.

---

### 24. What is ACM with CloudFront?

Global HTTPS certificate usage.

---

### 25. What is certificate revocation?

Invalidating compromised certificates.

---

### 26. What is OCSP?

Online Certificate Status Protocol.

---

### 27. What is perfect forward secrecy?

Protects past sessions from key compromise.

---

### 28. What is TLS version?

Encryption protocol version.

---

### 29. What is cipher suite?

Encryption algorithm combination.

---

### 30. What is private CA hierarchy?

Root and subordinate CA structure.

---

## Expert Level

### 31. How do you secure ACM?

IAM access control and monitoring.

---

### 32. What is certificate lifecycle management?

Creation, renewal, revocation.

---

### 33. What is centralized certificate management?

Single certificate governance.

---

### 34. What is ACM troubleshooting?

* Validation failure
* Expired cert
* DNS issue

---

### 35. What is imported cert limitation?

No automatic renewal.

---

### 36. What is ACM pricing?

Public certs are free.

---

### 37. What is enterprise PKI?

Organization-wide certificate infrastructure.

---

### 38. What is certificate rotation?

Replacing certificates periodically.

---

### 39. What is SSL offloading?

Encryption handled by load balancer.

---

### 40. What is HSTS?

HTTP Strict Transport Security.

---

### 41. What is browser trust model?

Trusted root certificate verification.

---

### 42. What is certificate pinning?

Restricting accepted certificates.

---

### 43. What is hybrid certificate management?

Cloud and on-prem certificate handling.

---

### 44. What is cross-account certificate sharing?

Sharing ACM certs between accounts.

---

### 45. What is ALB HTTPS listener?

Secure load balancer listener.

---

### 46. What is API Gateway HTTPS integration?

Secure API communication.

---

### 47. Common ACM interview scenario?

Secure website using ALB and ACM.

---

### 48. What is compliance requirement?

Encrypted communication standards.

---

### 49. What is monitoring certificate expiration?

CloudWatch and ACM alerts.

---

### 50. ACM best practices summary?

* DNS validation
* Auto renewal
* Strong TLS
* Monitoring

