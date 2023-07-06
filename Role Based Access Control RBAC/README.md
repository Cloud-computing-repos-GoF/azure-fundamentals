## Azure Role-Based Access Control RBAC

It's a good security practice to grant users only the rights they need to perform their job, and only to the relevant resources. Role-based access control is applied to a scope, which is a resource or set of resources that this access applies to.  

Here's a diagram that shows the relationship between roles and scopes.

![Responsibility Levels for Services](https://github.com/Cloud-computing-repos-GoF/azure-fundamentals/blob/master/images/RBAC_azure.png)

Scopes include:   

1. A management group (a collection of multiple subscriptions).  
2. A single subscription.   
3. A resource group.  
4. A single resource.  

Observers, Users managing resources, Admins, and Automated processes illustrate the kinds of users or accounts that would typically be assigned each of the various roles.   

When you grant access at a parent scope, those permissions are inherited by all child scopes. For example:  

* When you assign the Owner role to a user at the management group scope, that user can manage everything in all subscriptions within the management group.   
* When you assign the Reader role to a group at the subscription scope, the members of that group can view every resource group and resource within the subscription.  
* When you assign the Contributor role to an application at the resource group scope, the application can manage resources of all types within that resource group, but not other resource groups within the subscription.  

### Lock levels

Apply for resources, resource groups and subscriptions.  

* CanNotDelete  
* ReadOnly  

To make the protection process more robust, you can combine resource locks with Azure Blueprints. Azure Blueprints enables you to define the set of standard Azure resources that your organization requires. For example, you can define a blueprint that specifies that a certain resource lock must exist. Azure Blueprints can automatically replace the resource lock if that lock is removed.   

### Tags

One way to organize related resources is to place them in their own subscriptions. You can also use resource groups to manage related resources. Resource tags are another way to organize resources. Tags provide extra information, or metadata, about your resources. This metadata is useful for:  

* **Resource management Tags** enable you to locate and act on resources that are associated with specific workloads, environments, business units, and owners.  
* **Cost management and optimization Tags** enable you to group resources so that you can report on costs, allocate internal cost centers, track budgets, and forecast estimated cost.  
* **Operations management Tags** enable you to group resources according to how critical their availability is to your business. This grouping helps you formulate service-level agreements (SLAs). An SLA is an uptime or performance guarantee between you and your users.   
* **Security Tags** enable you to classify data by its security level, such as public or confidential.   
* **Governance and regulatory compliance Tags** enable you to identify resources that align with governance or regulatory compliance requirements, such as ISO 27001. Tags can also be part of your standards enforcement efforts. For example, you might require that all resources be tagged with an owner or department name.   
* **Workload optimization and automation Tags** can help you visualize all of the resources that participate in complex deployments. For example, you might tag a resource with its associated workload or application name and use software such as Azure DevOps to perform automated tasks on those resources.   


You can also manage tags by using Azure Policy. For example, you can apply tags to a resource group, but those tags aren't automatically applied to the resources within that resource group. You can use Azure Policy to ensure that a resource inherits the same tags as its parent resource group.

### Azure Policy

Azure Policy is a service in Azure that enables you to create, assign, and manage policies that control or audit your resources. These policies enforce different rules across all of your resource configurations so that those configurations stay compliant with corporate standards.

