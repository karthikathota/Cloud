# Capital Expenses

These are typically big investments. Like property, buldings and equipment.  
We can resell them later and get some of the money back.  

# Operating Expenses 

Expenses incurred through normal operations.  
This can be called as the cost to do the business. For example rent, payroll, insurance, R&D, etc.  
100% of these can be deducted against the revunue, reducing the tax owning in a year. 

# Benefits Of Cloud 

## High Availabilty

Ability of a system to remain operational to users 24/7 during planned and unplanned outages then we can claim a 100% availabilty. Generally, it is very hard to 
get this 100% availabilty.

Planned outages maybe like OS security patches, application updates, hardware repalcements, migrating to new hosting provider.  
Unplanned outages maybe hardware outages, software bugs, network disruptions, power outages at the data centers and some extreme cases like natural disasters, cyber attacks, etc.  

### Methods to Mitigate Planned Outages 

1) Gradual Deployement Strategy: In this new deployement are done gradually few at a time rather than deploying on all the servers at the sametime. This helps in identifying the deployement that causes unexpected results. 
2) Small Deployement
3) Frequent Deployement
4) Easy rollback plans

### Methods to Mitigate Unplanned Planned Outages 

1) Every simple component has redundancy(i.e error with one single component doesnot affect the whole system).
2) Constant heath monitoring.
3) Strong security practices.
4) Be geographically distributed. 

In conculsion, we can say that High Availabilty is the effort to avoid obvious sources of downtime.


## Scalability

Ability of a system to accomodate increase or decrease in demand by adding or removing resources as needed easily.  
It allows u to adapt to changing user patterns and handle increased traffic without requiring changes to the application code or core system design.  

#### Vertical Scaling(Scaling Up or Scaling Down)

Adding more resources to a single server. It maybe like increasing the memory, adding more CPU's,etc. There is a limit to this.

#### Horizontal Scaling(Scaling Out or Scaling In):

Adding more servers to a system.
No limit to scaling. It becomes complex as we addon servers. It can improve the systems availabilty.  


Adding more resources to a system adds to the cost drastically. 

## Elasticity

The ability of a system to automatically scale up or down the amount of resources that a system uses in response to changing demand. .
Often called as ***autoscaling*** in cloud computing.  
Adds resources automatically to reduce the load.  
It also removes resources when the load is low.  

#### Why is it needed 

More efficient and cost-effective use of resources.  
Minimizes computing waste i.e resources that are paid but not used.   

## Reliability

All the above 3 concepts play a crucial role in determining the reliability of a system.  
It can be defined as the ability of a system to be accesible and usable by users whenever they need it.  

Key Concepts:
1) Ability of s system to recover from failures. Many types of failures can occur in a well defined system like hardware failures, network interruptions, power failures, etc.  

It is achieved by:  
1) Auto Scaling 
2) Avoid single point failures  
3) Multi region deployement  

## Predictability

It gives you the confidence that the system will continue to perform at the expected level in future.  

#### How is it achieved

1) Auto-Scaling  
2) Load Balancing  
3) Different types of types, sizes, pricing tiers
4) Cost management tools

## Security 

Cloud providers are massive targets for hackers so they spend a lot of time and money on making the cloud a secure platform.  
Cloud providers go through security audits and compliance certifications and they provide tools for customers they need to enable and monitor security with their 
own application.  

#### How is it achieved

1) Industry standard compilance certifications  
2) Microsoft Security Response Center(MSRC)  
3) Always on DDos(Distributed denial of service)
4) Role based access control
5) Always up to date platform services  

## Governance 

How a organization chooses to do a business  
Ultimately it is the process of defining, implementing and monitoring a framework of policies that guides 
and organization's cloud operations  

#### How is it achieved

1) Azure policy and blueprint: makes sure that certain policies are followed
2) Management grops: allows to manageme subscriptions  
3) Custom roles  

## Manageability

There are 2 parts
1) Management of the cloud
2) Management in the cloud 

### Management Of The Cloud 

Includes all of the features that cloud providers give to manage own application  
Some types are:  
Templates  
Automation  
Scaling  
Monitoring and alerts  
Self-healing

### Management In The Cloud 

These are the features given by cloud providers to manage resources
Some types are:  
Web portals  
Command line interfaces  
APIs  
PowerShell 

# Cloud Service Types 

There are primarily three types  
1) Infrastructure as a Service(IaaS)  
2) Platform as as Service(PaaS)
3) Software as a Service(SaaS)

#### What is "As a Service"

You can rent the service for a short time rather than owning it  
No commitment and usage as needed by the customer  
Pay only for what the customer used  

## Infrastructure as a Service(IaaS)

These are essential services of IT like  
1) computing  
2) Storage  
3) Networking  

These are cloud equivalents for realworld hardware.  


One example is azure  
Pay by the second for what the customer uses  
Many choices of CPU's, RAM, etc.  

#### IaaS Storage

Azure Storage is one example  
Can handle blobs, files, queues and tables  

#### IaaS Networking

Virtual Networking is one example  
Here, the virtual network donot cost anything and bandwidth is the one that costs.  
There are ingress(data entering azure) and egress(data leaving azure) bandwidth costs.  

## Platform as as Service(PaaS)

PaaS includes a service layer on the top os IaaS. Like Middleware, development tools, database server and more.  

#### PaaS Computing 

One example is Azure App Service where we simply upload the code and configurations to azure, and it runs the code without needing 
to worry about the VM underneath  
Includes sacling features, CI/CD, containers, staging and development environments, etc  

#### PaaS Storage

Azure SQL database is an example  
Freed from worrying about the server VM itself or the other harware component that affect the storage.  

#### PaaS Networking

Azure front door is an example  
These are software application that perform networking application.  

## Software as a Service(SaaS)

These are apps that are ready to use and customer needs to simply set it up and use it  

## Serverless

Serverless computing in Azure allows you to build and deploy applications without managing the underlying infrastructure. 
Here we donot specificaaly pick the hardware. Basically paying for the service and not the hardware.  
