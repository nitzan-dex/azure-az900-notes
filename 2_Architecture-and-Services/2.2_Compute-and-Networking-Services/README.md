### Compare compute types, including container instances, virtual machines (VMs), and functions
- VMs: Slow to spin up.
- Containers: Less control, easier to scale.
- Azure Container Instance: Serverless Containers W/O Orchestration.
- AKS: Mangaged k8s
- Azure Functions: Event-driven, serverless, potentially cheaper due to no uptime costs. 

### Describe VM options, including Azure Virtual Machines, Azure Virtual Machine Scale Sets, availability sets, and Azure Virtual Desktop


**VM Scale Sets** enable the creation and management of identical, load-balanced VMs that adjust to demand automatically or on a set schedule. 

**VM Availability Sets** group VMs to promote HA
- update domain: Group VMs so that every VM in the group can reboot at the same time during an update without compromising availability. Only one update domain would be rebooted at a time.  
- fault domain: Group VMs so that each group has a separate power source and network switch.

**Azure Virtual Desktop** 
Hosts a Windows desktop on the cloud that's accessible across devices and OS's.  

- User login to this desktop can be managed from Entra ID.
- Supports multi-session windows 10 or 11 deployment, which regular VMs can't do.

### What is Azure Batch? 
A platform for that creates and manages a pool of virtual machines, intended for large-scale _parallel_ and _high-performance computing_.

### Describe application hosting options, including web apps, containers, and virtual machines
== Do it == 

### Describe the resources required for virtual machines
- Virtual Disk
- VNET
- Virtual NIC
- NSG
- Public IP Address

### Describe application hosting options, including the Web Apps feature of Azure App Service, containers, and virtual machines
Use VMs or containers.

You can also use **Azure App Service**, which will come with the following things built in:
- continuous deployment from a Git repo
- secured endpoints
- auto-scaling
- load balancing
- supports multiple programming languages

### Describe virtual networking, including the purpose of Azure Virtual Networks, Azure virtual subnets, peering, Azure DNS, Azure VPN Gateway, and Azure ExpressRoute
Virtual networks are what allow your resources to communicate with each other, and to your on-premises servers.  

**Azure Virtual Network** A logical representation of
your network in Azure
- Region
- VMs in different VNETS cannot communicate by default

 **Subnets** Segment address space of
VNET to create sub-networks
- VMs in different subnets within a VNET can
communicate by default!

A **P2S VPN Gateway** is how a secure connection is established between an Azure VNet and an individual computer.  

**VNet peering** and **Azure VPN Gateway(S2S VPN Gateway)** connect and encrypt communications between Azure VNets, and between on-premises networks and VNets.

**Azure ExpressRoute** is a way to connect vnets without using the public internet. The three models that ExpressRoute supports are:  
- CloudExchange colocation
- Point-to-point Ethernet connection 
- Any-to-any connection

VNets enable traffic filtering with security groups

**Azure DNS** is adomain hosting service who offers:
- anycast networking: DNS queries are answered by the closest available DNS server.
- Uses Azure RBAC
- monitor modifications to a resource
- resource locking
- private DNS domains and zones

**you can't register a domain name using Azure DNS**. 

### Describe Virtual Private Networks (VPNs)
A VPN is an encrypted tunnel over another network,. VPN Gateways are either:
- policy-based
- route-based

A VNet can have only one VPN gateway, but it can connect to multiple targets.

For HA,VPN gateways have several configuration options. By default, they are configured to be `active/standby`

