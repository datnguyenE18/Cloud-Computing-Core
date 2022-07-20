# **Types of VMs**


A few different types of VMs that can be provisioned in the cloud


- **Shared ( or Public) Cloud VMs** are provider-managed, multi-tenant deployments that can be provisioned on-demand with predefined sizes. 
 
  - Being multi-tenant means that the underlying physical server is virtualized and is shared across other tenants or users.



  - Rather than pick from only pre-defined sizes, some providers also offer custom configurations that allow users to define the number of cores and RAM and local storage characteristics



  - Public VMs are usually priced by time



- **Transient (or Spot) VMs** take advantage of unused capacity in a cloud data center. Cloud providers make this unused capacity available to users at a much lower cost than regular VMs of similar sizes. 
 
  - the Cloud provider can choose to de-provision them at any time
 
  - these VMs are great for non-production workloads such as testing and developing applications. Or running stateless workloads, testing scalability, or running big data and high performance computing (HPC) workloads at a low cost



- **Reserved VMs** that allow you to reserve capacity and guarantee resources for future deployments
 
- **Dedicated hosts** that offer single-tenant isolation
