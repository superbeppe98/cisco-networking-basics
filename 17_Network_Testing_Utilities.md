[Back to Syllabus](./README.md#course-syllabus)

## 17.0.1 Webster - Why Should I Take this Module?
- Kishori tries to reach a website using her desktop computer at her nursing station. She gets an error message when trying to reach the site. She checks the wired connection, and it is fine. She uses her laptop to try to reach that same website with no success. On the desktop, she goes to the command prompt and pings a different website on the internet. Now she realizes she has no connection. She calls the IT department. Madhav comes to the station to further investigate the issue. Madhav pings a website. Kishori explains that she tried that already. Then he pings the default gateway and receives a reply. The router is working. It is the ISP that is down. Madhav is impressed that Kishori has learned so much over the past few months. He tells her that she should apply for that promotion and that she can use him as a reference!
- Are you ready to learn some troubleshooting commands? Keep reading!

## 17.0.2 What Will I Learn in this Module?

- Module Title: Network Testing Utilities
- Module Objective: Use various tools to test and troubleshoot network connectivity

## 17.1.1 Overview of Troubleshooting Commands
- A number of software utility programs are available that can help identify network problems. Most of these utilities are provided by the operating system as command line interface (CLI) commands. The syntax for the commands may vary between operating systems
- Some of the available utilities include:
    - ipconfig - Displays IP configuration information
    - ping - Tests connections to other IP hosts
    - netstat - Displays network connections
    - tracert - Displays the route taken to the destination
    - nslookup - Directly queries the name server for information on a destination domain

## 17.1.2 The ipconfig Command
- When a device does not get an IP address, or has an incorrect IP configuration, it cannot communicate on the network or access the internet. On Windows devices, you can view the IP configuration information with the ipconfig command at the command prompt. The ipconfig command has several options that are helpful including /all, /release, and /renew
- Click below for examples of the ipconfig command.
    - ipconfig
        - The ipconfig command is used to display the current IP configuration information for a host. Issuing this command from the command prompt will display the basic configuration information including IP address, subnet mask, and default gateway
    - ipconfig /all
        - The command ipconfig /all displays additional information including the MAC address, IP addresses of the default gateway, and the DNS servers. It also indicates if DHCP is enabled, the DHCP server address, and lease information
        - How can this utility assist in the troubleshooting process? Without an appropriate IP configuration, a host cannot participate in communications on a network. If the host does not know the location of the DNS servers, it cannot translate names into IP addresses
    - ipconfig /release and ipconfig /renew
        - If IP addressing information is assigned dynamically, the command ipconfig /release will release the current DHCP bindings. ipconfig /renew will request fresh configuration information from the DHCP server. A host may contain faulty or outdated IP configuration information and a simple renewal of this information is all that is required to regain connectivity
        - If, after releasing the IP configuration, the host is unable to obtain fresh information from the DHCP server, it could be that there is no network connectivity. Verify that the NIC has an illuminated link light, indicating that it has a physical connection to the network. If this does not solve the problem, it may be an issue with the DHCP server or network connections to the DCHP server.

## 17.1.3 Packet Tracer - Use the ipconfig Command
- In this activity, you will use the ipconfig command to identify incorrect configuration on a PC

## 17.1.4 The ping Command
- Probably the most commonly used network utility is ping. Most IP enabled devices support some form of the ping command in order to test whether or not network devices are reachable through the IP network
- If the IP configuration appears to be correctly configured on the local host, next, test network connectivity by using ping. The ping command can be followed by either an IP address or the name of a destination host. In the example, the user pings the default gateway at 10.10.10.1 and then pings ww​w.cisco.com
- When a ping is sent to an IP address, a packet known as an echo request is sent across the network to the IP address specified. If the destination host receives the echo request, it responds with a packet known as an echo reply. If the source receives the echo reply, connectivity is verified by the reply from the specific IP address. The ping is not successful if a message such as request timed out or general failure appears
- If a ping command is sent to a name, such as ww​w.cisco.com, a packet is first sent to a DNS server to resolve the name to an IP address. After the IP address is obtained, the echo request is forwarded to the IP address and the process proceeds. If a ping to the IP address succeeds, but a ping to the name does not, there is most likely a problem with DNS.

## 17.1.5 Ping Results
- If ping commands to both the name and IP address are successful, but the user is still unable to access the application, then the problem most likely resides in the application on the destination host. For example, it may be that the requested service is not running
- If neither ping is successful, then network connectivity along the path to the destination is most likely the problem. If this occurs, it is common practice to ping the default gateway. If the ping to the default gateway is successful, the problem is not local. If the ping to the default gateway fails, the problem resides on the local network
- In some cases, the ping may fail but network connectivity is not the problem. A ping may fail due to the firewall on the sending or receiving device, or a router along the path that is blocking the pings
- The basic ping command usually issues four echoes and waits for the replies to each one. It can, however, be modified to increase its usefulness. The options listed in the figure display additional features available

## 17.1.6 Packet Tracer - Use the ping Command
- In this activity, you will use the ping command to identify an incorrect configuration on a PC

## 17.2.1 What Did I Learn in this Module?
- Troubleshooting Commands
- A number of software utility programs are available that can help identify network problems. Most of these utilities are provided by the operating system as CLI commands
- Some of the available utilities include:
    - ipconfig - Displays IP configuration information
    - ping - Tests connections to other IP hosts
    - netstat - Displays network connections
    - tracert - Displays the route taken to the destination
    - nslookup - Directly queries the name server for information on a destination domain
- The ipconfig command is used to display the current IP configuration information for a host. Issuing this command from the command prompt will display the basic configuration information including IP address, subnet mask, and default gateway
- The command ipconfig /all displays additional information including the MAC address, IP addresses of the default gateway, and the DNS servers. It also indicates if DHCP is enabled, the DHCP server address, and lease information
- If IP addressing information is assigned dynamically, the command ipconfig /release will release the current DHCP bindings. ipconfig /renew will request fresh configuration information from the DHCP server. A host may contain faulty or outdated IP configuration information and a simple renewal of this information is all that is required to regain connectivity
- Probably the most commonly used network utility is ping. Most IP enabled devices support some form of the ping command in order to test whether or not network devices are reachable through the IP network. When a ping is sent to an IP address, a packet known as an echo request is sent across the network to the IP address specified. If the destination host receives the echo request, it responds with a packet known as an echo reply. If the source receives the echo reply, connectivity is verified by the reply from the specific IP address

## 17.2.2 Webster - Reflection Questions
- Congratulations! You’ve made it all the way through this course! Way back in the first module of this course, I mentioned that I can troubleshoot and fix my web. In fact, I can even make it stronger and more secure. Being able to do that is very satisfying. You have learned about the many commands that you can use to troubleshoot and fix your own network. You can use these commands to investigate your network, even if it is performing as it should. Which command(s) would you start with?

## 17.2.3 Network Testing Utilities Quiz
