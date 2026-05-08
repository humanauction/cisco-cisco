# Cisco Learning Dump

## Why

just somewhere to put the stuff I learn about Cisco and networking plus badges, etc... for later reference.

## Packet Tracer

<img src="packetTracer/images/badge-packet-tracer.png" alt="Packet Tracer Badge" height="120px">

### 1.Intro to

Skills Learned: Cisco Packet Tracer to visualize and simulate a network using everyday examples.

### 2.Exploring Networking

Skills Learned: connect, configure network devices, wireless devices, verify connectivity.

### 3.IoT

Skills Learned: IoT, Network Simulation, Environmental Controls, Programming, JavaScript, Python, Visual Blocky.

#### Module 1: Create Your Own Smart Home Network

In simple terms, the IoT is a collection of networked sensors, actuators, and smart devices that gather and share data. To connect the devices to your network, you need a home gateway or registration server. To control the devices, you have two options: you can interact directly with a device, or you can connect remotely over the network using a remote PC, tablet, or smart phone. You can connect and control smart devices using either a Home Gateway device or a remote registration server. The Home Gateway device acts as a local connection to your IoT smart devices. The Home Gateway device provides an IoT registration service that is always turned on, and an auto discovery service for Things in the local Ethernet and wireless network. When a home gateway device has been added to the logical workspace and you click the device, you will see the following:

- Physical tab – The device has an internet port, four LAN ports, and multiple antennae.
  Config tab – This shows the interfaces and network settings that are configurable.
  GUI tab – This shows the registration server inside the device that allows for interaction with IoT devices. It is on by default but can be turned off.
  Attributes tab – This is blank by default but can show features and values e.g. MTBF, cost, power source, and wattage. IoT devices can also be registered to a dedicated Registration Server for remote monitoring, control, or programming. The dedicated registration server has the additional benefit of being able to provide many other services to your network, e.g. Web, DHCP, DNS, email, and FTP.

#### Module 2: Environmental Controls and IoT Things in Packet Tracer

In the Physical Workspace there are containers. Containers include the intercity, city, buildings, and wiring closets. They all have their own set of environmental values. If there are no devices configured to affect the environment, their values are looped on a 24-hour cycle. Different containers may have different levels of insulation and thus different transference values. The transference values determine the rate that the child container converges with the parent container, and it works the same way for all environment types. To be able to provide true IoT solutions, it is critical to have programming knowledge. Packet Tracer provides supports JavaScript, Python, and Visual Blocky. Important terms and concepts:

- Current time – Time inside a container that increments by 30 minute increments. Every 1 second in real time equates to 30 minutes in “Container” time. The timer goes from 0 (midnight) to 11:59.
  KeyFrame – Represents a single moment in time.
  KeyFrame graph – A graph that shows the value of environmental elements at any given point in time throughout the day.
  Transference - Values that determine the rate that the child container converges with the parent container and works the same way for all environment types.
  You can use programming language to modify environmental elements within a container. You can even create a new IoT “Thing” in Packet Tracer. First, decide what the Thing will do, how it will connect to the network, and how it will work. You also need to identify an existing Thing that functions in a similar manner as the new Thing. The existing script can then be modified to create the new script. Clicking any IoT device that is in the workspace will reveal the specifications about that device. The specifications include:

- Features – How the device works or what it does. Devices can generate high and low values based on a button being pushed or toggled on and off or they can detect certain environmental values (eg. smoke or sunlight).
  Usage – Things may connect to other IoT devices in order to receive LOW or HIGH inputs or it may read the variable set in the Environment object.
  Direct Control – Shows you what keystrokes will allow you to physically interact with the Thing.
  Local and Remote Control – Shows how to control the Thing locally or remotely (if applicable).
  Data Specifications – How the values are produced or the port/slot used to connect to the sensor.
  Example – Describes an example of how it works.

## Networking Basics

### Module 1

#### Learning outcomes

Network Types

The internet is not owned by any individual or group. The internet is a worldwide collection of interconnected networks (internetwork or internet for short), cooperating with each other to exchange information using common standards. Through telephone wires, fiber-optic cables, wireless transmissions, and satellite links, internet users can exchange information in a variety of forms.
Small home networks connect a few computers to each other and to the internet. The SOHO network allows computers in a home office or a remote office to connect to a corporate network, or access centralized, shared resources. Medium to large networks, e.g. those used by corporations and schools, can have many locations with hundreds or thousands of interconnected hosts. The internet is a network of networks that connects hundreds of millions of computers world-wide.
There are devices all around that you may interact with on a daily basis that are also connected to the internet. These include mobile devices e.g. smartphones, tablets, smartwatches, and smart glasses. Things in your home can be connected to the internet e.g. a security system, appliances, your smart TV, and your gaming console. Outside your home there are smart cars, RFID tags, sensors and actuators, and even medical devices which can be connected.

Data Transmission

The following categories are used to classify types of personal data:
Volunteered data - This is created and explicitly shared by individuals, e.g. social network profiles. This type of data might include video files, pictures, text, or audio files.
Observed data - This is captured by recording the actions of individuals, e.g. location data when using cell phones.
Inferred data -This is data e.g. a credit score, which is based on analysis of volunteered or observed data.

The term bit is an abbreviation of “binary digit” and represents the smallest piece of data. Each bit can only have one of two possible values, 0 or 1.

There are three common methods of signal transmission used in networks:
Electrical signals - Transmission is achieved by representing data as electrical pulses on copper wire.
Optical signals - Transmission is achieved by converting the electrical signals into light pulses.
Wireless signals - Transmission is achieved by using infrared, microwave, or radio waves through the air.

Bandwidth and Throughput

Bandwidth is the capacity of a medium to carry data. Digital bandwidth measures the amount of data that can flow from one place to another in a given amount of time. Bandwidth is typically measured in the number of bits that (theoretically) can be sent across the media in a second. Common bandwidth measurements are as follows:
Thousands of bits per second (Kbps)
Millions of bits per second (Mbps)
Billions of bits per second (Gbps)
Throughput does not usually match the specified bandwidth. Many factors influence throughput including:
The amount of data being sent and received over the connection
The latency created by the number of network devices encountered between source and destination
Latency refers to the amount of time, including delays, for data to travel from one given point to another.

### Module 2: Network Components, Types, Connections

Module Objective:
Explain network types, components, and connections.

Topic Title - Topic Objective
Clients and Servers - Explain the roles of clients and servers in a network
Network Components - Explain the roles of network infrastructure devices
ISP Connectivity Options - Describe ISP connectivity options

P2P
Peer-to-Peer Applications
A P2P application allows a device to act as both a client and a server within the same communication, as shown in the figure. In this model, every client is a server and every server is a client. P2P applications require that each end device provide a user interface and run a background service.

Some P2P applications use a hybrid system where resource sharing is decentralized, but the indexes that point to resource locations are stored in a centralized directory. In a hybrid system, each peer accesses an index server to get the location of a resource stored on another peer.

The network infrastructure contains three categories of hardware components, as shown in the figure:

End devices - phones, laptops, printers
An end device (or host) is either the source or destination of a message transmitted over the network, as shown in the animation. In order to uniquely identify hosts, addresses are used. When a host initiates communication, it uses the address of the destination host to specify where the message should be sent.

Intermediate devices - switches, routers, firewall appliances

Network media - WAN - used by ISPs, etc...
ISP Services
An ISP can be the local cable provider, a landline telephone service provider, the cellular network that provides your smartphone service, or an independent provider who leases bandwidth on the physical network infrastructure of another company.

Many ISPs also offer additional services to their contract subscribers, as shown in the figure. These services can include email accounts, network storage, and website hosting and automated backup or security services.

ISPs are critical to communications across the global internet. Each ISP connects to other ISPs to form a network of links that interconnect users all over the world. ISPs are connected in a hierarchical manner that ensures that internet traffic generally takes the shortest path from the source to the destination.

The internet backbone is like an information super highway that provides high-speed data links to connect the various service provider networks in major metropolitan areas around the world. The primary medium that connects the internet backbone is fiber-optic cable.

other connectivity options include:
Cellular
Cellular internet access uses a cell phone network to connect. Wherever you can get a cellular signal, you can get cellular internet access. Performance will be limited by the capabilities of the phone and the cell tower to which it is connected. The availability of cellular internet access is a real benefit for people in areas that would otherwise have no internet connectivity at all, or for people who are constantly on the move. The downside of cellular connectivity is that the carrier usually meters the bandwidth usage of the connection and may charge extra for bandwidth that exceeds the contract data plan.

Sat service
Satellite service is a good option for homes or offices that do not have access to DSL or cable. Satellite dishes (see figure) require a clear line of sight to the satellite and so might be difficult in heavily wooded areas or places with other overhead obstructions. Speeds will vary depending on the contract, though they are generally good. Equipment and installation costs can be high (although check the provider for special deals), with a moderate monthly fee thereafter. Like cellular access, the availability of satellite internet access is a real benefit in areas that would otherwise have no internet connectivity at all.

dialup
An inexpensive option that uses any phone line and a modem. To connect to the ISP, a user calls the ISP access phone number. The low bandwidth provided by a dial-up modem connection is usually not sufficient for large data transfer, although it is useful for mobile access while traveling. A modem dial-up connection should only be considered when higher speed connection options are not available.

#### Learning outcomes

Clients and Servers:
All computers connected to a network that participate directly in network communication are classified as hosts. Hosts can send and receive messages on the network. In modern networks, computer hosts can act as a client, a server, or both. The software installed on the computer determines which role the computer plays.
Client and server software usually run on separate computers, but it is also possible for one computer to run both client and server software at the same time. In small businesses and homes, many computers function as the servers and clients on the network. This type of network is called a P2P network. In larger businesses, because of the potential for high amounts of network traffic, it is often necessary to have dedicated servers to support the number of service requests. P2P networks are easy to set up, less complex, lower in cost, and can be used for simple tasks e.g. transferring files and sharing printers. However, there is no centralized administration. They have less security, are not scalable, and can perform slower.

Network Components:
There are symbols that represent various types of networking equipment. The network infrastructure is the platform that supports the network. It provides the stable and reliable channel over which our communications can occur. The network infrastructure contains three categories of hardware components: end devices, intermediate devices, and network media. Hardware is often the visible components of the network platform e.g. a laptop, PC, switch, router, wireless access point, or the cabling used to connect the devices. Components that are not visible include wireless media.
End devices, or hosts, form the interface between users and the underlying communication network. Some examples of end devices include:
Computers (workstations, laptops, file servers, web servers)
Network printers
Telephones and teleconferencing equipment
Security cameras
Mobile devices (e.g. smartphones, tablets, PDAs, and wireless debit/credit card readers and barcode scanners)

ISP Connectivity Options:
An ISP provides the link between the home network and the internet. An ISP can be the local cable provider, a landline telephone service provider, the cellular network that provides your smartphone service, or an independent provider who leases bandwidth on the physical network infrastructure of another company. Each ISP connects to other ISPs to form a network of links that interconnect users all over the world. ISPs are connected in a hierarchical manner that ensures that internet traffic generally takes the shortest path from the source to the destination.
The interconnection of ISPs that forms the backbone of the internet is a complex web of fiber-optic cables with expensive networking switches and routers that direct the flow of information between source and destination hosts.
For a home user, connecting to the ISP is a fairly uncomplicated process. This is the most common connection option. It consists of using a wireless integrated router to connect to the ISP. The router includes a switch to connect wired hosts and a wireless AP to connect wireless hosts. The router also provides client IP addressing information and security for inside hosts. The two most common methods are cable and DSL. Other options include cellular, satellite, and dial-up telephone.

### Module 3: Wireless and Mobile Networks

Module Objective:
wireless networks - different network types used by cell, mobile devices
Mobile device Connectivity - configuring mobile devices for wireless connectivity

#### Learning Outcomes

Wireless Networks:
Mobile phones use radio waves to transmit voice signals to antennas mounted on towers located in specific geographic areas. When a telephone call is made, the voice signal is relayed from one tower to another tower until it is delivered to its destination. This type of network is used when you make a phone call to another mobile phone or to a wired telephone. It is also used to send text messages directly from the phone. The most common type of cellular telephone network is called a GSM network. The abbreviations 3G, 4G, 4G-LTE, and 5G are used to describe enhanced cell phone networks that are optimized for the fast transmission of data. Currently, 4G still dominates as the current mobile network used by most phones.
In addition to the GSM and 4G/5G transmitters and receivers, smartphones make connections in a variety of ways.
Wi-Fi transmitters and receivers located within the smartphone enable the phone to connect to local networks and the internet. Wi-Fi networks are usually privately owned but often provide guest or public access hotspots. A hotspot is an area where Wi-Fi signals are available.
Bluetooth is wireless technology that allows devices to communicate over short distances. Multiple devices can be connected at the same time with Bluetooth.
NFC is a wireless communication technology that enables data to be exchanged by devices that are in very close proximity to each other, usually less than a few centimeters.

Mobile Device Connectivity
Almost all mobile devices are capable of connecting to Wi-Fi networks. These precautions should be taken to protect Wi-Fi communications on mobile devices:
Never send login or password information using unencrypted text (plaintext).
Use a VPN connection when possible if you are sending sensitive data.
Enable security on home networks.
Use WPA2 or higher encryption for security.
Two of the most popular operating systems for mobile devices are Android and Apple iOS. Mobile devices are preprogrammed to use a Wi-Fi network for the internet if one is available, and the device can connect to the access point and receive an IP address. If no Wi-Fi network is available, the device uses the cellular data capability if it is configured.
Bluetooth technology provides a simple way for mobile devices to connect to each other and to wireless accessories. Bluetooth is wireless, automatic, and uses very little power, which helps conserve battery life. Some examples of devices that use Bluetooth include hands-free headsets, keyboards, a mouse, stereo controls, car speakerphones, and mobile speakers.
Bluetooth pairing occurs when two Bluetooth devices establish a connection to share resources. In order for the devices to pair, the Bluetooth radios are turned on, and one device begins searching for other devices. Other devices must be set to discoverable mode, also called visible, so that they can be detected.
When a Bluetooth device is in discoverable mode, it transmits the following information when another Bluetooth device requests it:
Name
Bluetooth class
Services that the device can use
Technical information, e.g. the features or the Bluetooth specification that it supports
During the pairing process, a PIN may be requested to authenticate the pairing process.

### Module 4: Build a Home Network

Module Objective: Configure integrated wireless router and wireless Client for home network connectivity

Wired Network Technology
Ethernet patch cable, usually unshielded twisted pair. These cables can be purchased with the RJ-45 connectors already installed
Category 5e is the most common wiring used in a LAN. The cable is made up of 4 pairs of wires that are twisted to reduce electrical interference
Coaxial cable has an inner wire surrounded by a tubular insulating layer, that is then surrounded by a tubular conducting shield. Most coax cables also have an external insulating sheath or jacket.
Fiber-optic cables can be either glass or plastic with a diameter about the same as a human hair and it can carry digital information at very high speeds over long distances. Fiber-optic cables have a very high bandwidth, which enables them to carry very large amounts of data.

4.3.1 Wi-Fi Networks
standards have been developed to allow wireless device communication. They specify (inc) the RF spectrum used, data rates, how the information is transmitted...
The main organization responsible for the creation of wireless technical standards is the Institute of Electrical and Electronics Engineers (IEEE).
IEEE 802.11 standard governs the WLAN environment. There are amendments to the IEEE 802.11 standard that describe characteristics for different standards of wireless communications. Wireless standards for LANs use the 2.4 GHz and 5 GHz frequency bands. Collectively these technologies are referred to as Wi-Fi.

Another organization, known as the Wi-Fi Alliance, is responsible for testing wireless LAN devices from different manufacturers. The Wi-Fi logo on a device means that this equipment meets standards and should operate with other devices that use the same standard.

Wireless routers using the 802.11 standards have multiple settings that have to be configured. These settings include the following:

N.B. SSID stands for Service Set Identifier.

Network mode
Determines the type of technology that must be supported. For example,802.11b,802.11g,802.11n or Mixed Mode.

Network Name (SSID)
Used to identify the WLAN. All devices that wish to participate in the WLAN must have the same SSID.

Standard Channel
Specifies the channel over which communication will occur. By default, this is set to Auto to allow the access point (AP) to determine the optimum channel to use.

SSID Broadcast
Determines if the SSID will be broadcast to all devices within range. By default, set to Enabled.

Network Mode

The 802.11 protocol can provide increased throughput based on the wireless network environment. If all wireless devices connect with the same 802.11 standard, maximum speeds can be obtained for that standard. If the access point is configured to accept only one 802.11 standard, devices that do not use that standard cannot connect to the access point.

A mixed mode wireless network environment can include devices that use any of the existing Wi-Fi standards. This environment provides easy access for older devices that need a wireless connection but do not support the latest standards.

When building a wireless network, it is important that the wireless components connect to the appropriate WLAN. This is done using the SSID.

The SSID is a case-sensitive, alphanumeric string that contains up to 32 characters. It is sent in the header of all frames transmitted over the WLAN. The SSID is used to tell wireless devices, called wireless stations (STAs), which WLAN they belong to and with which other devices they can communicate.

We use the SSID to identify a specific wireless network. It is essentially the name of the network. Wireless routers usually broadcast their configured SSIDs by default. The SSID broadcast allows other devices and wireless clients to automatically discover the name of the wireless network. When the SSID broadcast is disabled, you must manually enter the SSID on wireless devices.

Disabling SSID broadcasting can make it more difficult for legitimate clients to find the wireless network. However, simply turning off the SSID broadcast is not sufficient to prevent unauthorized clients from connecting to the wireless network. All wireless networks should use the strongest available encryption to restrict unauthorized access.

Router setup
A cable modem connection will have a coaxial terminal to accept a BNC-type connector. A DSL connection will have a port for a telephone-type cable, usually an RJ-11 connector.
After confirming that the computer is connected to the network router and the link lights on the NIC indicate a working connection, the computer needs an IP address. Most network routers are set up so that the computer receives an IP address automatically from a local DHCP server automatically configured on the wireless router. If the computer does not have an IP address, check the router documentation and configure the PC or tablet with a unique IP address, subnet mask, default gateway, and DNS information.

Design Considerations
What should my network be called?
If SSID broadcasting is on, the SSID name will be seen by all wireless clients within your signal range. Many times the SSID gives away too much information about the network to unknown client devices. It is not a good practice to include the device model or brand name as part of the SSID. Wireless devices have default settings that are easy to find on the internet, as well as known security weaknesses.

What types of devices will attach to my network?
Wireless devices contain radio transmitter/receivers that function within a specific frequency range. If a device only has the necessary radio for 802.11 b/g, it will not connect if the wireless router or access point is configured to only accept 802.11n or 802.11ac standards. If all devices support the same standard, the network will work at its optimum speed. If you have devices that do not support the n or ac standards, then you will have to enable legacy mode. A legacy mode wireless network environment varies between router models but can include a combination of 802.11a, 802.11b, 802.11g, 802.11n, and 802.11ac. This environment provides easy access for legacy devices that need a wireless connection.

#### Learning Outcomes

<img src="networkingBasics/images/checkpointPass1.png" alt="checkpointPass1" height="240px">

### Module 5: Communication Principles

Communication Protocols - Method, Language, Confirmation
Communication Standards -
Network Communication Models - compare OSI and TCP/IP models

TEST questions
TODO: learn protocolsbetter
Question 2
Rory is studying the fields inside an Ethernet frame for an upcoming test and notices that the destination Media Access Control (MAC) address is listed first before the source MAC address. Which of the following protocol characteristics is Rory investigating?

message timing
message pattern
encapsulation - SELECTED
encoding
timing

Question 3
As Rory continues to study Ethernet, he discovers that a frame can typically be 64 to 1518 bytes of information that is converted into a series of bits before being sent out on the network. Which two protocol characteristics did Rory learn about for Ethernet?

message pattern
message size - SELECTED
encapsulation
encoding - SELECTED
timing

5.2 Network Standards Organizations
when a new standard is proposed, each stage of the development and approval process is recorded in a numbered Request for Comments (RFC) document so that the evolution of the standard is tracked. RFCs for internet standards are published and managed by the Internet Engineering Task Force (IETF). orgs: IEEE, IANA, ICAAN, IETF, ITU, TIA.

network protocols
ETHERNET | IP | TCP | HTTP
ETHERNET - The Ethernet protocol is used for NIC card, network interface card to network interface card communications in the same network.
IP - can be IP version 4 or IP version 6. This makes sure that the message gets from the original source to the final destination. Whether or not that message is within the same network or has to go across multiple networks.addressing, routing, fragmentation, reassembly, best effort delivery
TCP - reordering, reliability, flow control, congestion control
HTTP - exchange/transfer of HTML. web page requests and responses

TCP/IP model Layers
Application - HTTP, FTP, SMTP, DNS
Transport - TCP, UDP
Internet - IP
Network Access - Ethernet, Wi-Fi, DSL, Cable

5.3.4 The OSI Reference Model
Protocol Model - a set of rules that govern how data is transmitted between two points in a network. A protocol model is a framework for understanding how protocols work together to enable communication between devices on a network.

Reference Model - a conceptual model that defines the functions of a communication system in terms of layers. A reference model is a theoretical framework that provides a common language and structure for understanding how different protocols and technologies work together to enable communication between devices on a network.

The OSI model is a theoretical model that characterizes and standardizes the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. The OSI model partitions a communication system into seven abstraction layers. The layers are (from top 7 to bottom 1):
Application - process-to-process communication, e.g. HTTP, FTP, SMTP, DNS
Presentation - common representation of data transfrered between layer services. e.g. encryption, compression, translation
Session - provides services to Presentation Layer to organize and synchronize communication between applications. e.g. session establishment, maintenance, and termination
Transport - defines Services to segement, transfer, and reassemble the data for individual communications between end devices. e.g. TCP, UDP
Network - services to exchange individual pieces of data over the network between identified end devices. e.g. IP, routing, fragmentation, reassembly, best effort delivery
Data Link - methods for exchanging data frames between devices over a common media. e.g. Ethernet, Wi-Fi, DSL, Cable
Physical - mechanical, electical, functional, and procedural means to activate, maintain, and deactivate physical connections for bit transmission to/from end devices. e.g. Ethernet, Wi-Fi, DSL, Cable

TCP/IP vs OSI

```mermaid
flowchart LR
    subgraph OSI Model
        direction TB
        OSI7["7<br>Application"]
        OSI6["6<br>Presentation"]
        OSI5["5<br>Session"]
        OSI4["4<br>Transport"]
        OSI3["3<br>Network"]
        OSI2["2<br>Data Link"]
        OSI1["1<br>Physical"]
    end
    subgraph TCP/IP Model
        direction TB
        TCP4["Application"]
        TCP3["Transport"]
        TCP2["Internet"]
        TCP1["Network Access"]
    end
    OSI7 --- TCP4
    OSI6 --- TCP4
    OSI5 --- TCP4
    OSI4 --- TCP3
    OSI3 --- TCP2
    OSI2 --- TCP1
    OSI1 --- TCP1
    style OSI7 fill:#e3e3ff
    style OSI6 fill:#e3e3ff
    style OSI5 fill:#e3e3ff
    style OSI4 fill:#cce5ff
    style OSI3 fill:#d4edda
    style OSI2 fill:#fff3cd
    style OSI1 fill:#fff3cd
    style TCP4 fill:#e3e3ff
    style TCP3 fill:#cce5ff
    style TCP2 fill:#d4edda
    style TCP1 fill:#fff3cd
```

The key similarities are in the transport and network layers; however, the two models differ in how they relate to the layers above and below each layer:

OSI Layer 3, the network layer, maps directly to the TCP/IP internet layer. This layer is used to describe protocols that address and route messages through an internetwork.
OSI Layer 4, the transport layer, maps directly to the TCP/IP transport layer. This layer describes general services and functions that provide ordered and reliable delivery of data between source and destination hosts.
The TCP/IP application layer includes several protocols that provide specific functionality to a variety of end user applications. The OSI model Layers 5, 6, and 7 are used as references for application software developers and vendors to produce applications that operate on networks.
Both the TCP/IP and OSI models are commonly used when referring to protocols at various layers. Because the OSI model separates the data link layer from the physical layer, it is commonly used when referring to these lower layers.

learning outcomes:
Communication Protocols: A protocol is a set of rules that govern how data is transmitted between two points in a network. Protocols are necessary to ensure that devices on a network can communicate with each other effectively. these include:
message format - the structure of the data being transmitted, including the headers and payload.
message timing - the timing of when messages are sent and received, including any delays or timeouts that may occur.
message pattern - the sequence of messages that are exchanged between devices, including any acknowledgments or responses that may be required.
encapsulation - the process of adding headers and trailers to data as it moves through the layers of a network protocol stack. This allows data to be transmitted across different types of networks and ensures that it is properly formatted for the receiving device.
encoding - the process of converting data into a specific format for transmission, e.g. converting text into binary code or compressing data to reduce its size for faster transmission.
Confirmation - the process of acknowledging the receipt of a message or data, which can help ensure that messages are delivered successfully and that any errors or issues can be identified and resolved.
message pattern - the sequence of messages that are exchanged between devices, including any acknowledgments or responses that may be required. This can include the order in which messages are sent and received, as well as any specific patterns or protocols that must be followed for successful communication.
message size - the amount of data that is being transmitted in a message, which can affect the speed and efficiency of communication. Protocols may have specific limits on message size, and larger messages may require additional processing or fragmentation to be transmitted successfully.
encapsulation - the process of adding headers and trailers to data as it moves through the layers of a network protocol stack. This allows data to be transmitted across different types of networks and ensures that it is properly formatted for the receiving device. Encapsulation can also provide additional functionality, e.g. error checking or encryption, to help ensure the integrity and security of the data being transmitted.
encoding - the process of converting data into a specific format for transmission, e.g. converting text into binary code or compressing data to reduce its size for faster transmission. Encoding can also involve adding error correction codes or other information to help ensure that the data is transmitted accurately and can be properly decoded by the receiving device.
timing - the timing of when messages are sent and received, including any delays or timeouts that may occur.

Communication Standards

Network communication standards are developed by various organizations to ensure that devices from different manufacturers can communicate with each other effectively. These standards define the protocols, formats, and procedures for communication between devices on a network. Some of the key organizations responsible for developing network communication standards include:
IEEE (Institute of Electrical and Electronics Engineers) - develops standards for wired and wireless networking technologies, including Ethernet and Wi-Fi.
IANA (Internet Assigned Numbers Authority) - manages the allocation of IP addresses and other internet protocol resources.
ICANN (Internet Corporation for Assigned Names and Numbers) - manages the domain name system (DNS) and other internet-related resources.
IETF (Internet Engineering Task Force) - develops and promotes internet standards, including protocols for communication between devices on a network.
ITU (International Telecommunication Union) - develops standards for telecommunications and information communication technologies.
TIA (Telecommunications Industry Association) - develops standards for telecommunications and information communication technologies, including standards for cabling and network infrastructure.

OSI Model Layer Descriptions

<img src="networkingBasics/images/module5Pass.png" alt="module5Pass" height="240px">

### Module 6: Network Media

objective: Network Media types

UTP - unshielded twisted pair
Coaxial cable - an inner wire surrounded by a tubular insulating layer, that is then surrounded by a tubular conducting shield. Most coax cables also have an external insulating sheath or jacket.
fiber-optic cables - can be either glass or plastic with a diameter about the same as a human hair and it can carry digital information at very high speeds over long distances. Fiber-optic cables have a very high bandwidth, which enables them to carry very large amounts of data.

3 media cables:
Modern networks primarily use three types of media to interconnect devices, as shown in the figure:

Metal wires within cables - Data is encoded into electrical impulses.
Glass or plastic fibers within cables (fiber-optic cable) - Data is encoded into pulses of light.
Wireless transmission - Data is encoded via modulation of specific frequencies of electromagnetic waves.

The four main criteria for choosing network media are DEASC:

D, Distance: What is the maximum distance that the media can successfully carry a signal?
E, Environment: What is the environment in which the media will be installed?
AS, Amount of Data: What is the amount of data and at what speed must it be transmitted?
C, Cost: What is the cost of the media and installation?

<img src="networkingBasics/images/module6Pass.png" alt="module6Pass" height="240px">

### Module 7: Access layer

Learning objectives:
Encapsualtion and the Ethernet frame
Access Layer

Ethernet Frame:
Preamble - 7 bytes used for synchronization
Start Frame Delimiter (SFD) - 1 byte used to indicate the start of the frame
Destination MAC Address - 6 bytes used to identify the destination host
Source MAC Address - 6 bytes used to identify the source host
Length Type - 2 bytes used to indicate the protocol being encapsulated in the payload OR type of data IPv4, IPv6...
Data Payload - 46 to 1500 bytes of data being transmitted
Frame Check Sequence (FCS) - 4 bytes used for error checking

Switches:
like to learn. but only for about 5 mins.
Ethernet Switches:
802.3 Ethernet frame is used for communication between devices on the same network. The Ethernet frame contains a destination MAC address and a source MAC address, which are used to identify the devices that are communicating. When a switch receives an Ethernet frame, it reads the destination MAC address and forwards the frame only to the port that is connected to the device with that MAC address. This process is called switching, and it helps to reduce network congestion and improve performance by ensuring that frames are only sent to the devices that need them.
MAC address tables:

learning outcomes:
Encapsulation and the Ethernet Frame: Encapsulation is the process of adding headers and trailers to data as it moves through the layers of a network protocol stack. This allows data to be transmitted across different types of networks and ensures that it is properly formatted for the receiving device. The Ethernet frame is a specific type of data packet used in Ethernet networks. It consists of several fields, including a preamble, start frame delimiter, destination MAC address, source MAC address, length/type field, data payload, and frame check sequence. Each of these fields serves a specific purpose in the encapsulation process, allowing data to be transmitted effectively and efficiently across an Ethernet network.

Access layer: The access layer is the layer of a network that provides connectivity to end devices, e.g. computers, printers, and mobile devices. It is responsible for providing access to the network and ensuring that data is transmitted securely and efficiently between end devices and the rest of the network. The access layer typically includes switches, wireless access points, and other networking devices that connect end devices to the network infrastructure. The access layer also provides features e.g. authentication, authorization, and accounting (AAA) to ensure that only authorized users can access the network and that their activities are monitored and logged for security purposes.

MAC Filtering:
MAC filtering in wireless networks acts as a security access control mechanism that permits or denies access to a network based on a device's unique 48-bit hardware address (MAC address). It functions as a gatekeeper, creating white or blacklists to allow or block specific devices, but it does not provide traffic encryption.
Key Characteristics of MAC Filtering:
Access Control Method: It is a security feature, often found on routers and access points, to allow only authorized devices to connect to a Wi-Fi network.Whitelist/Blacklist Functionality: Administrators can create a list of authorized devices (whitelist) to permit access or a list of disallowed devices (blacklist) to block access.
Hardware Identifier Based: It uses the unique MAC address of a device’s network interface card (NIC) to identify it, regardless of its IP address.
Limited Security (Weakness): It is considered a weak security measure because MAC addresses can be easily spoofed or cloned by attackers.Maintenance Intensive: Managing MAC address lists is cumbersome in larger networks, requiring constant manual updates.No Encryption: MAC filtering does not encrypt traffic or protect against eavesdropping; it only controls access.
Limitations:
Spoofing: Attackers can bypass MAC filters by "spoofing" (impersonating) the MAC address of an authorized device.Complexity: It does not scale well to large environments with many devices, leading to increased management overhead.Randomization Conflict: Modern devices often use randomized MAC addresses for privacy, which can cause connectivity issues when MAC filtering is enabled.It is generally recommended to use MAC filtering as an extra layer in combination with strong encryption protocols like WPA2 or WPA3, rather than as a standalone security measure.

switches:
A switch keeps its MAC address table current by using the source MAC address and the incoming port of incoming data frames. By examining these two pieces of information, the switch learns which device is connected to which port and updates the table's timestamp to keep entries active.

Key details on how switches maintain this information:
Source MAC Address: When a frame arrives, the switch examines the source MAC address to identify which device sent the data.
Incoming Port: The switch records the specific interface (port) on which the frame arrived.
Association/Learning: The switch pairs the source MAC address with the incoming port in its table, allowing it to know where to send future traffic.
Aging Mechanism: If a device stops sending frames, the switch will remove that device's MAC address from the table after a certain period (aging time) to keep the table accurate.

While the switch uses the destination MAC address to decide where to send a frame, it specifically uses the source MAC address and incoming port to update and maintain the table.

<img src="networkingBasics/images/module7Pass.png" alt="module7Pass" height="240px">

### Checkpoint 2

<img src="networkingBasics/images/checkpointPass2.png" alt="checkpointPass2" height="240px">

### Module 8: Internet Protocol

learning objective: IP address features

IPv4 address purpose - logical network address used for routing and addressing,

IPv4 address structure - addresses and subnets used together

learning outcomes:
IPv4 Address Purpose: An IPv4 address is a logical network address used for routing and addressing in an IP network. It serves as a unique identifier for devices on a network, allowing them to communicate with each other and with devices on other networks. IPv4 addresses are used to identify both the source and destination of data packets as they traverse the internet or other IP-based networks. They are essential for the proper functioning of the internet and enable devices to send and receive data across networks.

IPv4 Address Structure: An IPv4 address is a 32-bit binary number that is typically represented in dotted decimal notation, consisting of four octets separated by periods (e.g., 192.168.1.1). Each octet can range from 0 to 255, allowing for a total of approximately 4.3 billion unique addresses. IPv4 addresses are structured into two main parts: the network portion and the host portion. The network portion identifies the specific network to which the device belongs, while the host portion identifies the individual device within that network. Subnetting is often used to divide larger networks into smaller, more manageable subnets, allowing for more efficient use of IP addresses and improved network performance.

<img src="networkingBasics/images/module8Pass.png" alt="module8Pass" height="240px">

### Module 9: IPv4 and Network Segmentation
