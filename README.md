AWS Custom IAM Policies — 

1. Resource Limit Enforcement:
Restricts IAM users to max 2 EC2 instances and 1 S3 bucket, with full ELB, CloudWatch, and Auto Scaling access.

2. Full read access across EC2, S3, IAM, CloudTrail, Config, and VPC. Zero write permissions. Designed for security auditors or compliance reviewers who need to inspect everything but change nothing.

3. Blocks all API calls outside us-east-1 and ap-southeast-1 · global services exempted

4. User can do nothing until MFA is verified· self-service MFA setup always allowed

5. Block to launch expensive EC2, RDS, NAT Gateway, EBS.

6. Block creation of EC2, S3, RDS, Lambda, ELB without required tags like why/which purpose you creating this service.