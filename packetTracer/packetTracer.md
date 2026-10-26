## Packet Tracer

### 1. Intro To

**Skills Learned** - Cisco Packet Tracer to visualize and simulate a network using everyday examples.

### 2. Exploring Networking

**Skills Learned** - connect, configure network devices, wireless devices, verify connectivity.

### 3. IoT

**Skills Learned** - IoT, Network Simulation, Environmental Controls, Programming, JavaScript, Python, Visual Blocky.

#### Module 1: Create Your Own Smart Home Network

In simple terms, the IoT is a collection of networked sensors, actuators, and smart devices that gather and share data. To connect the devices to your network, you need a home gateway or registration server. To control the devices, you have two options: you can interact directly with a device, or you can connect remotely over the network using a remote PC, tablet, or smartphone. You can connect and control smart devices using either a Home Gateway device or a remote registration server. The Home Gateway device acts as a local connection to your IoT smart devices. The Home Gateway device provides an IoT registration service that is always turned on, and an auto discovery service for Things in the local Ethernet and wireless network.

**Home Gateway tabs**

- **Physical tab** - The device has an internet port, four LAN ports, and multiple antennae.
- **Config tab** - Shows the interfaces and network settings that are configurable.
- **GUI tab** - Shows the registration server inside the device that allows for interaction with IoT devices. It is on by default but can be turned off.
- **Attributes tab** - Blank by default but can show features and values (for example, MTBF, cost, power source, and wattage). IoT devices can also be registered to a dedicated Registration Server for remote monitoring, control, or programming. The dedicated registration server has the additional benefit of providing many other services to your network (for example, web, DHCP, DNS, email, and FTP).

#### Module 2: Environmental Controls and IoT Things in Packet Tracer

In the Physical Workspace there are containers. Containers include the intercity, city, buildings, and wiring closets. They all have their own set of environmental values. If there are no devices configured to affect the environment, their values are looped on a 24-hour cycle. Different containers may have different levels of insulation and thus different transference values. The transference values determine the rate that the child container converges with the parent container, and it works the same way for all environment types. To provide true IoT solutions, it is critical to have programming knowledge. Packet Tracer provides support for JavaScript, Python, and Visual Blocky.

**Important terms and concepts**

- **Current time** - Time inside a container that increments by 30-minute steps. Every 1 second in real time equals 30 minutes in "Container" time. The timer goes from 0 (midnight) to 11:59.
- **KeyFrame** - Represents a single moment in time.
- **KeyFrame graph** - A graph that shows the value of environmental elements at any given point in time throughout the day.
- **Transference** - Values that determine the rate that the child container converges with the parent container and works the same way for all environment types.
- **Programming** - You can use programming language to modify environmental elements within a container. You can even create a new IoT Thing in Packet Tracer. First, decide what the Thing will do, how it will connect to the network, and how it will work. Identify an existing Thing that functions in a similar manner. The existing script can then be modified to create the new script. Clicking any IoT device in the workspace reveals its specifications.

**IoT device specifications**

- **Features** - How the device works or what it does. Devices can generate high and low values based on a button being pushed or toggled on and off, or they can detect certain environmental values (for example, smoke or sunlight).
- **Usage** - Things may connect to other IoT devices to receive LOW or HIGH inputs, or it may read the variable set in the Environment object.
- **Direct Control** - Shows keystrokes that allow you to physically interact with the Thing.
- **Local and Remote Control** - Shows how to control the Thing locally or remotely (if applicable).
- **Data Specifications** - How the values are produced or the port or slot used to connect to the sensor.
- **Example** - Describes an example of how it works.
