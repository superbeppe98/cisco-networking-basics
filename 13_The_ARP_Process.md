13.0.1 Webster - Why Should I Take this Module
Kishori was looking at her phone and noticed that her phone actually has its own IP address. She went home and noticed that the IP address had changed to a value that is different from the address that she had at the hospital. She remembered that DHCP provides addresses to devices automatically, so she thinks that she gets IP addresses from different places depending on where she is. This makes sense to her because she knows these addresses permit devices to join different networks. Kishori also notices that her phone has a MAC address. She has checked and she notices that the MAC address is always the same, no matter which network she is attached to. It makes sense to Kishori, that her IP address changes when she is connected to different networks in different locations, but her MAC address is always the same, because her phone is her phone no matter where she is.

This means that both IP and MAC addresses must be required in order for the phone to receive data. The IP address tells the sender of data where she is, and once the data gets to her location, the MAC address of her phone permits the device to receive data that is meant just for her. Thinking further, Kishori wonders how MAC addresses can be known to the network. DHCP provides the correct IP addresses for the network, but each device has its own, unique MAC address.

Kishori is ready to learn more! Are you? Keep reading!




13.0.2 What Will I Learn in this Module?
Module Title: The ARP Process

Module Objective: Explain how ARP enables communication on a network.


13.1.1 Destination on Same Network
Sometimes a host must send a message, but it only knows the IP address of the destination device. The host needs to know the MAC address of that device, but how can it be discovered? That is where address resolution becomes critical.

There are two primary addresses assigned to a device on an Ethernet LAN:

Physical address (the MAC address) – Used for NIC-to-NIC communications on the same Ethernet network.
Logical address (the IP address) – Used to send the packet from the source device to the destination device. The destination IP address may be on the same IP network as the source, or it may be on a remote network.
Layer 2 physical addresses (i.e., Ethernet MAC addresses) are used to deliver the data link frame with the encapsulated IP packet from one NIC to another NIC that is on the same network. If the destination IP address is on the same network, the destination MAC address will be that of the destination device.

Consider the following example using simplified MAC address representations.



In this example, PC1 wants to send a packet to PC2. The figure displays the Layer 2 destination and source MAC addresses and the Layer 3 IPv4 addressing that would be included in the packet sent from PC1.

The Layer 2 Ethernet frame contains the following:

Destination MAC address – This is the simplified MAC address of PC2, 55-55-55.
Source MAC address – This is the simplified MAC address of the Ethernet NIC on PC1, aa-aa-aa.
The Layer 3 IP packet contains the following:

Source IPv4 address – This is the IPv4 address of PC1, 192.168.10.10.
Destination IPv4 address – This is the IPv4 address of PC2, 192.168.10.11.





13.1.2 Destination on Remote Network
When the destination IP address (IPv4 or IPv6) is on a remote network, the destination MAC address will be the address of the host default gateway (i.e., the router interface).

Consider the following example using a simplified MAC address representation.



In this example, PC1 wants to send a packet to PC2. PC2 is located on remote network. Because the destination IPv4 address is not on the same local network as PC1, the destination MAC address is that of the local default gateway on the router.

Routers examine the destination IPv4 address to determine the best path to forward the IPv4 packet. When the router receives the Ethernet frame, it de-encapsulates the Layer 2 information. Using the destination IPv4 address, it determines the next-hop device, and then encapsulates the IPv4 packet in a new data link frame for the outgoing interface.

In our example, R1 would now encapsulate the packet with new Layer 2 address information, as shown in the figure.


The new destination MAC address would be that of the R2 G0/0/1 interface and the new source MAC address would be that of the R1 G0/0/1 interface.

Along each link in a path, an IP packet is encapsulated in a frame. The frame is specific to the data link technology that is associated with that link, such as Ethernet. If the next-hop device is the final destination, the destination MAC address will be that of the device Ethernet NIC, as shown in the figure.



How are the IP addresses of the IP packets in a data flow associated with the MAC addresses on each link along the path to the destination? For IPv4 packets, this is done through a process called Address Resolution Protocol (ARP). For IPv6 packets, the process is ICMPv6 Neighbor Discovery (ND).




13.1.3 Packet Tracer - Identify MAC and IP Addresses
In this Packet Tracer activity, you will complete the following objectives:

Gather PDU Information for Local Network Communication
Gather PDU Information for Remote Network Communication
This activity is optimized for viewing PDUs. The devices are already configured. You will gather PDU information in simulation mode and answer a series of questions about the data you collect.




13.1.4 Check Your Understanding - MAC and IP
Check your understanding of MAC and IP addressing by choosing the BEST answer to the following questions.





13.2.1 Video - The Ethernet Broadcast
This is a media player component. Select the play / pause button to watch or listen.
Press the Play button to watch the video.





13.2.2 Broadcast Domains
When a host receives a message addressed to the broadcast address, it accepts and processes the message as though the message was addressed directly to it. When a host sends a broadcast message, switches forward the message to every connected host within the same local network. For this reason, a local area network, a network with one or more Ethernet switches, is also referred to as a broadcast domain.

If too many hosts are connected to the same broadcast domain, broadcast traffic can become excessive. The number of hosts and the amount of network traffic that can be supported on the local network is limited by the capabilities of the switches used to connect them. As the network grows and more hosts are added, network traffic, including broadcast traffic, increases. To improve performance, it is often necessary to divide one local network into multiple networks, or broadcast domains, as shown in the figure. Routers are used to divide the network into multiple broadcast domains.



13.2.3 Access Layer Communication
On a local Ethernet network, a NIC only accepts a frame if the destination address is either the broadcast MAC address, or else corresponds to the MAC address of the NIC.

Most network applications, however, rely on the logical destination IP address to identify the location of the servers and clients. The figure illustrates the problem that arises if a sending host only has the logical IP address of the destination host. How does the sending host determine what destination MAC address to place within the frame?

The sending host can use an IPv4 protocol called address resolution protocol (ARP) to discover the MAC address of any host on the same local network. IPv6 uses a similar method known as Neighbor Discovery.



13.2.4 Video - Address Resolution Protocol





13.2.5 ARP
ARP uses a three step process to discover and store the MAC address of a host on the local network when only the IPv4 address of the host is known:

The sending host creates and sends a frame addressed to a broadcast MAC address. Contained in the frame is a message with the IPv4 address of the intended destination host.
Each host on the network receives the broadcast frame and compares the IPv4 address inside the message with its configured IPv4 address. The host with the matching IPv4 address sends its MAC address back to the original sending host.
The sending host receives the message and stores the MAC address and IPv4 address information in a table called an ARP table.
When the sending host has the MAC address of the destination host in its ARP table, it can send frames directly to the destination without doing an ARP request. Because ARP messages rely on broadcast frames to deliver the requests, all hosts in the local IPv4 network must be in the same broadcast domain.

Click Play in the figure to see an animation of the ARP process.



13.2.6 Check Your Understanding - Broadcast Containment
Check your understanding of broadcast containment by choosing the correct answer to the following questions.

13.3.1 What Did I Learn in this Module?

MAC and IP
Sometimes a host must send a message, but it only knows the IP address of the destination device. The host needs to know the MAC address of that device. The MAC address can be discovered using address resolution. There are two primary addresses assigned to a device on an Ethernet LAN:

Physical address (the MAC address) – Used for NIC-to-NIC communications on the same Ethernet network.
Logical address (the IP address) – Used to send the packet from the source device to the destination device. The destination IP address may be on the same IP network as the source, or it may be on a remote network.
When the destination IP address (IPv4 or IPv6) is on a remote network, the destination MAC address will be the address of the host default gateway (i.e., the router interface). Routers examine the destination IPv4 address to determine the best path to forward the IPv4 packet. When the router receives the Ethernet frame, it de-encapsulates the Layer 2 information. Using the destination IPv4 address, it determines the next-hop device, and then encapsulates the IPv4 packet in a new data link frame for the outgoing interface. Along each link in a path, an IP packet is encapsulated in a frame. The frame is specific to the data link technology that is associated with that link, such as Ethernet. If the next-hop device is the final destination, the destination MAC address will be that of the device Ethernet NIC.



Broadcast Containment
A message can only contain one destination MAC address. Address resolution lets a host send a broadcast message to a unique MAC address that is recognized by all hosts. The broadcast MAC address is a 48-bit address made up of all ones. MAC addresses are usually represented in hexadecimal notation. The broadcast MAC address in hexadecimal notation is FFFF.FFFF.FFFF. Each F in the hexadecimal notation represents four ones in the binary address.

When a host sends a broadcast message, switches forward the message to every connected host within the same local network. For this reason, a local area network, a network with one or more Ethernet switches, is also referred to as a broadcast domain.

If too many hosts are connected to the same broadcast domain, broadcast traffic can become excessive. The number of hosts and the amount of network traffic that can be supported on the local network is limited by the capabilities of the switches used to connect them. To improve performance, you may need to divide one local network into multiple networks, or broadcast domains. Routers are used to divide the network into multiple broadcast domains.

On a local Ethernet network, a NIC only accepts a frame if the destination address is either the broadcast MAC address, or else corresponds to the MAC address of the NIC. Most network applications rely on the logical destination IP address to identify the location of the servers and clients. How does the sending host determine what destination MAC address to place within the frame? The sending host can ARP to discover the MAC address of any host on the same local network.

ARP uses a three-step process to discover and store the MAC address of a host on the local network when only the IPv4 address of the host is known:

The sending host creates and sends a frame addressed to a broadcast MAC address. Contained in the frame is a message with the IPv4 address of the intended destination host.
Each host on the network receives the broadcast frame and compares the IPv4 address inside the message with its configured IPv4 address. The host with the matching IPv4 address sends its MAC address back to the original sending host.
The sending host receives the message and stores the MAC address and IPv4 address information in a table called an ARP table.
IPv6 uses a similar method known as Neighbor Discovery.




13.3.2 Webster - Reflection Questions
All of my devices (and all of your devices) have an IP address, and a MAC address. When someone wants to send a message to my phone, my IP address tells their router where my device is. My MAC address is how my phone knows to let me see the message. That router also needs to know my MAC address and uses ARP to find it. Do you know how to look up the MAC address of each of your connected devices?




