### [Back to main readme](Readme.md)

# WAF or Web Aplication Firewall
AWS WAF is a web application firewall that helps protect web applications from attacks by allowing you to configure rules that allow, block, or monitor (count) web requests based on conditions that you define. These conditions include IP addresses, HTTP headers, HTTP body, URI strings, SQL injection and cross-site scripting.

The Managed Rules for WAF address issues like the OWASP Top 10 security risks. These rules are regularly updated as new issues emerge. AWS WAF includes a full-featured API that you can use to automate the creation, deployment, and maintenance of security rules.

- You pay only for what you use
- You can use with origins not hosted in AWS
- Protects your web site from SQL injection, Cross-Site Sripting (XSS)
- Define rules by
	- IP
	- Country
	- Values in request
	- String in request (regex)
	- Length of request
	- Sql njection
	- XSS
- Block request that exceed a number of request in 5 min
- Reuse rules for multiple web apps
- Manage rule groups or use from marketplace
- reaal time metrics
- Automate 
- Use [AWS CloudTrail](AWSCloudTrail.md) to receive history of all calls
- Support fro IPv6 and IPv4
- Setup conditions for IPv6
- Regions
	- Northern Virginia
	- Ohio
	- Oregon
	- Northern California
	- Montreal
	- Sao Pablo
	- AWS GovCloud (Us-West)
- Use Rate-base rule to protect some parts of the application
- Configure custom error page
- Test rules with
	- [Cloud Watch](CloudWatch.md)
	- Sample web request (stored by 3 hours)
- It protects web request over HTTP or HTTPS

WAF
![alt text](https://www.credera.com/wp-content/uploads/2017/02/aws-region.png "WAF")


## Levels

### Allow all requests except the ones that you specify
This is useful when you want CloudFront or an Application Load Balancer to serve content for a public website, but you also want to block requests from attackers.

### Block all requests except the ones that you specify
This is useful when you want to serve content for a restricted website whose users are readily identifiable by properties in web requests, such as the IP addresses that they use to browse to the website.

### Count the requests that match the properties that you specify
When you want to allow or block requests based on new properties in web requests, you first can configure AWS WAF to count the requests that match those properties without allowing or blocking those requests. This lets you confirm that you didn't accidentally configure AWS WAF to block all the traffic to your website. When you're confident that you specified the correct properties, you can change the behavior to allow or block requests.

## AWS Firewall Manager

### WAF support services
- [ALB or Application Load Balancer](ALB.md)
- [Amazon API Gateway](APIGW.md)
- [Amazon CloudFront](CloudFront.md)

## Pricing

- Number of access control list created (web ACLs)
- Number of rules added to ACLs
- Number request

[More information](https://aws.amazon.com/waf/pricing/)