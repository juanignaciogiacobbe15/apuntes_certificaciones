# Domain Name System(DNS)
- Suppose that AnyCompany has a website hosted in the AWS Cloud. Customers enter the web address into their browser, and they are able to access the website. This happens because of **Domain Name System (DNS)** resolution. DNS resolution involves a customer DNS resolver communicating with a company DNS server.
- DNS resolution is the process of translating a domain name to an IP address.

	![[dns.png]]

	1. When you enter the domain name into your browser, this request is sent to a customer DNS resolver.
	2. The customer DNS resolver asks the company DNS server for the IP address that corresponds to AnyCompany’s website.
	3. The company DNS server responds by providing the IP address for AnyCompany’s website, 192.0.2.0.

## Amazon Route 53
- Is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS.
- Connects user requests to infrastructure running in AWS (such as [[04A-Amazon Elastic Compute Cloud(EC2)]] instances and load balancers). It can route users to infrastructure outside of AWS.
- This enables you to manage all of your domain names within a single location.

### How Amazon Route 53 and Amazon CloudFront deliver content

	![[route53_and_cloudfront.png]]

1. A customer requests data from the application by going to AnyCompany’s website.
2. Amazon Route 53 uses DNS resolution to identify AnyCompany.com’s corresponding IP address, 192.0.2.0. This information is sent back to the customer.
3. The customer’s request is sent to the nearest edge location through Amazon CloudFront.
4. Amazon CloudFront connects to the Application Load Balancer, which sends the incoming packet to an Amazon EC2 instance.