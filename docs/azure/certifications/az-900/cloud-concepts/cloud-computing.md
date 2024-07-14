Traditionally organizations have relied on on Prem data centers. Due to the many benefits of the cloud (rapid deployment, scalability, disaster recovery, cost savings, etc), Many organizations are moved away from traditional data centers. Notably, Netflix decommissioned its data centers and are fully in the public cloud.

## Cloud Models
Organizations can decide to partially or fully integrate with the cloud. Organizations have three cloud models to choose from: private, public, or hybrid.

### Private
Physical servers remain in house. Azure implements this via Azure stack. Azure stack is a set of vendor specific servers and Microsoft software. The servers are shipped to the customers’ data centers. The Azure stack software virtualizes the servers and provides a UI like the Azure portal. This has the benefit of giving the customer granular control and full control of data like PHI. However, customers still need to maintain the data centers.

### Public
This is a fully managed model. Customers use Microsoft's data centers. Physical server resources are shared with other customers. There is an option for a non-shared isolated server, but the cost is much more. Resources are fully managed by Microsoft. This enables the full benefit of the cloud.

### Hybrid
This model is a combination of private and public. An example is having an on-prem database while having a web app deployed in the public cloud. A hybrid approach is typically used for incremental migration to the public cloud. Another good use case is for keeping PHI inside the organization.

### Public vs Private Pros/Cons
| Feature       |  Public       | Private      |
| ------------- | ------------- | ------------- |
| Granular control | N | Y |
| Limited PHI Exposure | N | Y |
| On demand scalability | Y | Y |
| Manage Disaster Recovery | Y | N |
| Maintenance Free | Y | N |
| Rapid Deployment | Y | Y |
| No Capital Expenditure | Y | N |

## Shared Responsibility Model
The shared responsibility model, models the responsibility relationship between the application, customer, and Azure. Application to fully operate, layers must be managed. There are 8 layers: Network, storage, servers (physical hosts, data center, physical network, etc), Virtualization, operating system, runtime, and application. At any given layer, Azure, the customer, or both are responsible. The responsible party is dependent on the chosen service type.

## Service Types
There are three service models. Starting from self-managed to fully managed they are, IaaS, PaaS, and SaaS.

### On-prem
This is not a service type but it's worth talking about. On-prem is a traditional data center. Organizations are responsible for everything (maintenance, cooling, software updates, server upgrades, etc).

### Iaas
Infrastructure as a service is a service type where Azure physically hosts the data center. This is a low-level basic cloud service type. Azure handles all the server provisioning (memory, storage, and physical networking). A virtual machine is an example of IaaS resource.

### Paas
This stands for platform as a service. Azure handles things like networking, runtime, operating systems, disaster recovery, scaling, etc. With platform as a service, multiple server instances can be provisioned with little to no maintenance. App service is an example of this. 

Both the customer and Microsoft must ensure the security of the network. Customers should keep accounts and data secure. The network should be properly managed utilizing such concepts as network security groups.

### SaaS
Software as a service is the most high-level service type. It is fully managed. Customers should keep data and user accounts secure. An example of software as a service is PowerBI, Jira, Office 365, etc.