11.0.1 Webster - Why Should I Take this Module?

Kishori’s nursing station just received a new laptop from the IT department. The IT specialist, Madhav, is setting it up on the desk and trying to connect to the network. He asks Kishori to log in to the computer. She enters her username and password and attempts to access a patient file. She explains that there must be a connection error. Madhav takes a seat to further investigate. Madhav checks the cable and it is connected. On his tablet, he pulls up the list of IPv4 addresses for all of the computers on this floor on this network. He found the issue! There is an error in the IPv4 address. Madhav explains that the intern in their department may have manually configured the network information on this host, rather than using Dynamic Host Configuration Protocol (DHCP). Kishori has not heard about DHCP. She is going to do some reading on this topic.

Are you ready to learn about DHCP? I am here to help! Let's get started with this module!



11.0.2 What Will I Learn in this Module?
Module Title: Dynamic Addressing with DHCP

Module Objective: Configure a DHCP server




11.1.1 Static IPv4 Address Assignment
IPv4 addresses can be assigned either statically or dynamically.

With a static assignment, the network administrator must manually configure the network information for a host. At a minimum, this includes the following:

IP address - This identifies the host on the network.
Subnet mask - This is used to identify the network on which the host is connected.
Default gateway - This identifies the networking device that the host uses to access the internet or another remote network.
Static addresses have some advantages. For instance, they are useful for printers, servers, and other networking devices that need to be accessible to clients on the network. If hosts normally access a server at a particular IPv4 address, it would not be good if that address changed.

Static assignment of addressing information can provide increased control of network resources, but it can be time consuming to enter the information on each host. When IPv4 addresses are entered statically, the host only performs basic error checks on the IPv4 address. Therefore, errors are more likely to occur.

When using static IPv4 addressing, it is important to maintain an accurate list of which IPv4 addresses are assigned to which devices. Additionally, these are permanent addresses and are not normally reused.

11.1.2 Dynamic IPv4 Address Assignment
On local networks it is often the case that the user population changes frequently. New users arrive with laptops and need a connection. Others have new workstations that need to be connected. Rather than have the network administrator assign IPv4 addresses for each workstation, it is easier to have IPv4 addresses assigned automatically. This is done using a protocol known as Dynamic Host Configuration Protocol (DHCP).

DHCP automatically assigns addressing information such as IPv4 address, subnet mask, default gateway, and other configuration information, as shown in the figure.

DHCP is generally the preferred method of assigning IPv4 addresses to hosts on large networks because it reduces the burden on network support staff and virtually eliminates entry errors.

Another benefit of DHCP is that an address is not permanently assigned to a host but is only leased for a period of time. If the host is powered down or taken off the network, the address is returned to the pool for reuse. This is especially helpful with mobile users that come and go on a network.









11.1.3 DHCP Servers
If you enter an airport or coffee shop with a wireless hotspot, DHCP makes it possible for you to access the internet. As you enter the area, your laptop DHCP client contacts the local DHCP server via a wireless connection. The DHCP server assigns an IPv4 address to your laptop.

Various types of devices can be DHCP servers as long as they are running DHCP service software. With most medium to large networks, the DHCP server is usually a local dedicated PC-based server.

With home networks, the DHCP server may be located at the ISP and a host on the home network receives its IPv4 configuration directly from the ISP, as shown in the figure.















Many home networks and small businesses use a wireless router and modem. In this case, the wireless router is both a DHCP client and a server. The wireless router acts as a client to receive its IPv4 configuration from the ISP and then acts as a DHCP server for internal hosts on the local network. The router receives the public IPv4 address from the ISP, and in its role as a DHCP server, it distributes private addresses to internal hosts.

In addition to PC-based servers and wireless routers, other types of networking devices such as dedicated routers can provide DHCP services to clients, although this is not as common.














11.1.4 Check Your Understanding - Static and Dynamic Addressing
Check your understanding of static and dynamic addressing by choosing the correct answer to the following questions.












11.2.1 Video - DHCPv4 Operation

11.2.2 Video - DHCP Service Configuration



11.2.3 Packet Tracer - Configure DHCP on a Wireless Router
In this activity, you will complete the following objectives:

Connect 3 PCs to a wireless router.
Change the DHCP setting to a specific network range.
Configure the clients to obtain their address via DHCP.




11.3.1 What Did I Learn in this Module?

Static and Dynamic Addressing
With a static assignment, the network administrator must manually configure the network information for a host. At a minimum, this includes the host IPv4 address, subnet mask, and default gateway. Static assignment of addressing information can provide increased control of network resources, but it can be time consuming to enter the information on each host. When using static IPv4 addressing, it is important to maintain an accurate list of which IPv4 addresses are assigned to which devices.

IPv4 addresses can be assigned automatically using a protocol known as DHCP. DHCP is generally the preferred method of assigning IPv4 addresses to hosts on large networks because it reduces the burden on network support staff and virtually eliminates entry errors. Another benefit of DHCP is that an address is not permanently assigned to a host but is only leased for a period of time. If the host is powered down or taken off the network, the address is returned to the pool for reuse.

As you enter area with a wireless hotspot, your laptop DHCP client contacts the local DHCP server via a wireless connection. The DHCP server assigns an IPv4 address to your laptop. With home networks, the DHCP server may be located at the ISP and a host on the home network receives its IPv4 configuration directly from the ISP. Many home networks and small businesses use a wireless router and modem. In this case, the wireless router is both a DHCP client and a server.

11.3.1 What Did I Learn in this Module?

DHCPv4 Configuration
The DHCP server is configured with a range, or pool, of IPv4 addresses that can be assigned to DHCP clients. A client that needs an IPv4 address will send a DHCP Discover message which is a broadcast with a destination IPv4 address of 255.255.255.255 (32 ones) and a destination MAC address of FF-FF-FF-FF-FF-FF (48 ones). All hosts on the network will receive this broadcast DHCP frame, but only a DHCP server will reply. The server will respond with a DHCP Offer, suggesting an IPv4 address for the client. The host then sends a DHCP Request asking to use the suggested IPv4 address. The server responds with a DHCP Acknowledgment.

For most home and small business networks, a wireless router provides DHCP services to the local network clients. To configure a home wireless router, access its graphical web interface by opening the browser and entering the router default IPv4 address. The IPv4 address of 192.168.0.1 and subnet mask of 255.255.255.0 are the defaults for the internal router interface. This is the default gateway for all hosts on the local network and also the internal DHCP server IPv4 address. Most home wireless routers have DHCP Server enabled by default.




11.3.2 Webster - Reflection Questions

Have you manually entered an IPv4 address for all the devices on your home network? These are called static addresses. I did this for my home network, and I made a mistake when entering the address for my tablet. I had to redo it. Can you imagine having to do this for a huge corporate network with hundreds, or even thousands of devices? What other advantages are there to using DHCP for device addressing?



11.3.3 Dynamic Addressing with DHCP Quiz






