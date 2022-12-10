# Reflecting on AWS Best Practices


Write a few paragraphs that answer the following questions:

* What are the benefits of using multiple AWS accounts to run workloads?
* What are some common patterns for organizing resources in AWS accounts?
* What is the benefit of using AWS Identity and Access Management (IAM) roles for authenticating into AWS accounts?

Answer:

(a) The benefits of using multiple AWS accounts to run workloads are :

1. Group workloads based on business purpose and ownership
2. Apply distinct security controls by environment
3. Constrain access to sensitive data
4. Promote innovation and agility
5. Limit scope of impact from adverse events
6. Support multiple IT operating models
7. Distribute AWS Service Quotas and API request rate limits

(b) Some common patterns for organizing resources in AWS accounts are:

1. Single AWS account
2. Production starter organization
3. Basic Organization
4. Advanced Organization

(c) The benefit of using AWS IAM roles for authenticating into AWS accounts are:

* IAM controls access to AWS services and resources.
* IAM enables access between AWS services (e.g. EC2 to RDS).
* The main feature of IAM is that it allows you to create separate usernames and passwords for individual users or resources and delegate access.
* IAM supports identity federation. If the user is already authenticated, such as through a Facebook or Google account, IAM can be made to trust that authentication method and then allow access based on it.
* IAM is a free service. There is no additional charge for IAM security. There is no additional charge for creating additional users, groups, or policies.
* IAM is PCI DSS compliance.
* IAM supports MFA.
