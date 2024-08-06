# AWS Global Infrastructure
- Throughout the globe, AWS builds Regions to be closest to where the business traffic demands. Locations like Paris, Tokyo, Sao Paulo, Dublin, Ohio. Inside each Region, we have multiple data centers that have all the compute, storage, and other services you need to run your applications.
- Each Region can be connected to each other Region through a high speed fiber network, controlled by AWS, a truly global operation from corner to corner if you need it to be.

## Selecting a Region
- Compliance with data governance and legal requirements: Depending on your company and location, you might need to run your data out of specific areas. For example, if your company requires all of its data to reside within the boundaries of the UK, you would choose the London Region.
- Proximity to your customers: Selecting a Region that is close to your customers will help you to get content to them faster. For example, your company is based in Washington, DC, and many of your customers live in Singapore. You might consider running your infrastructure in the Northern Virginia Region to be close to company headquarters, and run your applications from the Singapore Region.
- Available services within a Region: Sometimes, the closest Region might not have all the features that you want to offer to customers. AWS is frequently innovating by creating new services and expanding on features within existing services. However, making new services available around the world sometimes requires AWS to build out physical hardware one Region at a time.
- Pricing.

## Availability Zones
- Is a single data center or a group of data centers within a Region. Availability Zones are located tens of miles apart from each other. This is close enough to have low latency (the time between when content requested and received) between Availability Zones. However, if a disaster occurs in one part of the Region, they are distant enough to reduce the chance that multiple Availability Zones are affected.

	![[availability_zones 1.png]]


	![[ec2-instance-availability_zone1.png]]

	![[ec2-instance-availability_zone2.png]]

	![[ec2-instance-availability_zone3.png]]

## Edge Locations
- Amazon CloudFront: Es el Content Delivery Network(CDN) de AWS.
- An **edge location** is a site that Amazon CloudFront uses to store cached copies of your content closer to your customers for faster delivery.

	![[edge_loc1.png]]
	![[edge_loc2.png]]

	![[edge_loc3.png]]
