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
1) Computing  
2) Storage  
3) Networking  

These are cloud equivalents for realworld hardware.  


One example is VM's in Azure and EC2(Elastic Cloud Computing) in AWS
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

One example is Azure App Service,Azure SQL Database,Azure Cosmos DB,Azure Functions where we simply upload the code and configurations to azure, and it runs the code without needing 
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

 
Serverless computing in Azure allows you to build and deploy applications without managing the underlying infrastructure. 
Here we donot specifically pick the hardware. Basically paying for the service and not the hardware.  

# Core Azure Architecture 

## Region 

Areas of world where azure has set of datacenters.  
Not necessarily countires but it can be a place of the county. Usually each region is connected to another region to make a region pair.  
Region pairs have highest speed connections and speical treatment during azure updates.  

## Soverring Regions 

These are not connected to the Azure public cloud. Customer require approval to create a subscription.  

## Availabilty Zones

Azure availabilty zones are physically separate locations within each azure region. They are independent from one another.  
This allows cloud resources (like virtual machines or databases) to replicate across zones for better disaster recovery.  

## Resource

Any azure service that customers have access to, such as VM, DB, etc.  
Each resource has a name and sometimes they may need to be unique. Most resources have cost associated with them.  


## Resource Groups

A logical grouping of resources. All the services in a resource group have a similar lifecycle i.e deploy together, delete together. 
Any resoruce can access anyother resource in a resource group.
Resource groups make the management of Azure resources easier. With a resource group, you can allow a user to manage all resources in the resource group, such as virtual machines, websites, and subnets. 
The permissions you apply to the resource group apply to all resources contained in the resource group.  

## Subscriptions 

In Azure, a subscription is an organizational unit used to manage access, resource creation, and 
billing for the resources and services you use in the cloud. It serves as a container for all your Azure resources (such as virtual machines, databases, and storage accounts) 
and provides a way to logically group these resources. Each subscription is 
tied to a billing account and can be associated with specific billing, quotas, and policies.

## Management Groups

In Microsoft Azure, management groups are a way to organize and manage multiple Azure subscriptions at a higher level. They allow you to group 
subscriptions together for unified policy and access management, making it easier to govern large-scale environments, 
especially in enterprises with multiple departments, projects, or business units.

![](/.img/management_group.png)

## Computing Services 

Compute services in the cloud refer to resources provided by azure that allow users to run an application process the data and execute a program.  

#### Virtual Machines 

These are best examples of IaaS. 
A virtual machine is a single software package with hardware resources, an operating system, and all its applications. 
You get control over the OS and can install applications, but you're responsible for managing the VMs. 

We scale the VM's to handle more traffic whenever necessary. It can be done in 2 ways:-  
1) ScaleUP:- We can increase the size of VM easily by turning a 4CPU vm into an 8CPU vm in minutes.  
2) ScaleOut:- One more way is to add more VM's and have them work together to hanfle more traffic.  

#### Virtual Machines Scale Sets(VMSS) 

A group of VM that can grow and shrink in quantity based on predefined rule. 

This can be done by monitoring demand, predfined schedules where more traffic can be found, and many more way.  

### Availabilty Sets

You have multiple VM with same identical functions. We need a differentiating factor that seperates one from the other.  

#### How is it achieved

1) Fault Domains(FDs):-  A fault domain is a group of resources that share the same power source and physical network switch. If a power or network failure occurs, 
all VMs in the same fault domain are impacted. By placing VMs in different fault domains, you're reducing the chance that all your VMs will go down at the same time.  
2) Update Domains (UDs): These help during maintenance events. Update domains are groups of VMs that get updated or rebooted at the same time when there's a scheduled maintenance. 
By distributing your VMs across update domains, only a portion of your VMs are taken offline during maintenance.  

### Proximity Groups

This is opposite to Availabilty Sets. In the multiple VM that have an identical function are arranged together.  
This increases the chance of less availabilty of a system in case of any unplanned outages.  

### App Services(Web Apps)

This comes under PaaS. In this no full complete over server is there. We package the code and configurations and the azure will 
run the code based on the promised performance levels.  

### Contianer Services

Containers are lightweight, standalone packages that bundle an application with all its dependencies, making them portable and consistent across different environments. 
Cloud container services help automate and simplify the deployment, scaling, and management of these containers.

Examples:-

Azure Container Instances (ACI):- ACI is a service that lets you run containers without the need to manage virtual machines or Kubernetes clusters.  
Azure Kubernetes Service (AKS)::- AKS is Azure's fully managed Kubernetes service, offering simplified Kubernetes cluster management.   

### Azure Functions

Function allows you to run small pieces of code in response to events occuring without worrying about managing the underlying infrastructure. You only pay for the compute resources you use while the function is executed and how many times the function is used. The pricing is very less compared to counterparts.  
These functions have many features:-  
1) Serverless :- You don't need to provision or manage servers. The cloud platform automatically scales resources up or down based on demand, and you're billed only for the time your function code runs.  
2) Scalability :- Azure Functions automatically scale out based on the number of incoming events. It can handle multiple simultaneous function executions without the need for manual intervention.
3) Integrations with Azure Services:- Azure Functions integrates deeply with other Azure services like Azure Storage, Azure Cosmos DB, Azure Event Grid, Azure Logic Apps, and more. This allows seamless workflows and event-driven architectures.  

### Virtual Networks 

Virtual Networks (VNets) in Azure are fundamental building blocks for private networking in Azure. They allow you to create isolated network environments within the Azure cloud, where you can securely run and manage your resources such as virtual machines, databases, and web services 
In azure 2 VM's cannot connect to eachother. So, we use virutal networks to connect the VM's.  
These are cosidered as IaaS.  
These VNets's are given addresses of IPV4 or IPV6 or somtimes both. These addresses cannot be accessed outside of azure and by other networks in azure.  

#### Subnets 

All VNets are divided into one or more subnets. These subnets are assigned a IP address which must exists in the address space 
of the parent VNets.  
Usually there is a security layer between subnets and the traffic must match predefined ruleset to pass.  

### Network Security Groups

Also called as NSG. An Access Control List(ACL) that blocks traffic that is inbound and outbound from a subnet unless it matches some predefined rules. These rules are based on 
source IP, source port, destination IP, destination port, and protocol(5-tuple match).  

### Peering 

In general communication is blocked between 2 subnets on different networks, so to get around that we setup a peering relationship between the 2 subnets 
which allows communication between the VM on one network with a VM on another network.  
