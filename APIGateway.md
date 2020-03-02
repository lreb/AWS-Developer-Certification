### [Back to main readme](Readme.md)

it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.

- fetures
	- Metering: define limits, plans fot traffic 
	- Security: IAM, Cognito
	- Resilency: amnages traffic
	- Monitoring: through integration with Amazon CloudWatch
	- Lifecycle Management: lets you operate multiple API versions and multiple stages for each version simultaneously so that existing applications can continue to call previous versions after new API versions are published
	- Designed for Developers: can assign static content for thir responses
	- Real-Time Two-Way Communication: (websocket) chat apps, streaming dashboards
- helps to manage traffic to backends
- concurrent api calls
- CORS support
- authorization and access control
- throttling: ensures that API traffic is controlled to help your backend services maintain performance and availability
- monitoring
- API version management
- pay for the API calls
- Types
	- HTTP api: APIs that proxy to AWS Lambda functions or HTTP backends, They do not currently offer API management functionality.
	- RESTful APIs; serverless workloads and HTTP backends, REST APIs offer API proxy functionality and API management features in a single solution. REST APIs offer API management features such as usage plans, API keys, publishing, and monetizing APIs.
	- WEBSOCKET APIs: real-time two-way communication applications
		- The maximum supported message size is 128 KB
		- charges
			- Connection minutes: Total number of minutes the clients or devices are connected to the WebSocket connection (rounded to a minute).
			- Messages: Total number of messages sent to and received from connected clients. Messages are charged in increments of 32KB. Refer to the pricing page for details about WebSocket API pricing and examples.
- security
	- [IAM Identity Access Management](IAM.md)
	- [Cognito](Cognito.md)
	- OAuth
	- OIDC
	- execute a Lambda authorizer from AWS Lambda
	- SAML
	- expose HTTPS endpoints only
	- You can also give an Amazon VPC or VPC endpoint from a different account access to the Private API using a Resource Policy
	- Lambda authorizers to support your own bearer token auth strategy.
	- You can set a standard rate limit and a burst rate limit per second for each method in your REST APIs and each route in WebSocket APIs. Further, API Gateway automatically protects your backend systems from distributed denial-of-service (DDoS) attacks, whether attacked with counterfeit requests (Layer 7) or SYN floods (Layer 3).
	- you can proxy requests to backend HTTP/HTTPS resources running in your Amazon VPC by setting up Private Integrations using VPC Links
- 750,000 connection minutes per month for up to 12 months
- can import an API definition using OpenAPI 3
- can accept any payloads sent over HTTPS for HTTP APIs, REST APIs, and WebSocket APIs. Typical data formats include JSON, XML
- can execute AWS Lambda functions in your account, start AWS Step Functions state machines, or call HTTP endpoints hosted on AWS Elastic Beanstalk, Amazon EC2, and also non-AWS hosted HTTP based operations that are accessible via the public Internet
- setup plans from 5 to 1000 (RPS) request per day
- With the Swagger importer tool you can create and deploy new APIs as well as update existing ones.
- you can exported to, Swagger files. Documentation is supported for REST APIs in API Gateway

Api Gateway
![alt text](https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto/gigs/112407571/original/6fc6cb6ffe217c4258a87fe3e4db3d92aa567161/write-aws-lambda-method-and-trigger-using-api-gateway.jpg "WAF")