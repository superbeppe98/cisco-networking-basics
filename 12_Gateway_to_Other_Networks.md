

## 12.0.1 Webster - Why Should I Take this Module?
Kishori receives an email from Rina asking if they can meet in the cafeteria for lunch. Kishori meets Rina and is eager to ask her a few more networking questions. Rina is always happy to share her knowledge. When Kishori was speaking with Madhav, she learned that her department is part of a LAN. Each department within the hospital has its own LAN. Kishori asks Rina how she is able to send and receive emails that are outside of her network. Rina explains that gateways and Network Address Translation (NAT) make all of this seamless communication possible. Rina is impressed with Kishori’s new knowledge and interest in networking! She mentions that there are several nurses in the hospital that have this knowledge and are paid more because they are able to troubleshoot the devices in the patient’s room. She recommends that Kishori take some courses so that she could eventually apply for this promotion. Wow! Who knew that nurses could get promoted by learning technology!

This module will help Kishori understand gateways and NAT. Are you ready to learn more? Let's go!



## 12.0.2 What Will I Learn in this Module?
Module Title: Gateways to Other Networks

Module Objective: Explain how routers connect networks together.


## 12.1.1 Video - Gateways to Other Networks
This is a media player component. Select the play / pause button to watch or listen.
Press the Play button to watch the video.


## 12.1.2 Routers as Gateways
The router provides a gateway through which hosts on one network can communicate with hosts on different networks. Each interface on a router is connected to a separate network.

The IPv4 address assigned to the interface identifies which local network is connected directly to it.

Every host on a network must use the router as a gateway to other networks. Therefore, each host must know the IPv4 address of the router interface connected to the network where the host is attached. This address is known as the default gateway address. It can be either statically configured on the host or received dynamically by DHCP.

When a wireless router is configured to be a DHCP server for the local network, it automatically sends the correct interface IPv4 address to the hosts as the default gateway address. In this manner, all hosts on the network can use that IPv4 address to forward messages to hosts located at the ISP and get access to hosts on the internet. Wireless routers are usually set to be DHCP servers by default.

The IPv4 address of that local router interface becomes the default gateway address for the host configuration. The default gateway is provided, either statically or by DHCP.

When a wireless router is configured as a DHCP server, it provides its own internal IPv4 address as the default gateway to DHCP clients. It also provides them with their respective IPv4 address and subnet mask, as shown in the figure.


## 12.1.3 Routers as Boundaries Between Networks
The wireless router acts as a DHCP server for all local hosts attached to it, either by Ethernet cable or wirelessly. These local hosts are referred to as being located on an internal, or inside, network. Most DHCP servers are configured to assign private addresses to the hosts on the internal network, rather than internet routable public addresses. This ensures that, by default, the internal network is not directly accessible from the internet.

The default IPv4 address configured on the local wireless router interface is usually the first host address on that network. Internal hosts must be assigned addresses within the same network as the wireless router, either statically configured, or through DHCP. When configured as a DHCP server, the wireless router provides addresses in this range. It also provides the subnet mask information and its own interface IPv4 address as the default gateway, as shown in the figure.

Many ISPs also use DHCP servers to provide IPv4 addresses to the internet side of the wireless router installed at their customer sites. The network assigned to the internet side of the wireless router is referred to as the external, or outside, network.

When a wireless router is connected to the ISP, it acts like a DHCP client to receive the correct external network IPv4 address for the internet interface. ISPs usually provide an internet-routable address, which enables hosts connected to the wireless router to have access to the internet.

The wireless router serves as the boundary between the local internal network and the external internet.




## 12.1.4 Check Your Understanding - Network Boundaries
Check your understanding of network boundaries by choosing the correct answer to the following questions.


## 12.2.1 Video - Introduction to NAT



12.2.2 Packet Tracer - Examine NAT on a Wireless Router
In this activity, you will complete the following objectives:

Examine NAT configuration on a wireless router.
Set up 4 PCs to connect to a wireless router using DHCP.
Examine traffic that crosses the network using NAT.



## 12.3.1 What Did I Learn in this Module?

Network Boundaries
Every host on a network must use the router as a gateway to other networks. Therefore, each host must know the IPv4 address of the router interface connected to the network where the host is attached. This address is known as the default gateway address. It can be either statically configured on the host or received dynamically by DHCP.

The wireless router acts as a DHCP server for all local hosts attached to it, either by Ethernet cable or wirelessly. These local hosts are referred to as being located on an internal, or inside, network. When a wireless router is connected to the ISP, it acts like a DHCP client to receive the correct external network IPv4 address for the internet interface. ISPs usually provide an internet-routable address, which enables hosts connected to the wireless router to have access to the internet. The wireless router serves as the boundary between the local internal network and the external internet.


NAT Operation
The wireless router receives a public address from the ISP, which allows it to send and receive packets on the internet. It, in turn, provides private addresses to local network clients.

The process used to convert private addresses to internet-routable addresses is called NAT. With NAT, a private (local) source IPv4 address is translated to a public (global) address. The process is reversed for incoming packets. The wireless router is able to translate many internal IPv4 addresses to the same public address, by using NAT.

Only packets destined for other networks need to be translated. These packets must pass through the gateway, where the wireless router replaces the private IPv4 address of the source host with its own public IPv4 address.



## 12.3.2 Webster - Reflection Questions
It turns out that the IPv4 addresses on the devices in my home network are private addresses that are only used in my LAN. But if I need to venture out beyond my home network, perhaps to go to the internet, or send an email to someone outside of my network, my device needs to be assigned a public address. How does your router know if you are trying to get access to a device or a website that is outside of your LAN? How do you know that your private address has been translated into a public address?



## 12.3.3 Gateways to Other Networks Quiz
