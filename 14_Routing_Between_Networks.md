## 14.0.1 Webster - Why Should I Take this Module?
Kishori leaves work for the day and begins her drive home. Her friend has called her to warn her that there is a lot of congestion on her usual route home. She used the GPS on her phone to reroute to a less congested road. Kishori wonders if networks can get congested. Do they find a faster route?

Great question Kishori! Networks can also have this issue of congestion slowing down its performance. In a network, the router can determine the best path. How does a network become congested? What can you do to limit that congestion? You and Kishori will find out in this module!



## 14.0.2 What Will I Learn in this Modules?
Module Title: Routing Between Networks

Module Objective: Create a fully connected LAN.




## 14.1.1 Video - Dividing the Local Network
This is a media player component. Select the play / pause button to watch or listen.
Press the Play button to watch the video.





## 14.1.2 Now We Need Routing
In most situations we want our devices to be able to connect beyond our local network: out to other homes, businesses, and the internet. Devices that are beyond the local network segment are known as remote hosts. When a source device sends a packet to a remote destination device, then the help of routers and routing is needed. Routing is the process of identifying the best path to a destination.

A router is a networking device that connects multiple Layer 3, IP networks. At the distribution layer of the network, routers direct traffic and perform other functions critical to efficient network operation. Routers, like switches, are able to decode and read the messages that are sent to them. Unlike switches, which make their forwarding decision based on the Layer 2 MAC address, routers make their forwarding decision based on the Layer 3 IP address.

The packet format contains the IP addresses of the destination and source hosts, as well as the message data being sent between them. The router reads the network portion of the destination IP address and uses it to find which one of the attached networks is the best way to forward the message to the destination.

Anytime the network portion of the IP addresses of the source and destination hosts do not match, a router must be used to forward the message. If a host located on network 1.1.1.0 needs to send a message to a host on network 5.5.5.0, the host will forward the message to the router. The router receives the message, de-encapsulates the Ethernet frame, and then reads the destination IP address in the IP packet. It then determines where to forward the message. It re-encapsulates the packet back into a new frame, and forwards the frame on to its destination.

Click Play to see how the MAC and IP addresses are used.

IP Packet Encapsulated in an Ethernet Frame


## 14.1.3 Check Your Understanding - The Need for Routing
Check your understanding of the need for routing by choosing the correct answer to the following questions.


## 14.2.1 Video - Router Packet Forwarding
## 14.2.2 Video - Messages Within and Between Networks - Part 1


## 14.2.3 Video - Messages Within and Between Networks - Part 2

## 14.2.4 Routing Table Entries
Routers move information between local and remote networks. To do this, routers must use routing tables to store information. Routing tables are not concerned with the addresses of individual hosts. Routing tables contain the addresses of networks, and the best path to reach those networks. Entries can be made to the routing table in two ways: dynamically updated by information received from other routers in the network, or manually entered by a network administrator. Routers use the routing tables to determine which interface to use to forward a message to its intended destination.

If the router cannot determine where to forward a message, it will drop it. Network administrators configure a static default route that is placed into the routing table so that a packet will not be dropped due to the destination network not being in the routing table. A default route is the interface through which the router forwards a packet containing an unknown destination IP network address. This default route usually connects to another router that can forward the packet towards its final destination network.


    Type - The connection type. C stands for directly connected.
Network - The network address.
Port - The interface used to forward packets to the network.


## 14.2.5 The Default Gateway
The method that a host uses to send messages to a destination on a remote network differs from the way a host sends messages on the same local network. When a host needs to send a message to another host located on the same network, it will forward the message directly. A host will use ARP to discover the MAC address of the destination host. The IPv4 packet contains the destination IPv4 address and encapsulates the packet into a frame containing the MAC address of the destination and forwards it out.

When a host needs to send a message to a remote network, it must use the router. The host includes the IP address of the destination host within the packet just like before. However, when it encapsulates the packet into a frame, it uses the MAC address of the router as the destination for the frame. In this way, the router will receive and accept the frame based on the MAC address.

How does the source host determine the MAC address of the router? A host is given the IPv4 address of the router through the default gateway address configured in its TCP/IP settings. The default gateway address is the address of the router interface connected to the same local network as the source host. All hosts on the local network use the default gateway address to send messages to the router. When the host knows the default gateway IPv4 address, it can use ARP to determine the MAC address. The MAC address of the router is then placed in the frame, destined for another network.

It is important that the correct default gateway be configured on each host on the local network. If no default gateway is configured in the host TCP/IP settings, or if the wrong default gateway is specified, messages addressed to hosts on remote networks cannot be delivered.


## 14.2.6 Check Your Understanding - Select the Default Gateway
Refer to the figure. Select default gateway for each of the following questions.



## 14.2.7 Check Your Understanding - The Routing Table
Check your understanding of the routing table by choosing the correct answer to the following questions.



## 14.3.1 Local Area Networks
The term local area network (LAN) refers to a local network, or a group of interconnected local networks that are under the same administrative control. In the early days of networking, LANs were defined as small networks that existed in a single physical location. Although LANs can be a single local network installed in a home or small office, the definition of LAN has evolved to include interconnected local networks consisting of many hundreds of hosts, installed in multiple buildings and locations.

The important thing to remember is that all the local networks within a LAN are under one administrative control. Other common characteristics of LANs are that they typically use Ethernet or wireless protocols, and they support high data rates.

The term intranet is often used to refer to a private LAN that belongs to an organization, and is designed to be accessible only by the members of the organization, employees, or others with authorization.


## 14.3.2 Local and Remote Network Segments
List of expandable sections. Select each button to expand the content.
Within a LAN, it is possible to place all hosts on a single local network or divide them up between multiple networks connected by a distribution layer device. How this placement is determined depends on desired results.

Click below to learn more about local and remote network segments.


All Hosts in One Local Segment
Placing all hosts on a single local network allows them to be seen by all other hosts. This is because there is one broadcast domain and hosts use ARP to find each other.

In a simple network design, it may be beneficial to keep all hosts within a single local network. However, as networks grow in size, increased traffic will decrease network performance and speed. In this case, it may be beneficial to move some hosts onto a remote network.

Advantages of a single local segment:

Appropriate for simpler networks
Less complexity and lower network cost
Allows devices to be "seen" by other devices
Faster data transfer - more direct communication
Ease of device access
Disadvantages of a single local segment:

All hosts are in one broadcast domain which causes more traffic on the segment and may slow network performance
Harder to implement QoS
Harder to implement security



## 14.3.2 Local and Remote Network Segments
List of expandable sections. Select each button to expand the content.
Within a LAN, it is possible to place all hosts on a single local network or divide them up between multiple networks connected by a distribution layer device. How this placement is determined depends on desired results.

Click below to learn more about local and remote network segments.


Hosts on a Remote Segment
Placing additional hosts on a remote network will decrease the impact of traffic demands. However, hosts on one network will not be able to communicate with hosts on the other network without the use of routing. Routers increase the complexity of the network configuration and can introduce latency, or time delay, on packets sent from one local network to the other.

Advantages:

More appropriate for larger, more complex networks
Splits up broadcast domains and decreases traffic
Can improve performance on each segment
Makes the machines invisible to those on other local network segments
Can provide increased security
Can improve network organization
Disadvantages:

Requires the use of routing (distribution layer)
Router can slow traffic between segments
More complexity and expense (requires a router)




## 14.3.3 Packet Tracer - Observe Traffic Flow in a Routed Network
In this Packet Tracer activity, you will complete the following objectives:

Part 1: Observe Traffic Flow in an Unrouted LAN
Part 2: Reconfigure the Network to Route Between LANs
Part 3: Observe Traffic Flow in the Routed Network



## 14.3.4 Packet Tracer - Create a LAN
In this Packet Tracer activity, you will complete the following objectives:

Connect Network Devices and Hosts
Configure Devices with IPv4 Addressing
Verify the End Device Configuration and Connectivity
Use Networking Commands to View Host Information




## 14.4.1 What Did I Learn in this Module?

The Need for Routing
As networks grow, it is often necessary to divide one access layer network into multiple access layer networks. There are many ways to divide networks based on different criteria:

Broadcast containment - Routers in the distribution layer can limit broadcasts to the local network where they need to be heard.
Security requirements - Routers in the distribution layer can separate and protect certain groups of computers where confidential information resides.
Physical locations - Routers in the distribution layer can be used to interconnect local networks at various locations of an organization that are geographically separated.
Logical grouping - Routers in the distribution layer can be used to logically group users, such as departments within a company, who have common needs or for access to resources.
The distribution layer connects these independent local networks and controls the traffic flowing between them. It is responsible for ensuring that traffic between hosts on the local network stays local.

A router is a networking device that connects multiple Layer 3, IP networks. At the distribution layer of the network, routers direct traffic and perform other functions critical to efficient network operation. Routers, like switches, are able to decode and read the messages that are sent to them. Unlike switches, which make their forwarding decision based on the Layer 2 MAC address, routers make their forwarding decision based on the Layer 3 IP address.

Anytime the network portion of the IP addresses of the source and destination hosts do not match, a router must be used to forward the message.




## 14.4.1 What Did I Learn in this Module?

The Routing Table
Each port, or interface, on a router connects to a different local network. Every router contains a table of all locally connected networks and the interfaces that connect to them.

When a router receives a frame, it decodes the frame to get to the packet containing the destination IP address. It matches the network portion of the destination IP address to the networks that are listed in the routing table. If the destination network address is in the table, the router encapsulates the packet in a new frame in order to send it out. It forwards the new frame out of the interface associated with the path, to the destination network. The process of forwarding the packets toward their destination network is called routing.

A router forwards a packet to one of two places: a directly connected network containing the actual destination host, or to another router on the path to reach the destination host. When a router encapsulates the frame to forward it out a routed interface, it must include a destination MAC address. If the router must forward the packet to another router through a routed interface, it will use the MAC address of the connected router. Routers obtain these MAC addresses from ARP tables.

A host is given the IPv4 address of the router through the default gateway address configured in its TCP/IP settings. The default gateway address is the address of the router interface connected to the same local network as the source host. All hosts on the local network use the default gateway address to send messages to the router.

Routing tables contain the addresses of networks, and the best path to reach those networks. Entries can be made to the routing table in two ways: dynamically updated by information received from other routers in the network, or manually entered by a network administrator.


Create a LAN
LAN refers to a local network, or a group of interconnected local networks that are under the same administrative control. All the local networks within a LAN are under one administrative control. Other common characteristics of LANs are that they typically use Ethernet or wireless protocols, and they support high data rates.

Within a LAN, it is possible to place all hosts on a single local network or divide them up between multiple networks connected by a distribution layer device.

Placing all hosts on a single local network allows them to be seen by all other hosts. This is because there is one broadcast domain and hosts use ARP to find each other.

Placing additional hosts on a remote network will decrease the impact of traffic demands. However, hosts on one network will not be able to communicate with hosts on the other network without the use of routing. Routers increase the complexity of the network configuration and can introduce latency, or time delay, on packets sent from one local network to the other.



## 14.4.2 Webster - Reflection Questions
On my home network (LAN), I do not usually have enough network traffic to experience congestion, although it can happen when all my children are streaming different movies and I am trying to upload a document to my work. Can you think of a way that I could divide my LAN into multiple networks?



