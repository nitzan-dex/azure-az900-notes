### Describe Azure regions, region pairs, and sovereign regions

**Region** - Geographical designation of several AZs. 
**AZ** Smaller geographical designations of one or more data centers. 

**Region pairs**
Some are 2-way some are 1-way.
Region pairs must be _at least_ 300 miles away from each other.  

**Sovereign regions** are Azure instances that are isolated from the "main" Azure instance, and are used for organizations that need to comply with certain regulations. E.g - Azure China


### Describe Azure resources and resource groups
- A resource must belong to a single resource group.
- Hold resources with a shared lifecycle 
- Resources inherits properties form their Resource group
  
  
### Describe subscriptions
A way of organizing resource groups and in terms of 
1. billing
2. access



Why to use another Subscription
- Subscription limits
- Diffrent Payment methods
- Logical Organisation

### Describe management groups
Management groups have one or more subscriptions.

### Describe the hierarchy of resource groups, subscriptions, and management groups
In order of descending specificity:
resouce -> resouce group -> subscription -> management group
