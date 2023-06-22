[Back to Syllabus](./README.md#course-syllabus)

## 8.0.1 Webster - Why Should I Take this Module?8.0.1 Webster - Why Should I Take this Module?

- Kishori is learning a lot from Rina! She understands that when she sends or receives a package in the mail, there is a unique address involved. A postal code is critical in the address to route the package to the correct post office. She asks Rina if computers use something like a zip code to route the message to the correct place. Rina goes into more detail about the process and explains that much like Kishori’s home address identifies where she lives, an IPv4 address identifies a host on the network. A host needs an IPv4 address to participate on the internet and almost all LANs today. Every packet sent across the internet has a source and destination IPv4 address. This information is required by networking devices to ensure the information gets to the destination and any replies are returned to the source
- My friend Kishori never thought she would be so interested in all of this tech information, but she really wants to learn more! Do you? Take this module to learn about the Internet Protocol and the structure of IPv4 addresses!

## 8.0.2 What Will I Learn in this Module?

- Module Title: The Internet Protocol
- Module Objective: Explain the features of an IP address

## 8.1.1 The IPv4 Address

- A host needs an IPv4 address to participate on the internet and almost all LANs today. The IPv4 address is a logical network address that identifies a particular host. It must be properly configured and unique within the LAN, for local communication. It must also be properly configured and unique in the world, for remote communication. This is how a host is able to communicate with other devices on the internet
- An IPv4 address is assigned to the network interface connection for a host. This connection is usually a network interface card (NIC) installed in the device. Examples of end-user devices with network interfaces include workstations, servers, network printers, and IP phones. Some servers can have more than one NIC and each of these has its own IPv4 address. Router interfaces that provide connections to an IP network will also have an IPv4 address
- Every packet sent across the internet has a source and destination IPv4 address. This information is required by networking devices to ensure the information gets to the destination and any replies are returned to the source
- This animation consists of a user sitting at a desktop p c with I P address 192.168.200.8 which is connected to the internet. The p c is sending packets to a remote web server, www.cisco.com, at IP address 192.168.5.100. Also connected to the internet cloud are two other servers, Business A at 172.16.30.5 and Business B at 10.5.105.50

## 8.1.2 Octets and Dotted-Decimal Notation

- IPv4 addresses are 32 bits in length. Here is an IPv4 address in binary: 11010001101001011100100000000001
- Notice how difficult this address is to read. Imagine having to configure devices with a series of 32 bits! For this reason, the 32 bits are grouped into four 8-bit bytes called octets like this: 11010001.10100101.11001000.00000001
- That's better, but still difficult to read. That's why we convert each octet into its decimal value, separated by a decimal point or period. The above binary IPv4 becomes this dotted-decimal representation: 209.165.200.1
- Note: For now, you do not need to know how to convert between binary and decimal number systems

## 8.1.3 Packet Tracer - Connect to a Web Server

In this activity, you will observe how packets are sent across the internet using IP addresses.

## 8.2.1 Video - The IPv4 Address Structure

## 8.2.2 Networks and Hosts

- The logical 32-bit IPv4 address is hierarchical and is made up of two parts, the network and the host. In the figure, the network portion is blue, and the host portion is red. Both parts are required in an IPv4 address. Both networks have the subnet mask 255.255.255.0. The subnet mask is used to identify the network on which the host is connected
- As an example, there is a host with an IPv4 address 192.168.5.11 with a subnet mask of 255.255.255.0. The first three octets, (192.168.5), identify the network portion of the address, and the last octet, (11) identifies the host. This is known as hierarchical addressing because the network portion indicates the network on which each unique host address is located. Routers only need to know how to reach each network, rather than needing to know the location of each individual host
- With IPv4 addressing, multiple logical networks can exist on one physical network if the network portion of the logical network host addresses is different. For example: three hosts on a single, physical local network have the same network portion of their IPv4 address (192.168.18) and three other hosts have different network portions of their IPv4 addresses (192.168.5). The hosts with the same network number in their IPv4 addresses will be able to communicate with each other, but will not be able to communicate with the other hosts without the use of routing. In this example, there is one physical network and two logical IPv4 networks
- Another example of a hierarchical network is the telephone system. With a telephone number, the country code, area code, and exchange represent the network address and the remaining digits represent a local phone number

## 8.2.3 Check Your Understanding - IPv4 Address Structure

- Check your understanding of IPv4 address structure by choosing the correct answer to the following questions

## 8.3.1 What Did I Learn in this Module?

- Purpose of the ipv4 address:The IPv4 address is a logical network address that identifies a particular host. It must be properly configured and unique within the LAN, for local communication. It must also be properly configured and unique in the world, for remote communication
- An IPv4 address is assigned to the network interface connection for a host. This connection is usually a NIC installed in the device
- Every packet sent across the internet has a source and destination IPv4 address. This information is required by networking devices to ensure the information gets to the destination and any replies are returned to the source
- The ipv4 address structure:
    - The logical 32-bit IPv4 address is hierarchical and is made up of two parts, the network, and the host. As an example, there is a host with an IPv4 address 192.168.5.11 with a subnet mask of 255.255.255.0. The first three octets, (192.168.5), identify the network portion of the address, and the last octet, (11) identifies the host. This is known as hierarchical addressing because the network portion indicates the network on which each unique host address is located
    - Routers only need to know how to reach each network, rather than needing to know the location of each individual host. With IPv4 addressing, multiple logical networks can exist on one physical network if the network portion of the logical network host addresses is different

## 8.3.2 Webster - Reflection Questions

- It makes sense that every device on the network has an IP address, and routers use these addresses to send packets from the source to the destination. When I send a letter through the mail, I put my address and the address of the recipient on the envelope. But now I see the other connection to how networks operate. The postal code and city of my recipient is a little bit like the network portion of the IP address, and the street address is like the host portion of the IP address. Can you think of any other analogies to network operations and IP addresses?

## 8.3.3 The Internet Protocol Quiz

[Go to Next Module](./9_IPv4_and_Network_Segmentation.md)
