14.0.1 Webster - Why Should I Take this Module?
Kishori leaves work for the day and begins her drive home. Her friend has called her to warn her that there is a lot of congestion on her usual route home. She used the GPS on her phone to reroute to a less congested road. Kishori wonders if networks can get congested. Do they find a faster route?

Great question Kishori! Networks can also have this issue of congestion slowing down its performance. In a network, the router can determine the best path. How does a network become congested? What can you do to limit that congestion? You and Kishori will find out in this module!



14.0.2 What Will I Learn in this Modules?
Module Title: Routing Between Networks

Module Objective: Create a fully connected LAN.




14.1.1 Video - Dividing the Local Network
This is a media player component. Select the play / pause button to watch or listen.
Press the Play button to watch the video.





14.1.2 Now We Need Routing
In most situations we want our devices to be able to connect beyond our local network: out to other homes, businesses, and the internet. Devices that are beyond the local network segment are known as remote hosts. When a source device sends a packet to a remote destination device, then the help of routers and routing is needed. Routing is the process of identifying the best path to a destination.

A router is a networking device that connects multiple Layer 3, IP networks. At the distribution layer of the network, routers direct traffic and perform other functions critical to efficient network operation. Routers, like switches, are able to decode and read the messages that are sent to them. Unlike switches, which make their forwarding decision based on the Layer 2 MAC address, routers make their forwarding decision based on the Layer 3 IP address.

The packet format contains the IP addresses of the destination and source hosts, as well as the message data being sent between them. The router reads the network portion of the destination IP address and uses it to find which one of the attached networks is the best way to forward the message to the destination.

Anytime the network portion of the IP addresses of the source and destination hosts do not match, a router must be used to forward the message. If a host located on network 1.1.1.0 needs to send a message to a host on network 5.5.5.0, the host will forward the message to the router. The router receives the message, de-encapsulates the Ethernet frame, and then reads the destination IP address in the IP packet. It then determines where to forward the message. It re-encapsulates the packet back into a new frame, and forwards the frame on to its destination.

Click Play to see how the MAC and IP addresses are used.

IP Packet Encapsulated in an Ethernet Frame


14.1.3 Check Your Understanding - The Need for Routing
Check your understanding of the need for routing by choosing the correct answer to the following questions.



