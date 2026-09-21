# Cloud and Virtualization

## Cloud Types

There are four primary cloud models

### Public Cloud-based applications and services

offered in a public cloud are made available to the general population. Services may be free or are offered on a pay-per-use model, such as paying for online storage. The public cloud uses the internet to provide services.

### Private clouds

Cloud-based applications and services offered in a private cloud are intended for a specific organization or entity, such as the government. A private cloud can be set up using the private network of an organization, though this can be expensive to build and maintain. A private cloud can also be managed by an outside organization with strict access security.

### Hybrid clouds

A hybrid cloud is made up of two or more clouds (example: part private, part public), where each part remains a separate object, but both are connected using a single architecture. Individuals on a hybrid cloud would be able to have degrees of access to various services based on user access rights.

### Community clouds

A community cloud is created for exclusive use by a specific community. The differences between public clouds and community clouds are the functional needs that have been customized for the community. For example, healthcare organizations must remain compliant with policies and laws (e.g., HIPAA) that require special authentication and confidentiality.

## Advantages of Virtualization

One major advantage of virtualization is overall reduced cost:

1. Less equipment is required - Virtualization enables server consolidation, which requires fewer physical devices and lowers maintenance costs.
2. Less energy is consumed - Consolidating servers lowers the monthly power and cooling costs.
3. Less space is required - Server consolidation reduces the amount of required floor space.

### Additional benefits of virtualization:

- Easier prototyping - Self-contained labs, operating on isolated networks, can be rapidly created for testing and prototyping network deployments.
- Faster server provisioning - Creating a virtual server is far faster than provisioning a physical server.
- Increased server uptime - Most server virtualization platforms now offer advanced redundant fault tolerance features.
- Improved disaster recovery - Most enterprise server virtualization platforms have software that can help test and automate failover before a disaster happens.
- Legacy support - Virtualization can extend the life of OSs and applications providing more time for organizations to migrate to newer solutions

## SERVER TYPES

Web Server
Windows OS
Hardware
CPU, Memory, NIC, Disk
Email Server
Windows OS
Hardware
CPU, Memory, NIC, Disk
SQL Server
Windows OS
Hardware
CPU, Memory, NIC, Disk
File Server
Windows OS
Hardware
CPU, Memory, NIC, Disk
DHCP Server
Windows OS
Hardware
CPU, Memory, NIC, Disk
Active Directory (AD) Server
Windows OS
Hardware
CPU, Memory, NIC, Disk
AAA RADIUS Server
Linux
Hardware
CPU, Memory, NIC, Disk
Network Management Server (NMS)
Linux
Hardware
CPU, Memory, NIC, Disk

## Hypervisors

The hypervisor is a program, firmware, or hardware that adds an abstraction layer on top of the physical hardware. The abstraction layer is used to create virtual machines which have access to all the hardware of the physical machine such as CPUs, memory, disk controllers, and NICs. Each of these virtual machines runs a complete and separate operating system. With virtualization, it is not uncommon for 100 physical servers to be consolidated as virtual machines on top of 10 physical servers that are using hypervisors.

2 approaches: bare metal vs hosted

### TYPE 1 Hypervisor - “Bare Metal”

Type 1 hypervisors AKA “bare metal” approach because the hypervisor is installed directly on the hardware. Type 1 hypervisors are usually used on enterprise servers and data center networking devices.
With Type 1 hypervisors, the hypervisor is installed directly on the server or networking hardware. Then, instances of an OS are installed on the hypervisor, as shown in the figure. Type 1 hypervisors have direct access to the hardware resources; therefore, they are more efficient than hosted architectures. Type 1 hypervisors improve scalability, performance, and robustness.

TYPE 2 Hypervisor - “Hosted”
Type 2 hypervisor is software that creates and runs VM instances. The computer, on which a hypervisor is supporting one or more VMs, is a host machine. Type 2 hypervisors are also called hosted hypervisors. This is because the hypervisor is installed on top of the existing OS, such as macOS, Windows, or Linux. Then, one or more additional OS instances are installed on top of the hypervisor, as shown in the figure. A big advantage of Type 2 hypervisors is that management console software is not required.

## LearningOutcomes:

Cloud, Cloud Services

In general, when talking about the cloud, we are talking about data centers, cloud computing, and virtualization. Data centers are usually large facilities which provide massive amounts of power, cooling, and bandwidth. Only very large companies can afford their own data centers. Most smaller organizations lease the services from a cloud provider.

Cloud Services

- SaaS SOFTWARE
- PaaS PLATFORM
- IaaS INFRASTRUCTURE

4 primary cloud models:
Public
Private,
Hybrid
Community

Virtualization is the foundation of cloud computing. Without it, cloud computing, as it is most-widely implemented, would not be possible. Virtualization means creating a virtual rather than physical version of something, such as a computer. An example would be running a "Linux computer" on your Windows PC.

![module2Pass](image.png)
