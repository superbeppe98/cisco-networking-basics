[Back to Syllabus](./README.md#course-syllabus)

## 9.0.1 Webster - Why Should I Take this Module?

- Kishori has a new patient, Divya, who was admitted today. Like Srinivas, Divya does not speak the same language that Kishori speaks. Divya only speaks Telugu and has limited English. Kishori wants to send an email to the nurses on the next shift to determine whether any of them speak Telugu. Kishori can send a multicast email message, which is a single email message sent to specific multiple recipients. You know about the structure of IPv4 addresses. Now it is time to learn more about them. Have you heard of unicast, broadcast, and multicast IPv4 addresses? What are public, private, and reserved IPv4 addresses? Dive into this module to get a deeper understanding of IPv4 addresses

## 9.0.2 What Will I Learn in this Module?

- Module Title: IPv4 and Network Segmentation
- Module Objective: Explain how IPv4 addresses are used in network communication and segmentation

## 9.1.1 Video - IPv4 Unicast

## 9.1.2 Unicast

- In the previous topic you learned about the structure of an IPv4 address; each has a network portion and a host portion. There are different ways to send a packet from a source device, and these different transmissions affect the destination IPv4 addresses
- Unicast transmission refers to one device sending a message to one other device in one-to-one communications
- A unicast packet has a destination IP address that is a unicast address which goes to a single recipient. A source IP address can only be a unicast address, because the packet can only originate from a single source. This is regardless of whether the destination IP address is a unicast, broadcast, or multicast
- Play the animation to see an example of unicast transmission.
- Note: In this course, all communication between devices is unicast unless otherwise noted
- IPv4 unicast host addresses are in the address range of 1.1.1.1 to 223.255.255.255. However, within this range are many addresses that are reserved for special purposes. These special purpose addresses will be discussed later in this module
- Note: In the animation, notice that the subnet mask for 255.255.255.0 is represented using slash notion or /24. This indicates that the subnet mask is 24 bits long. The subnet mask 255.255.255.0 in binary is 11111111.11111111.11111111.00000000

## 9.1.3 Video - IPv4 Broadcast

## 9.1.4 Broadcast

- Broadcast transmission refers to a device sending a message to all the devices on a network in one-to-all communications
- A broadcast packet has a destination IP address with all ones (1s) in the host portion, or 32 one (1) bits
- Note: IPv4 uses broadcast packets. However, there are no broadcast packets with IPv6
- A broadcast packet must be processed by all devices in the same broadcast domain. A broadcast domain identifies all hosts on the same network segment. A broadcast may be directed or limited. A directed broadcast is sent to all hosts on a specific network. For example, a host on the 172.16.4.0/24 network sends a packet to 172.16.4.255. A limited broadcast is sent to 255.255.255.255. By default, routers do not forward broadcasts

## 9.1.5 Video - IPv4 Multicast

## 9.1.6 Multicast

- Multicast transmission reduces traffic by allowing a host to send a single packet to a selected set of hosts that subscribe to a multicast group
- A multicast packet is a packet with a destination IP address that is a multicast address. IPv4 has reserved the 224.0.0.0 to 239.255.255.255 addresses as a multicast range
- Hosts that receive particular multicast packets are called multicast clients. The multicast clients use services requested by a client program to subscribe to the multicast group
- Each multicast group is represented by a single IPv4 multicast destination address. When an IPv4 host subscribes to a multicast group, the host processes packets addressed to this multicast address, and packets addressed to its uniquely allocated unicast address
- Routing protocols such as OSPF use multicast transmissions. For example, routers enabled with OSPF communicate with each other using the reserved OSPF multicast address 224.0.0.5. Only devices enabled with OSPF will process these packets with 224.0.0.5 as the destination IPv4 address. All other devices will ignore these packets
- The animation demonstrates clients accepting multicast packets

## 9.1.7 Activity - Unicast, Broadcast, or Multicast

- Instructions:
    - Click Start to see a destination IP address. Next, click the host or hosts which will receive a packet based on the address type (unicast, broadcast, or multicast). Click Check to verify your answer. Click New Problem again to get a new problem

## 9.2.1 Public and Private IPv4 Addresses

- Just as there are different ways to transmit an IPv4 packet, there are also different types of IPv4 addresses. Some IPv4 addresses cannot be used to go out to the internet, and others are specifically allocated for routing to the internet. Some are used to verify a connection and others are self-assigned. As a network administrator, you will eventually become very familiar with the types of IPv4 addresses, but for now, you should at least know what they are and when to use them
- Public IPv4 addresses are addresses which are globally routed between internet service provider (ISP) routers. However, not all available IPv4 addresses can be used on the internet. There are blocks of addresses called private addresses that are used by most organizations to assign IPv4 addresses to internal hosts
- In the mid-1990s, with the introduction of the World Wide Web (WWW), private IPv4 addresses were introduced because of the depletion of IPv4 address space. Private IPv4 addresses are not unique and can be used internally within any network.
- Note: The long-term solution to IPv4 address depletion was IPv6

## 9.2.2 Routing to the Internet

- Most internal networks, from large enterprises to home networks, use private IPv4 addresses for addressing all internal devices (intranet) including hosts and routers. However, private addresses are not globally routable
- In the figure, customer networks 1, 2, and 3 are sending packets outside their internal networks. These packets have a source IPv4 address that is a private address and a destination IPv4 address that is public (globally routable). Packets with a private address must be filtered (discarded) or translated to a public address before forwarding the packet to an ISP
- Private IPv4 Addresses and Network Address Translation (NAT)

## 9.2.3 Activity - Pass or Block IPv4 Addresses

- Instructions:
    - Decide to Pass or Block each IP address depending on whether it is Public (the internet) or Private (small local network). Click Start to begin and click on either Pass or Block

## 9.2.4 Special Use IPv4 Addresses

- There are certain addresses, such as the network address and broadcast address, that cannot be assigned to hosts. There are also special addresses that can be assigned to hosts, but with restrictions on how those hosts can interact within the network

- Loopback addresses
    - Loopback addresses (127.0.0.0 /8 or 127.0.0.1 to 127.255.255.254) are more commonly identified as only 127.0.0.1. These are special addresses used by a host to direct traffic to itself. For example, the ping command is commonly used to test connections to other hosts. But you can also use the ping command to test if the IP configuration on your own device, as shown in the figure
    - Note: You will learn more about the ping command later in this course

- Link-Local addresses
    - Link-local addresses (169.254.0.0 /16 or 169.254.0.1 to 169.254.255.254) are more commonly known as the Automatic Private IP Addressing (APIPA) addresses or self-assigned addresses. They are used by a Windows client to self-configure in the event that the client cannot obtain an IP addressing through other methods. Link-local addresses can be used in a peer-to-peer connection but are not commonly used for this purpose

## 9.2.5 Legacy Classful Addressing

- In 1981, IPv4 addresses were assigned using classful addressing as defined in RFC 790 (https://tools.ietf.org/html/rfc790), Assigned Numbers. Customers were allocated a network address based on one of three classes, A, B, or C. The RFC divided the unicast ranges into specific classes as follows:
    - Class A (0.0.0.0/8 to 127.0.0.0/8) - Designed to support extremely large networks with more than 16 million host addresses. Class A used a fixed /8 prefix with the first octet to indicate the network address and the remaining three octets for host addresses (more than 16 million host addresses per network)
    - Class B (128.0.0.0 /16 - 191.255.0.0 /16) - Designed to support the needs of moderate to large size networks with up to approximately 65,000 host addresses. Class B used a fixed /16 prefix with the two high-order octets to indicate the network address and the remaining two octets for host addresses (more than 65,000 host addresses per network)
    - Class C (192.0.0.0 /24 - 223.255.255.0 /24) - Designed to support small networks with a maximum of 254 hosts. Class C used a fixed /24 prefix with the first three octets to indicate the network and the remaining octet for the host addresses (only 254 host addresses per network)
    - Note: There is also a Class D multicast block consisting of 224.0.0.0 to 239.0.0.0 and a Class E experimental address block consisting of 240.0.0.0 - 255.0.0.0.
- At the time, with a limited number of computers using the internet, classful addressing was an effective means to allocate addresses. As shown in the figure, Class A and B networks have a very large number of host addresses and Class C has very few. Class A networks accounted for 50% of the IPv4 networks. This caused most of the available IPv4 addresses to go unused

## 9.2.6 Assignment of IP Addresses

- Public IPv4 addresses are addresses which are globally routed over the internet. Public IPv4 addresses must be unique
- Both IPv4 and IPv6 addresses are managed by the Internet Assigned Numbers Authority (IANA). The IANA manages and allocates blocks of IP addresses to the Regional Internet Registries (RIRs). The five RIRs are shown in the figure
- RIRs are responsible for allocating IP addresses to ISPs who provide IPv4 address blocks to organizations and smaller ISPs. Organizations can also get their addresses directly from an RIR (subject to the policies of that RIR)
- The five RIRs are:
    - AfriNIC (African Network Information Centre) - Africa Region
    - APNIC (Asia Pacific Network Information Centre) - Asia/Pacific Region
    - ARIN (American Registry for Internet Numbers) - North America Region
    - LACNIC (Regional Latin-American and Caribbean IP Address Registry) - Latin America and some Caribbean Islands
    - RIPE NCC (Réseaux IP Européens Network Coordination Centre) - Europe, the Middle East, and Central Asia

## 9.2.7 Activity - Public or Private IPv4 Address

## 9.2.8 Check Your Understanding - Types of IPv4 Addresses

## 9.3.1 Video - Network Segmentation

## 9.3.2 Broadcast Domains and Segmentation

- Have you ever received an email that was addressed to every person at your work or school? This was a broadcast email. Hopefully, it contained information that each of you needed to know. But often a broadcast is not really pertinent to everyone in the mailing list. Sometimes, only a segment of the population needs to read that information
- In an Ethernet LAN, devices use broadcasts and the Address Resolution Protocol (ARP) to locate other devices. ARP sends Layer 2 broadcasts to a known IPv4 address on the local network to discover the associated MAC address. Devices on Ethernet LANs also locate other devices using services. A host typically acquires its IPv4 address configuration using the Dynamic Host Configuration Protocol (DHCP) which sends broadcasts on the local network to locate a DHCP server
- Switches propagate broadcasts out all interfaces except the interface on which it was received. For example, if a switch in the figure were to receive a broadcast, it would forward it to the other switches and other users connected in the network.

- Routers Segment Broadcast Domains
    - Routers do not propagate broadcasts. When a router receives a broadcast, it does not forward it out other interfaces. For instance, when R1 receives a broadcast on its Gigabit Ethernet 0/0 interface, it does not forward out another interface
    - Therefore, each router interface connects to a broadcast domain and broadcasts are only propagated within that specific broadcast domain

## 9.3.3 Problems with Large Broadcast Domains

- A large broadcast domain is a network that connects many hosts. A problem with a large broadcast domain is that these hosts can generate excessive broadcasts and negatively affect the network. In the figure, LAN 1 connects 400 users that could generate an excess amount of broadcast traffic. This results in slow network operations due to the significant amount of traffic it can cause, and slow device operations because a device must accept and process each broadcast packet

- A Large Broadcast Domain
- The solution is to reduce the size of the network to create smaller broadcast domains in a process called subnetting. These smaller network spaces are called subnets
- In the figure, the 400 users in LAN 1 with network address 172.16.0.0 /16 have been divided into two subnets of 200 users each: 172.16.0.0 /24 and 172.16.1.0 /24. Broadcasts are only propagated within the smaller broadcast domains. Therefore, a broadcast in LAN 1 would not propagate to LAN 2

- Communicating Between Networks
    - Notice how the prefix length has changed from a single /16 network to two /24 networks. This is the basis of subnetting: using host bits to create additional subnets
    - Note: The terms subnet and network are often used interchangeably. Most networks are a subnet of some larger address block

## 9.3.4 Reasons for Segmenting Networks

- List of expandable sections. Select each button to expand the content
- Subnetting reduces overall network traffic and improves network performance. It also enables an administrator to implement security policies such as which subnets are allowed or not allowed to communicate together. Another reason is that it reduces the number of devices affected by abnormal broadcast traffic due to misconfigurations, hardware/software problems, or malicious intent
- There are various ways of using subnets to help manage network devices
- Click each image for an illustration of how network administrators can group devices and services into subnets
- Network administrators can create subnets using any other division that makes sense for the network. Notice in each figure, the subnets use longer prefix lengths to identify networks
- Understanding how to subnet networks is a fundamental skill that all network administrators must develop. Various methods have been created to help understand this process. Although a little overwhelming at first, pay close attention to the detail and, with practice, subnetting will become easier

## 9.3.5 Check Your Understanding - Network Segmentation

## 9.4.1 What Did I Learn in this Module?

- IPv4 Unicast, Broadcast, and Multicast
- Unicast transmission refers to one device sending a message to one other device in one-to-one communications. A unicast packet has a destination IP address that is a unicast address which goes to a single recipient. A source IP address can only be a unicast address because the packet can only originate from a single source. This is regardless of whether the destination IP address is a unicast, broadcast or multicast. IPv4 unicast host addresses are in the address range of 1.1.1.1 to 223.255.255.255

- Broadcast transmission refers to a device sending a message to all the devices on a network in one-to-all communications. A broadcast packet has a destination IP address with all ones (1s) in the host portion, or 32 one (1) bits. A broadcast packet must be processed by all devices in the same broadcast domain. A broadcast may be directed or limited. A directed broadcast is sent to all hosts on a specific network. A limited broadcast is sent to 255.255.255.255. By default, routers do not forward broadcasts

- Multicast transmission reduces traffic by allowing a host to send a single packet to a selected set of hosts that subscribe to a multicast group. A multicast packet is a packet with a destination IP address that is a multicast address. IPv4 has reserved the 224.0.0.0 to 239.255.255.255 addresses as a multicast range. Each multicast group is represented by a single IPv4 multicast destination address. When an IPv4 host subscribes to a multicast group, the host processes packets addressed to this multicast address, and packets addressed to its uniquely allocated unicast address

- Type of IPv4 address
    - Public IPv4 addresses are addresses which are globally routed between ISP routers. However, not all available IPv4 addresses can be used on the internet. There are blocks of addresses called private addresses that are used by most organizations to assign IPv4 addresses to internal hosts. Most internal networks, from large enterprises to home networks, use private IPv4 addresses for addressing all internal devices (intranet) including hosts and routers. However, private addresses are not globally routable. Before the ISP can forward this packet, it must translate the source IPv4 address, which is a private address, to a public IPv4 address using NAT
    - Loopback addresses (127.0.0.0 /8 or 127.0.0.1 to 127.255.255.254) are more commonly identified as only 127.0.0.1, these are special addresses used by a host to direct traffic to itself. Link-local addresses (169.254.0.0 /16 or 169.254.0.1 to 169.254.255.254) are more commonly known as the Automatic Private IP Addressing (APIPA) addresses or self-assigned addresses. They are used by a Windows DHCP client to self-configure in the event that there are no DHCP servers available

- In 1981, IPv4 addresses were assigned using classful addressing as defined in RFC 790 (https://tools.ietf.org/html/rfc790), Assigned Numbers. Customers were allocated a network address based on one of three classes, A, B, or C. The RFC divided the unicast ranges into specific classes as follows:
    - Class A (0.0.0.0/8 to 127.0.0.0/8) - Designed to support extremely large networks with more than 16 million host addresses
    - Class B (128.0.0.0 /16 - 191.255.0.0 /16) - Designed to support the needs of moderate to large size networks with up to approximately 65,000 host addresses
    - Class C (192.0.0.0 /24 - 223.255.255.0 /24) - Designed to support small networks with a maximum of 254 hosts
    - There is also a Class D multicast block consisting of 224.0.0.0 to 239.0.0.0 and a Class E experimental address block consisting of 240.0.0.0 - 255.0.0.0

- Public IPv4 addresses are addresses which are globally routed over the internet. Public IPv4 addresses must be unique. Both IPv4 and IPv6 addresses are managed by the IANA. The IANA manages and allocates blocks of IP addresses to the RIRs. RIRs are responsible for allocating IP addresses to ISPs who provide IPv4 address blocks to organizations and smaller ISPs. Organizations can also get their addresses directly from an RIR

- Network segmentation
In an Ethernet LAN, devices use broadcasts and ARP to locate other devices. ARP sends Layer 2 broadcasts to a known IPv4 address on the local network to discover the associated MAC address. Devices on Ethernet LANs also locate other devices using services. A host typically acquires its IPv4 address configuration using DHCP which sends broadcasts on the local network to locate a DHCP server. Switches propagate broadcasts out all interfaces except the interface on which it was received

- A large broadcast domain is a network that connects many hosts. A problem with a large broadcast domain is that these hosts can generate excessive broadcasts and negatively affect the network. The solution is to reduce the size of the network to create smaller broadcast domains in a process called subnetting. These smaller network spaces are called subnets. The basis of subnetting is to use host bits to create additional subnets. Subnetting reduces overall network traffic and improves network performance. It helps administrators to implement security policies such as which subnets are allowed or not allowed to communicate together. It reduces the number of devices affected by abnormal broadcast traffic due to misconfigurations, hardware/software problems, or malicious intent

## 9.4.2 Webster - Reflection Questions

- I just sent invitations to a party to several of my friends and family. The invitations went to different addresses, but the card inside is the same for everyone. This is like a multicast email isn’t it? I didn’t know you could do that, and I also didn’t know you could send a broadcast email to every person on your network! Can you think of a good reason to send a broadcast email to everyone in your network? Can you think of a reason why you should be careful before you send a broadcast email?

## 9.4.3 IPv4 and Network Segmentation Quiz
