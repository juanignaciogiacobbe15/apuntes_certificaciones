# Cloud Computing
> Is the on-demand delivery of IT resources over the internet with pay-as-you-go pricing.
> On-demand delivery indicates that AWS has the resources you need, when you need them.
> Is the delivery of computing services over the Internet.
> In AWS, you only pay for what you use. 

## Benefits
- Trade upfront expense for variable expense: refers to data centers, physical servers, and other resources that you would need to invest in before using them. Variable expense means you only pay for computing resources you consume instead of investing heavily in data centers and servers before you know how you're going to use them. Cost saving.
- Stop spending money to run and maintain data centers: focus less on these tasks and more on your applications and customers.
- Stop guessing capacity: you don’t have to predict how much infrastructure capacity you will need before deploying an application.  You can access only the capacity that you need. You can also scale in or scale out in response to demand.
- Benefit from massive economies of scale: you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers can aggregate in the cloud, providers, such as AWS, can achieve higher economies of scale. The economy of scale translates into lower pay-as-you-go prices.
- Increase speed and agility: The flexibility of cloud computing makes it easier for you to develop and deploy applications. It enables you to access new resources within minutes.
- Go global in minutes: The global footprint of the AWS Cloud enables you to deploy applications to customers around the world quickly, while providing them with low latency.
## CapEx VS OpEx
- Capital Expenditures(CapEx): Are upfront purchases toward fixed assets.
- Operating Expenses(OpEx): Are funds used to run day-to-day operations.

## Cloud Computing Models
### Infrastructure as a Service(IaaS)
- Building blocks(can be rented and you can choose how to put them together).

### Software as a Service(SaaS)
- Using a complete app on demand that someone offers to users.

### Platform as a Service(PaaS)
- Used by developers to help develop software using web-based-tools without worrying about the underlying infrastructure.

- [[02-Cloud Deployment Models]]

## Regions and Availability Zones(AZ)
- An AWS region is a physical location -> it groups their regions by geographic locations and can include several regions within each location.
- A Region is global and is made up of two or more AZs.
- There are several geographic locations -> Regions are fully independent and isolated, meaning that if one region is impacted by and earthquake for example, the others will not be.
- Regions are resource and service specific, meaning that they are isolated and resources are not automatically replicated across them.
- AWS regions consist of multiple availability zones -> the availability zones consist of one or more physically separated data centers.

	![[Cloud Practitioner (CLF-C02)/Foundations on Cloud Computing/img/availability_zones.png]]

- Each data center is housed in different facilities.
- AWS specifically defines an AZ as one or more discrete data centers with redundant power, networking and connectivity in a AWS region.

### Availability Zones Characteristics
- Is made up of multiple data centers.
- They're each connected through low latency links.
- Are foult tolerant -> if one AZ goes out  of service, the others should not be impacted.
- Multi-AZ deployments provide high availability and foult tolerant.

	![[availability_zones_characteristics.png]]

#### Quizzes

![[quiz_one.png]]

![[quiz_two.png]]