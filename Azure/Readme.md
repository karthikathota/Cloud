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
4) 