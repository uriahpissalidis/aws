# AWS Certified Cloud Practicioner Certification Course (CLF-001)

### Common Routes After Cloud Practitioner

SysOps Administrator (Junior DevOps)
Developer Associate (Cloud Developer)
Solutions Architect (Cloud Engineer, more common)

Cloud practitioner could be done from 6 - 30 hours. Recommended time is 1-2 hours a day for two weeks. 

Watch the video lecture and take notes.
Do the hands-on labs and follow along within your own account.
Do paid online practice exams

Exam consists of 4 domains:
* 26% Domain 1: Cloud Concepts (13 Questions)
* 25% Domain 2: Security and Compliance (16-17 Questions)
* 33% Domain 3: Technology (21-22 Questions) 
	|need to know wide range of AWS Services and know core services more in-depth|
* 16% Domain 4: Billing and Pricing (10-11 Questions)

***PASSING GRADE IS 700/1000 AND THE SCORE IS WEIGHTED***
65 questions, 50 scored, 15 unscored. 1.5 Hours, 1.5 mins per question. Exam time is 90 minutes, seat time is 120 minutes. Seat time refers to the amount of time you should allocate for the exam. It includes:

* Time to review the instructions
* Show online proctor your workspace
* Read/accept NDA
* Complete the exam
* Provide feedback at the end

When you pass you're valid for 3 years before recertification. 

Notes:

=====
Cloud Computing - the practice of using a network of remote servers hosted on the internet to store, manage and process data, rather than a local server or a personal computer.

On-Premise:
* You own the servers and hire IT people
* Pay/rent the real-estate
* Take all the risk

Cloud Providers:
* Someone else owns the servers and hires the IT people
* Someone else pays or rents the real-estate
* You are responsible for configuring cloud services and code, someone else takes care of the rest
=====

=====
**Dedicated Server**
One physical machine dedicated to single a business.
Runs a single web-app/site.
***Very expensive, high maintenance, high security.***

**Virtual Private Server (VPS)**
One physical machine dedicated to a single business. 
The physical machine is virtualized into sub-machines.
Runs multiple web-apps/sites
***Better utilization and isolation of resources***

**Shared Hosting**
One physical machine, shared by hundreds of businesses.
Relies on most tenants under-utilizing their resources.
***Very cheap, limited functionality, poor isolation***

**Cloud Hosting** (Cloud also includes the above use-cases)
Multiple physical machines that act as one system.
The system is abstracted into multiple cloud services
***Flexible, scalable, cost-effective, high configurabliity***

=====

=====
Amazon is a multinational computer technology headquartered in seattle washington. Founded in 1994 by Jeff Bezos. Andy Jassy is the current CEO of Amazon, previously the CEO of AWS.

=====

=====
AWS was launched in 2006 and is the leading cloud service provider. CSP = Cloud Service Provider.

* Simple Queue Service (SQS) was the first AWS service launched for public use in 2004.
* Simple Storage Service (S3) was launched in March of 2006.
* Elastic Compute Cloud (EC2) was launched in August of 2006 and still remains their most used service.
* In 2010, it was reported all of amazon's retail sites had migrated to AWS.
* To support training and skill standardization, AWS began offering a certification program for computer engineers on April 2013.

=====

=====
### What is a CSP?

A CSP is a company which provides multiple cloud services tens to hundreds of services.
Those cloud services can be chained together to create cloud architectures.
Those cloud services are accessible via Single Unified API eg. AWS API
Those cloud services utilized metered billing based on usage eg. per second, per hour.
Those cloud services have rich monitoring built in eg. AWS CloudTrail.
Those cloud services have an infrastructure as a Service (IaaS) offering.
Those cloud services offer automation via infrasctructure as code (IaC)

If a company offers multiple cloud services under a single UI but do not meet most of or all of these requirements it will be referred to as a cloud platform (Twilio, HashiCorp, Databricks)

=====

=====
## Landscape of CSPs
Tier 1: Early to market, wide offering, strong synergies between services, well recognized in the industry. AWS, Microsoft Azure, Google Cloud Platform (GCP) Alibaba Cloud.

Tier 2: Backed by well-known tech companies, slow to innovate and turned to specialization. IBM Cloud, Oracle Cloud, Rackspace (OpenStack)

Tier 3: Virtual Private Servers (VPS) turned to offer code IaaS offering. Simple, cost-effective. Vultr, Digital Ocean, Linode.

=====

=====
## Gartner Magic Quadrant for Cloud

Magic Quadrant (MQ), a series of market research reports published by IT consulting firm Gartner that rely on proprietary qualitative data analysis methods to demonstrate market trends, such as direction, maturity and participants.

=====

=====
## Common Cloud Services

A CSP can have hundreds of cloud services that are grouped into various types of services. The four most common types of cloud services (the 4 core) for Infrastructure as a Service (IaaS) would be:

1. Compute (EC2: Imagine having a virtual computer that can run applications, programs, and code.
2. Storage: Imagine having a virtual hard-drive that can store files.
3. Networking: Imagine having virtual network defining internet connections or network isolations between services or outbound to the internet
4. Imagine a virtual database for storing reporting data or a database for general purpose web-applications.

AWS has over 200+ cloud services.

Other categories outside of the 4 core:
Analytics, application integration, ar and vr, aws cost management, blockchain, business applications, containers, customer engagement, dev tools, end user computing, game tech, IoT, machine learning, management and governance, media services, migration and transfer, mobile, quantum technologies, robotics, satellites, security identity and compliance.

=====

=====
## Services available to us
Nav bar -> products -> compute. 
Also features has info available
Will be doing lots of pricing
Documentation is on the bottom of the page for their features/products

======

======
## Evolution of Computing
Dedicated -> VMs -> Containers -> Functions

Dedicated:
* A physical server is wholly utilized by a single customer
* You'll have to guess your capacity
* You'll overpay for an underutilized server
* You can't vertically scale, you need a manual migration
* Replacing a server is very difficult
* You are limited by your Host Operating System
* Multiple apps can result in conflicts in resource sharing (Multiple app usage is **bad practice**)
* You have a *guarantee of security, privacy, and full utility of underlying resources*

VMs:
* You can run multiple VMs on one machine
* Hypervisor is the software layer that let's you run the VMs
* A physical server shared by multiple customers
* You pay for a fraction of the server
* You'll overpay for an underutilized VM
* You are limited by your Guest's Operating System
* Multiple apps on a single VM can result in conflicts in resource sharing
* Easy to export or import images for migration
* Easy to vertically/horizontally scale

Containers:
* VM running multiple containers
* Docker Deamon is the name of the software layer that let's you run multiple containers (think of Docker)
* You can maximize the available capacity which is more cost effective
* Your containers share the same underlying OS so containers are more efficient than multiple VMs
* Multiple apps can run side-by-side without being limited to the same OS requirements and will not cause conflicts during resource sharing

Functions:
* Are managed VMs running managed containers
* Known as *serverless computing*
* You upload a piece of code, choose the amount of memory and duration
* Only responsible for code and data, nothing else
* Very cost-effective, only pay for the time code is running, VMs only run when there is code to be executed
* Cold starts is a side effect of this setup (think Heroku or Netlify) 

======

======
## Types of Cloud Computing

**SaaS** - Software as a Service (For Customers):
* A product that is run and managed by the service provider (Salesforce, Gmail, Office365)
* No need to worry about how the service is maintained. It just works and remains available

**PaaS** - Platform as a Service (For Devs):
* Focus on the deployment and management of your apps (Elastic Beanstalk, Git, Heroku, Google App Engine)
* Provisioning, configuring, hardware and OS are all taken care of by the platform

**IaaS** - Infrastructure as a Service (For Admins):
* The basic building blocks for cloud IT. Provides access to networking features, computers, and data storage space. (Azure, AWS, Oracle Cloud)
* IT staff, data centers, and hardware are all taken care of
======

======
## Cloud Computing Deployment Models

Public Cloud:
Everything (the workload or project) is built on the CSP (aka Cloud-native or Cloud First)

Private cloud:
Everything built on the company's data centers
Also known as on-premise
The cloud could be open stack

Hybrid cloud:
Using both on-premise
and
a CSP

Cross-Cloud (Multi cloud):
Using multiple cloud providers (eg Azure Arc and Anthos), AWS is usually not cross-cloud friendly

======

======
## Cloud Computing Deployment Models

Cloud:
* Fully utilizing Cloud Computing
Companies that are starting out today or are small enough to make the leap from a VPS to a CSP (startups, SaaS offerings, New projects and companies)

Hybrid:
* Using both cloud and on-premise
Organizations that started with their own datacenter, can't fully move to the cloud due to effort of migration of security compliance (Banks, FinTech, Large professional Service Providers, Legacy on-premise)

On-Premise:
* Deploying resources on-premises, using virtualization and resouce management tools is sometimes called "private cloud" (Canadian government, AIG, hospitals)

* Orgs can't run on cloud due to strict regulatory compliance or the sheer size of their org (ie, public sector aka government, sensitive data [think hospitals], insurance companies)

======

======
