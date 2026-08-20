day one of my journey introduction to cloud
1. What is the Cloud?
The cloud is a fundamental shift in how IT resources are delivered.

cloud computing is the on demand delivery of it resources over the internet with pay as you go pricing

AWS is the world's most comprehensive and broadly adopted cloud platform.

Millions of customers use AWS to be more agile, lower costs, and innovate faster.

2. The foundation of cloud computing
The foundation of cloud computing is the client server model:

Role	Analogy	Computing Equivalent
Client	The customer ordering coffee	A user making a request (e.g., accessing a website, running an app)
Server	The barista making the coffee	A virtual server (EC2 instance) that processes requests and returns responses
Request	"I want a triple mocha"	Any business need (rain analysis, medical X-rays, streaming video)
Response	The coffee is served	The server returns the requested data or result

The client makes a request to the server, and the server processes the request and sends back the response.
The client-server model is the backbone of all computing — whether in the cloud or on-premises. In AWS, the server is virtual and runs in the cloud.

3. Pay Only for What You Use (The Most Important AWS Concept!)
The Coffee Shop Analogy:

Employees are only paid for the hours they actually work.

The shop hires more baristas on busy days, fewer on slow days.

Staff are not paid to just "sit around" doing nothing.

How This Applies to AWS:

You ONLY pay for the resources you actually consume.

You don't pay for idle capacity or wasted resources.

With pay-as-you-go pricing, you generally pay for the AWS resources/services you consume, according to their specific pricing model. Stopping or deleting a resource can stop further usage charges, but some resources can have additional or ongoing charges depending on what remains provisioned.

4. Cloud Deployment Types
When you deploy cloud resources, you have three main options: Cloud, On-Premises, and Hybrid. Each type offers unique benefits and considerations.

I. Cloud (All-in Cloud)
What it is:

You run all your applications and infrastructure entirely in the cloud.

You migrate existing resources to the cloud OR design and build new applications natively in the cloud.

II. On-Premises (Traditional Data Center)
What it is:

You run all your applications and infrastructure in your own physical data center.

You own, manage, and maintain all the hardware and software.

Why do some companies still use on-premises?

Regulatory requirements – Some industries (healthcare, banking) require data to stay on-premises.

Low latency – Applications that require ultra-low latency (milliseconds) may run better on dedicated hardware.

Legacy systems – Old applications that are hard to migrate to the cloud.

III. Hybrid (Best of Both Worlds)
What it is:

You run some applications in the cloud and some in your on-premises data center.

You connect them using a secure network (VPN, Direct Connect).

Why choose Hybrid?

🔄 Gradual migration – Move applications to the cloud slowly over time.

🔄 Data sovereignty – Keep sensitive data on-premises while using the cloud for compute.

🔄 Bursting – Use the cloud for extra capacity during peak demand (e.g., holiday shopping season).

5. Benefits of cloud

i. Pay as you go: With AWS, you pay only for the resources you actually use, just like paying for electricity—no huge upfront costs, no paying for idle capacity.

ii. massive economies of scale: AWS buys a lot of hardwares in huge whole sale discount and because they buy that good amount of hardware we can purchase them at a lower cost.

iii.  Stop guessing capacity: AWS is very flexible it give you what you need emmidiately at the time you need it and you pay for it. So you never waste money on unused resources and never crash due to high demand.

iv. With AWS, you can test new ideas in seconds instead of months, and if they fail, you just delete them and stop paying—so you spend less time waiting and more time innovating.

Introduction to AWS Global Infrastructure

AWS Regions and Availability Zones

AWS global infrastructure consist of  physical location around the world that contain groups of data centers.
A data center is a building full of servers that store and process digital information.
These groups of data centers are called Availability Zones.
Region
→ Geographic area

Availability Zone
→ Isolated location within a Region

Data center
→ Physical facility containing computing infrastructure

One Region
→ Multiple Availability Zones
Regions and Availability Zones are designed to provide low-latency, fault-tolerant access to services for users within a given area.
Low latency refers to the minimal delay or lag between a user's action and the system's response.

The AWS Shared Responsibility Model

The AWS Shared Responsibility Model is about making sure both sides understand exactly which tasks are ours and which tasks are the customer’s.
AWS is responsible for the security of the cloud, and you are responsible for the security in the cloud.

-Customer responsibility: they are responsible for managing security requirements for their data including which data they store on AWS and who has access to that data.Customers also control how access to the data is granted, managed, and revoked

AWS responsibilities: its responsible for protecting the infrastructure that runs all the services offered in the AWS cloud.This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services.

In the AWS Shared Responsibility Model, the customer is responsible for managing OS patches. AWS provides the underlying infrastructure, but the customer must make sure that their OSs are up to date with the latest security patches. The customer is also responsible for encrypting client-side data. AWS provides various services to help with encryption, but it is the customer’s responsibility to implement and manage these services.

Physical security of data centers and hardware maintenance are AWS responsibilities. Updating software for compute, networking, storage, and database services is also an AWS responsibility.
