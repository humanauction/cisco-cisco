# Module 1: Networking Design

## Networking Design

there are four basic characteristics that network architects must address to meet user expectations:

- Fault Tolerance
- Scalability
- Quality of Service (QoS)
- Security

#### Fault tolerance

fault tolerant network is one that limits the number of affected devices during a failure
multiple paths to a destination is known as redundancymore redundancy = more fault tolerant network

packet-switched network is one way that reliable networks provide redundancy. Packet switching splits traffic into packets that are routed over a shared network
N.B. routers within the network switch the packets based on the condition of the network at that moment so all the packets in a single message could take very different paths to the same destination

#### QoS

congestion = demand for bandwidth exceeds the amount available
Network bandwidth is measured in the number of bits that can be transmitted in a single second, or bits per second (bps)

QoS policy = protocol so the router can manage the flow of data and voice traffic, giving priority to voice communications if the network experiences congestion.
focus of QoS i= prioritize time-sensitive traffic. The type of traffic, not the content of the traffic, is what is important.

#### Net Sec

Network administrators must address two types of network security concerns: network infrastructure security and information security.
Securing the network infrastructure includes physically securing devices that provide network connectivity and preventing unauthorized access to the management software that resides on them

Network administrators must also protect the information contained within the packets being transmitted over the network, and the information stored on network attached devices. In order to achieve the goals of network security, there are three primary requirements.

#### CIA

Confidentiality - Data confidentiality means that only the intended and authorized recipients can access and read data.
Integrity - Data integrity assures users that the information has not been altered in transmission, from origin to destination.
Availability - Data availability assures users of timely and reliable access to data services for authorized users.

## Physical and Logical Addresses

MAC address does not change. physically assigned to the host NIC
AKA physical address. The physical address remains the same regardless of where the host is placed on the network.
The IP address is like a persons address
AKA logical address. assigned logically based on host location.
The IP address AKA network address, is assigned to each host by a network administrator based on the local network.
IP addresses contain two parts.

1. identifies the network portion.
   The network portion of the IP address will be the same for all hosts connected to the same local network.
2. identifies the individual host on that network.
   Within the same local network, the host portion of the IP address is unique to each host

Both the physical MAC and logical IP addresses are required for a computer to communicate on a hierarchical network

## Hierarchical Analogy

MAC address indicates the individual identity of a specific host, but it does not indicate where on the network the host is located.

Ethernet technology generates a large amount of broadcast traffic in order for hosts to communicate. Broadcasts are sent to all hosts within a single network. Broadcasts consume bandwidth and slow network performance.On an Ethernet network, the host MAC address is similar to a person's name. A MAC address indicates the individual identity of a specific host, but it does not indicate where on the network the host is located. If all hosts on the internet (millions and millions of them) were each identified by their unique MAC address only, imagine how difficult it would be to locate a single one.
Additionally, Ethernet technology generates a large amount of broadcast traffic in order for hosts to communicate. Broadcasts are sent to all hosts within a single network. Broadcasts consume bandwidth and slow network performance. What would happen if the millions of hosts attached to the internet were all in one Ethernet network and were using broadcasts?
For these two reasons, large Ethernet networks consisting of many hosts are not efficient. It is better to divide larger networks into smaller, more manageable pieces. One way to divide larger networks is to use a hierarchical design model.

### 1.2.6 Access, Distribution, and Core

ADC
IP traffic is managed based on the characteristics and devices associated with each of the three layers of the hierarchical network design model: Access, Distribution and Core.Access Layer
The access layer provides a connection point for end user devices to the network and allows multiple hosts to connect to other hosts through a network device.
usually a switch or a wireless access point.
Typically, all devices within a single access layer will have the same network portion of the IP address.
If a message is destined for a local host, based on the network portion of the IP address, the message remains local.
If it is destined for a different network, it is passed up to the distribution layer.
Switches provide the connection to the distribution layer devices, usually a Layer 3 device such as a router or Layer 3 switch.

Distribution Layer
The distribution layer provides a connection point for separate networks and controls the flow of information between the networks.
Typically contains more powerful switches than the access layer PLUS routers for routing between networks.
Distribution layer devices = control the type and amount of traffic that flows access layer -> core layer.

Core Layer
The core layer is a high-speed backbone layer with redundant (backup) connections.
responsible for transporting large amounts of data between multiple end networks. Core layer devices typically include very powerful, high-speed switches and routers.
main goal = transport data quickly.

### unit Learning Outcome

### Reliable Networks
As networks evolve, we have learned that there are four basic characteristics that network architects must address to meet user expectations: Fault Tolerance, scalability, QoS, and security.  
A fault tolerant network limits the number of affected devices during a failure. It allows quick recovery when such a failure occurs. These networks depend on multiple paths between the source and destination of a message. If one path fails, the messages are instantly sent over a different link.  
A scalable network expands quickly to support new users and applications. It does this without degrading the performance of services that are being accessed by existing users. Networks can be scalable because the designers follow accepted standards and protocols.  
QoS is an increasing requirement of networks today. As data, voice, and video content continue to converge onto the same network, QoS becomes a primary mechanism for managing congestion and ensuring reliable delivery of content to all users. Network bandwidth is measured in bps. When simultaneous communications are attempted across the network, the demand for network bandwidth can exceed its availability, creating network congestion. The focus of QoS is to prioritize time-sensitive traffic. The type of traffic, not the content of the traffic, is what is important.  
Network administrators must address two types of network security concerns: network infrastructure security and information security. Network administrators must also protect the information contained within the packets being transmitted over the network, and the information stored on network attached devices. There are three primary requirements to achieve the goals of network security: Confidentiality, Integrity, and Availability.

### Hierarchical Network Design

The hierarchical network design is a method of organizing a network into distinct layers, each with a specific role and responsibility. This approach helps to manage complexity and improve the overall performance and reliability of the network.

The hierarchical network design is a method of organizing a network into distinct layers, each with a specific role and responsibility. This approach helps to manage complexity and improve the overall performance and reliability of the network.

Network administrators must address two types of network security concerns: network infrastructure security and information security. Network administrators must also protect the information contained within the packets being transmitted over the network, and the information stored on network attached devices. There are three primary requirements to achieve the goals of network security: Confidentiality, Integrity, and Availability.

IP addresses contain two parts. One part identifies the network portion. The network portion of the IP address will be the same for all hosts connected to the same local network. The second part of the IP address identifies the individual host on that network. Both the physical MAC and logical IP addresses are required for a computer to communicate on a hierarchical network.

The Network and Sharing Center on a PC shows your basic network information and set up connections, including your active networks and whether you are connected wired or wirelessly to the internet and within your LAN. You can view the properties of your connections here.

On an Ethernet network, the host MAC address is similar to a person's name. A MAC address indicates the individual identity of a specific host, but it does not indicate where on the network the host is located. If all hosts on the internet (millions and millions of them) were each identified by their unique MAC address only, imagine how difficult it would be to locate a single one. It is better to divide larger networks into smaller, more manageable pieces. One way to divide larger networks is to use a hierarchical design model.  
Hierarchical networks scale well. The access layer provides a connection point for end user devices to the network and allows multiple hosts to connect to other hosts through a network device, usually a switch or a wireless access point. Typically, all devices within a single access layer will have the same network portion of the IP address. The distribution layer provides a connection point for separate networks and controls the flow of information between the networks. Distribution layer devices control the type and amount of traffic that flows from the access layer to the core layer. The core layer is a high-speed backbone layer with redundant connections. It is responsible for transporting large amounts of data between multiple end networks. The main goal of the core layer is to transport data quickly.

![alt text](modulePass1.png)
