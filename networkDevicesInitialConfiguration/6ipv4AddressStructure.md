# IPv4 Address Structure

## Network and Host Portions

### IPv4 Address

An IPv4 address is a 32-bit hierarchical address that is made up of a network portion and a host portion. When determining the network portion versus the host portion, you must look at the 32-bit stream, as shown in the figure.

IPv4 Address
The diagram shows the breakdown of an IPv4 address into the network and host portions. The IPv4 address is 192.168.10.10. Underneath, the address is converted into 11000000 10101000 00001010 00001010. A dashed line shows the separation between the network and host portions. This occurs after the third octet and the 24th bit.
11000000 10101000 00001010 00001010
192 .168 .10 .10  
| Network Portion | Host Portion |

The bits within the network portion of the address must be identical for all devices that reside in the same network. The bits within the host portion of the address must be unique to identify a specific host within a network. If two hosts have the same bit-pattern in the specified network portion of the 32-bit stream, those two hosts will reside in the same network.

the role of the subnet mask is to know which portion of the 32-bits identifies the network and which identifies the host.

The Subnet Mask
Assigning an IPv4 address to a host requires:

1. IPv4 address - This is the unique IPv4 address of the host.
2. Subnet mask- This is used to identify the network/host portion of the IPv4 address.

Subnet Mask
Note: A default gateway IPv4 address is required to reach remote networks and DNS server IPv4 addresses are required to translate domain names to IPv4 addresses.

The IPv4 subnet mask is used to differentiate the network portion from the host portion of an IPv4 address. When an IPv4 address is assigned to a device, the subnet mask is used to determine the network address of the device. The network address represents all the devices on the same network.

Subnet Mask

```text

255      .255     .255     .0
11111111 11111111 11111111 00000000
```

Associating an IPv4 Address with its Subnet Mask
Notice how the subnet mask is a consecutive sequence of 1 bits followed by a consecutive sequence of 0 bits.

To identify the network and host portions of an IPv4 address, the subnet mask is compared to the IPv4 address bit for bit, from left to right.

![alt text](ipv4SubNet.png)

the subnet mask does not contain the network or host portion of an IPv4 address, it just tells the computer where to look for the part of the IPv4 address that is the network portion and which part is the host portion.

N.B. ANDing - The process used to identify the network portion and host portion is called ANDing.

## The Prefix Length

Expressing network addresses and host addresses with the dotted decimal subnet mask address can become cumbersome. Fortunately, there is an alternative method of identifying a subnet mask, a method called the prefix length.

The prefix length is the number of bits set to 1 in the subnet mask. It is written in “slash notation”, which is noted by a forward slash (/) followed by the number of bits set to 1. Therefore, count the number of bits in the subnet mask and prepend it with a slash.

Refer to the table for examples. The first column lists various subnet masks that can be used with a host address. The second column displays the converted 32-bit binary address. The last column displays the resulting prefix length.

```table
subnet mask     | 32-bit binary                 | Prefix length
255.0.0.0       | 11111111.00000000.00000000.00000000   | /8
255.255.0.0     | 11111111.11111111.00000000.00000000   | /16
255.255.255.0   | 11111111.11111111.11111111.00000000   | /24
255.255.255.0   | 11111111.11111111.11111111.10000000   | /25
255.255.255.0   | 11111111.11111111.11111111.11000000   | /26
255.255.255.0   | 11111111.11111111.11111111.11100000   | /27
255.255.255.0   | 11111111.11111111.11111111.11110000   | /28
255.255.255.0   | 11111111.11111111.11111111.11111000   | /29
255.255.255.0   | 11111111.11111111.11111111.11111100   | /30
255.255.255.255 | 11111111.11111111.11111111.11111111   | /32
```

Note: A network address is also referred to as a prefix or network prefix. Therefore, the prefix length is the number of 1 bits in the subnet mask.

When representing an IPv4 address using a prefix length, the IPv4 address is written followed by the prefix length with no spaces. For example, 192.168.10.10 255.255.255.0 would be written as 192.168.10.10/24.

## Determining the Network: Logical AND

A logical AND is one of three Boolean operations used in Boolean or digital logic. The other two are OR and NOT. The AND operation is used in determining the network address.

Logical AND is the comparison of two bits that produce the results shown below. Note how only a 1 AND 1 produces a 1. Any other combination results in a 0.

1 AND 1 = 1
0 AND 1 = 0
1 AND 0 = 0
0 AND 0 = 0

1 represents True and 0 represents False. When using an AND operation, both input values must be True (1) for the result to be True (1).

To identify the network address of an IPv4 host, the IPv4 address is logically ANDed, bit by bit, with the subnet mask. ANDing between the address and the subnet mask yields the network address.

To illustrate how AND is used to discover a network address, consider a host with IPv4 address 192.168.10.10 and subnet mask of 255.255.255.0, as shown in the figure:

IPv4 host address (192.168.10.10) - The IPv4 address of the host in dotted decimal and binary formats.
Subnet mask (255.255.255.0) - The subnet mask of the host in dotted decimal and binary formats.
Network address (192.168.10.0) - The logical AND operation between the IPv4 address and subnet mask results in an IPv4 network address shown in dotted decimal and binary formats.

Using the first sequence of bits as an example, notice the AND operation is performed on the 1-bit of the host address with the 1-bit of the subnet mask. This results in a 1 bit for the network address. 1 AND 1 = 1.

The AND operation between an IPv4 host address and subnet mask results in the IPv4 network address for this host. In this example, the AND operation between the host address of 192.168.10.10 and the subnet mask 255.255.255.0 (/24), results in the IPv4 network address of 192.168.10.0/24. This is an important IPv4 operation, as it tells the host what network it belongs to.

![alt text](ANDing.png)

## Learning Outcome

### IPv4 Address Structure

An IPv4 address is a 32-bit hierarchical address that is made up of a network portion and a host portion. When determining the network portion versus the host portion, you must look at the 32-bit stream. The bits within the network portion of the address must be identical for all devices that reside in the same network. The bits within the host portion of the address must be unique to identify a specific host within a network. If two hosts have the same bit-pattern in the specified network portion of the 32-bit stream, those two hosts will reside in the same network.

The IPv4 subnet mask is used to differentiate the network portion from the host portion of an IPv4 address. When an IPv4 address is assigned to a device, the subnet mask is used to determine the network address of the device. The network address represents all the devices on the same network.

An alternative method of identifying a subnet mask, a method called the prefix length. The prefix length is the number of bits set to 1 in the subnet mask. It is written in “slash notation”, which is noted by a forward slash (/) followed by the number of bits set to 1. For example, 192.168.10.10 255.255.255.0 would be written as 192.168.10.10/24.

The AND operation is used in determining the network address. Logical AND is the comparison of two bits. Note how only a 1 AND 1 produces a 1. Any other combination results in a 0.

```list
1 AND 1 = 1
0 AND 1 = 0
1 AND 0 = 0
0 AND 0 = 0
```

To identify the network address of an IPv4 host, the IPv4 address is logically ANDed, bit by bit, with the subnet mask. ANDing between the address and the subnet mask yields the network address.

## Module 6 Pass

![alt text](module6Pass.png)
