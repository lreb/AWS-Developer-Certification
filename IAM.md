# IAM

### [Back to main readme](Readme.md)

- We can grant IAM users access to services by using policies.
- IAM allows you to manage users, groups, and roles and their corresponding level of access to the AWS Platform.
- allows you to have your users Authenticate using Facebook, Google or Amazon; when uses Web Identity Federation (Cognito)


### Access key

- Use this API UpdateAccessKey for reenabling and disabling the access key in AWS.




## Policy
- Managed Policy
	- provided by AWS to allow you to easily assign IAM permissions to your users based on pre-defined common use cases
	- It can be assigned to multiple users, groups or roles.AWS occasionally updates the permissions defined in an AWS managed policy.It is available for use by any AWS account.
	- It can be assigned to multiple users, groups or roles in your account.It is managed by you.
- Inline Policy
	- It is embedded in a user, group or role.The policy will be deleted if you delete the user, group or role it is associated with.
	- Use to add permissions that are only ever intended to be used for a single user in your account

## Configure cross-account access

allow a user from one AWS account to access and manage resources in another AWS account