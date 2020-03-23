# AWS Systems Manager Parameter Store

## [Back to main readme](Readme.md)

You can store data such as passwords, database strings, Amazon EC2 instance IDs, Amazon Machine Image (AMI) IDs, and license codes as parameter values. You can store values as plain text or encrypted data. You can reference Systems Manager parameters in your scripts, commands, SSM documents, and configuration and automation workflows by using the unique name that you specified when you created the parameter.

## Benefits

- Use a secure, scalable, hosted secrets management service with no servers to manage.
- Improve your security posture by separating your data from your code.
- Store configuration data and secure strings in hierarchies and track versions.
- Control and audit access at granular levels.
- Configure change notifications and trigger automated actions for both parameters and parameter policies.
- Tag parameters individually, and then secure access from different levels, including operational, parameter, Amazon EC2 tag, and path levels.
- Reference AWS Secrets Manager secrets by using Parameter Store parameters.
- Use Parameter Store parameters with other Systems Manager capabilities and AWS services to retrieve secrets and configuration data from a central store.


- Use with
	- Amazon Elastic Compute Cloud (Amazon EC2)
	- Amazon Elastic Container Service (Amazon ECS)
	- AWS Secrets Manager
	- AWS Lambda
	- AWS CloudFormation
	- AWS CodeBuild
	- AWS CodePipeline
	- AWS CodeDeploy

Integrations with:
- AWS Key Management Service (AWS KMS)
- Amazon Simple Notification Service (Amazon SNS)
- Amazon CloudWatch
- AWS CloudTrail