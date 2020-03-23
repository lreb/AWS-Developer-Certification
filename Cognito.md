### [Back to main readme](Readme.md)

- User Pool
- Application Pool
- Access control for AWS resources
- Easy integration with your app
	- Amazon Cognito identity pools (federated identities) enable you to create unique identities for your users and federate them with identity providers. With an identity pool, you can obtain temporary, limited-privilege AWS credentials to access other AWS services
	- Amazon Cognito identity pools enable you to create unique identities and assign permissions for users
	- Users in an Amazon Cognito user pool
	- Users who authenticate with external identity providers such as Facebook, Google, or a SAML-based identity provider
	- Users authenticated via your own existing authentication process
	- Amazon Cognito identity pools assign your authenticated users a set of temporary, limited privilege credentials to access your AWS resources. The permissions for each user are controlled through IAM roles that you create
	- You can also define a separate IAM role with limited permissions for guest users who are not authenticated.
- Secure and scalable user directory
- Standards-based authentication
- Cognito is recommended for Web Identity Federation for mobile applications
- use to ensure your users have a seamless experience across all their devices (mobile application)

-Facebook
	- A user authenticates with Facebook first. They are then given an ID token by Facebook, which they can then trade for temporary security credentials.
	- After the user has successfully logged in to Facebook and received an authentication token, Cognito should be used to exchange the token for temporary access to DynamoDB

- Web identity federation
	- Synchronization of user data across multiple device types.Sign-up and sign-in to your applications.
	- 
- User pools
	- Cognito use to manage sign-up and sign-in functionality for mobile and web applications