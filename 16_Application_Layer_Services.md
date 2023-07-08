[Back to Syllabus](./README.md#course-syllabus)

16.0.1 Webster - Why Should I Take this Module?
Kishori needs to get access to a patient file. She has done this many times, but it is only now that she is wondering how this process actually happens in a network. Where does this electronic document come from? How is she able to access the hospital’s intranet? How is she able to access the internet at all? All of this is possible because of application layer services.

Kishori has more to learn before she applies for that position that Rina mentioned. There are many services that work at the application layer including some you’re familiar with such as FTP, DHCP, and DNS. Just about any time you want to retrieve something that is not already located on your computer, you will be the client requesting that the appropriate server send you that item. And of course, by now you know that there will be protocols involved. Read on!

16.0.2 What Will I Learn in this Module?
Module Title: Application Layer Services

Module Objective: Explain the function of common application layer services.



16.1.1 Client and Server Interaction
Every day, we use the services available over networks and the internet to communicate with others and to perform routine tasks. We rarely think of the servers, clients, and networking devices that are necessary in order for us to receive an email, update our status on social media, or shop for the best bargains in an online store. Most of the commonly used internet applications rely on complicated interactions between various servers and clients.

The term server refers to a host running a software application that provides information or services to other hosts that are connected to the network. A well-known example of an application is a web server. There are millions of servers connected to the internet, providing services such as web sites, email, financial transactions, music downloads, etc. A crucial factor to enable these complex interactions to function is that they all use agreed upon standards and protocols.

An example of client software is a web browser, like Chrome or Firefox. A single computer can also run multiple types of client software. For example, a user can check email and view a web page while instant messaging and listening to an audio stream. The table lists three common types of server software.


16.1.2 Video - Web Server and Client IP Interactions


16.1.3 URI, URN, and URL
Web resources and web services such as RESTful APIs are identified using a Uniform Resource Identifier (URI). A URI is a string of characters that identifies a specific network resource. As shown in the figure, a URI has two specializations:

Uniform Resource Name (URN) - This identifies only the namespace of the resource (web page, document, image, etc.) without reference to the protocol.
Uniform Resource Locator (URL) - This defines the network location of a specific resource on the network. HTTP or HTTPS URLs are typically used with web browsers. Other protocols such as FTP, SFTP, SSH, and others can be used as a URL. A URL using SFTP might look like: sftp://sftp.example.com.
These are the parts of a URI, as shown in the figure:

Protocol/scheme - HTTPS or other protocols such as FTP, SFTP, mailto, and NNTP
Hostname - w​ww.example.com
Path and file name - /author/book.html
Fragment - #page155
Parts of a URI



16.1.4 Video - Web Traffic in Packet Tracer


16.1.5 Packet Tracer - The Client Interaction
In this activity, you will observe the client interaction between the server and PC.


16.2.1 Common Network Application Services
What are the most common internet services that you use on a regular basis? For most people, the list includes services such as internet searches, social media sites, video and audio streaming, on-line shopping sites, email, and messaging. Each of these services relies on protocols from the TCP/IP protocol suite to reliably communicate the information between the clients and the servers.

Some of the most common servers that provide these services are shown in the figure. A brief description of each service is shown in the table.


16.2.2 Check Your Understanding - Common Network Applications
Check your understanding of network application services by choosing the correct answer to the following questions.


16.3.1 Video - DNS Servers.




16.3.2 A Note About Syntax Checker Activities
When you are learning how to modify device configurations, you might want to start in a safe, non-production environment before trying it on real equipment. There are different simulation tools to help build your configuration and troubleshooting skills. Because these are simulation tools, they typically do not have all the functionality of real equipment. One such tool is the Syntax Checker. In each Syntax Checker, you are given a set of instructions to enter a specific set of commands. You cannot progress in Syntax Checker unless the exact and full command is entered as specified. More advanced simulation tools, such as Packet Tracer, let you enter abbreviated commands, much as you would do on real equipment.



16.3.3 Syntax Checker - The nslookup Command
When you manually configure a device for network connectivity, recall that you also include a DNS server address. For home networks, this configuration is typically handled by DHCP running on the home router. Your ISP provides the DNS server address to your home router, and then your home router uses DHCP to send the configuration to all the devices connected to its network. When you type the name for a website, such as www.cisco.com, the DNS client running on your device first asks the DNS server for the IP address, such as 172.230.155.162, before sending out your HTTP request.

You can use the command nslookup to discover the IP addresses for any domain name. In this Syntax Checker activity, practice entering the nslookup command in both Windows and Linux.




16.4.1 Video - HTTP and HTML


16.4.2 HTTP and HTML
When a web client receives the IP address of a web server, the client browser uses that IP address and port 80 to request web services. This request is sent to the server using the Hypertext Transfer Protocol (HTTP).

When the server receives a port 80 request, the server responds to the client request and sends the web page to the client. The information content of a web page is encoded using specialized 'mark-up' languages. The HyperText Markup Language (HTML) coding tells the browser how to format the web page and what graphics and fonts to use. HTML is the most commonly used language.

Click Play in the figure to view a client request for a web page.


The HTTP protocol is not a secure protocol; information could easily be intercepted by other users as data is sent over the network. In order to provide security for the data, HTTP can be used with secure transport protocols. Requests for secure HTTP are sent to port 443. These requests use https in the site address in the browser, rather than http.

There are many different web servers and web clients available. The HTTP protocol and HTML standards make it possible for these servers and clients from many different manufacturers to work together seamlessly.


16.4.3 Packet Tracer - Observe Web Requests
In this activity, you will observe web requests when a client browser requests web pages from a server.



16.5.1 File Transfer Protocol
In addition to web services, another common service used across the internet is one that allows users to transfer files.

The File Transfer Protocol (FTP) provides an easy method to transfer files from one computer to another. A host running FTP client software can access an FTP server to perform various file management functions including file uploads and downloads.

The FTP server enables a client to exchange files between devices. It also enables clients to manage files remotely by sending file management commands such as delete or rename. To accomplish this, the FTP service uses two different ports to communicate between client and server.

The example in the figure illustrates how FTP operates. To begin an FTP session, control connection requests are sent to the server using destination TCP port 21. When the session is opened, the server uses TCP port 20 to transfer the data files.

FTP client software is built into computer operating systems and into most web browsers. Stand-alone FTP clients offer many options in an easy-to-use GUI-based interface.


16.5.2 Video - FTP Client Software



16.5.3 Packet Tracer - Use FTP Services
In this activity, you will put a file on an FTP server and get a file from an FTP server.



16.6.1 Video - Remote Access with Telnet or SSH


16.6.2 Telnet
Long before desktop computers with sophisticated graphical interfaces existed, people used text-based systems which were often just display terminals physically attached to a central computer. After networks became available, people needed a way to remotely access the computer systems in the same manner that they did with the directly-attached terminals.

Telnet was developed to meet that need. Telnet dates back to the early 1970s and is among the oldest of the application layer protocols and services in the TCP/IP suite. Telnet provides a standard method of emulating text-based terminal devices over the data network. Both the protocol itself and the client software that implements the protocol are commonly referred to as Telnet. Telnet servers listen for client requests on TCP port 23.

Appropriately enough, a connection using Telnet is called a virtual terminal (vty) session, or connection. Rather than using a physical device to connect to the server, Telnet uses software to create a virtual device that provides the same features of a terminal session with access to the server’s command line interface (CLI).

In the figure, the client has remotely connected to the server via Telnet. The client is now able to execute commands as if it were locally connected to the server.

Note: Telnet is not considered to be a secure protocol. SSH should be used in most environments instead of Telnet. Telnet is used in several examples in this course for simplicity of configuration.



16.6.3 Security Issues with Telnet
After a Telnet connection is established, users can perform any authorized function on the server, just as if they were using a command line session on the server itself. If authorized, they can start and stop processes, configure the device, and even shut down the system.

Although the Telnet protocol can require a user to login, it does not support transporting encrypted data. All data exchanged during Telnet sessions is transported as plaintext across the network. This means that the data can be easily intercepted and understood.

The Secure Shell (SSH) protocol offers an alternate and secure method for server access. SSH provides the structure for secure remote login and other secure network services. It also provides stronger authentication than Telnet and supports transporting session data using encryption. As a best practice, network professionals should always use SSH in place of Telnet, whenever possible.

The figure illustrates how SSH is more secure than Telnet. Notice how the data captured by the hacker when Telnet is used is clearly readable while the data captured when SSH is used is encrypted and therefore more secure.



16.6.4 Packet Tracer - Use Telnet and SSH
In this activity, you will establish remote session to a router using Telnet and SSH.



16.7.1 Email Clients and Servers
Email is one of the most popular client/server applications on the internet. Email servers run server software that enables them to interact with clients and with other email servers over the network.

Each mail server receives and stores mail for users who have mailboxes configured on the mail server. Each user with a mailbox must then use an email client to access the mail server and read these messages. Many internet messaging systems use a web-based client to access email. Examples of this type of client include Microsoft 365, Yahoo, and Gmail.

Mailboxes are identified by the format: user@c​ompany.domain

Various application protocols used in processing email include SMTP, POP3, and IMAP4.



16.7.2 Email Protocols
Simple Mail Transfer Protocol (SMTP)

SMTP is used by an email client to send messages to its local email server. The local server then decides if the message is destined for a local mailbox or if the message is addressed to a mailbox on another server.

If the server has to send the message to a different server, SMTP is used between those two servers as well. SMTP requests are sent to port 25.

Click Play in the figure to see how SMTP is used to send email.


Post Office Protocol (POP3)

A server that supports POP clients receives and stores messages addressed to its users. When the client connects to the email server, the messages are downloaded to the client. By default, messages are not kept on the server after they have been accessed by the client. Clients contact POP3 servers on port 110.

Internet Message Access Protocol (IMAP4)

A server that supports IMAP clients also receives and stores messages addressed to its users. However, unlike POP, IMAP keeps the messages in the mailboxes on the server, unless they are deleted by the user. The most current version of IMAP is IMAP4 which listens for client requests on port 143.

Many different email servers exist for the various network operating system platforms.




16.7.3 Text Messaging
Text messaging, shown in the figure, is one of the most popular communication tools in use today. In addition, text messaging software is built into many online applications, smartphone apps, and social media sites.


Both clients can simultaneously send and receive messages.

Text messages may also be called instant messages, direct messages, private messages, and chat messages. Text messaging enables users to communicate or chat over the internet in real-time. Text messaging services on a computer are usually accessed through a web-based client that is integrated into a social media or information sharing site. These clients usually only connect to other users of the same site.

There are also a number of standalone text message clients such as Cisco Webex Teams, Microsoft Teams, WhatsApp, Facebook Messenger, and many others. These applications are available for a wide variety of operating systems and devices. A mobile version is typically offered. In addition to text messages, these clients support the transfer of documents, video, music, and audio files.



16.7.4 Internet Phone Calls
Making telephone calls over the internet is becoming increasingly popular. An internet telephony client uses peer-to-peer technology similar to that used by instant messaging, as shown in the figure. IP telephony makes use of Voice over IP (VoIP) technology, which converts analog voice signals into digital data. The voice data is encapsulated into IP packets which carry the phone call through the network.

When the IP phone software has been installed, the user selects a unique name. This is so that calls can be received from other users. Speakers and a microphone, built-in or separate, are required. A headset is frequently plugged into the computer to serve as a phone.

Calls are made to other users of the same service on the internet, by selecting the username from a list. A call to a regular telephone (landline or cell phone) requires using a gateway to access the Public Switched Telephone Network (PSTN). Depending on the service, there may be charges associated with this type of call. The protocols and destination ports used by internet telephony applications can vary based on the software.


16.7.5 Check Your Understanding - Email and Messaging
Check your understanding of email and messaging by choosing the correct answer to the following questions.


16.8.1 What Did I Learn in this Module?

The Client Server Relationship
The term server refers to a host running a software application that provides information or services to other hosts that are connected to the network, such as a web server. An example of client software is a web browser, like Chrome or Firefox. A single computer can also run multiple types of client software. A crucial factor to enable these complex interactions to function is that they all use agreed upon standards and protocols.

The key characteristic of client/server systems is that the client sends a request to a server, and the server responds by carrying out a function, such as sending the requested document back to the client. The combination of a web browser and a web server is perhaps the most commonly used instance of a client/server system.

A URI is a string of characters that identifies a specific network resource. The parts of a URI are protocol/scheme, hostname, path and file name, and fragment. A URI has two specializations:

URN - This identifies only the namespace of the resource without reference to the protocol.
URL - This defines the network location of a specific resource on the network. HTTP or HTTPS URLs are typically used with web browsers. Other protocols such as FTP, SFTP, SSH, and others can be used as a URL.

Network Application Services
For most people, the most common internet services that they use include internet searches, social media sites, video and audio streaming, on-line shopping sites, email, and messaging. Each of these services relies on protocols from the TCP/IP protocol suite to reliably communicate the information between the clients and the servers. Common services include: DNS, SSH, SMTP, POP, IMAP, DHCP, HTTP, and FTP.

Domain Name System
The DNS provides a way for hosts to request the IP address of a specific server. DNS names are registered and organized on the internet within specific high-level groups, or domains. Some of the most common high-level domains on the internet are .com, .edu, and .net.

When the DNS server receives the request from a host, it checks its table to determine the IP address associated with that web server. If the local DNS server does not have an entry for the requested name, it queries another DNS server within the domain. When the DNS server learns the IP address, that information is sent back to the host.

Web Clients and Servers
When a web client receives the IP address of a web server, the client browser uses that IP address and port 80 to request web services. This request is sent to the server using HTTP. The HTTP protocol is not a secure protocol; information could easily be intercepted by other users as data is sent over the network. To provide security for the data, HTTP can be used with secure transport protocols. Requests for secure HTTP are sent to port 443. These requests use https in the site address in the browser, rather than http.

When the server receives a port 80 request, the server responds to the client request and sends the web page to the client. The information content of a web page is encoded using HTML. HTML coding tells the browser how to format the web page and what graphics and fonts to use.

There are many different web servers and web clients. The HTTP protocol and HTML standards make it possible for these servers and clients from many different manufacturers to work together seamlessly.




FTP Clients and Servers

FTP provides an easy method to transfer files from one computer to another. A host running FTP client software can access an FTP server to perform various file management functions including file uploads and downloads. The FTP server enables a client to exchange files between devices. It also enables clients to manage files remotely by sending file management commands such as delete or rename. To accomplish this, the FTP service uses two different ports to communicate between client and server. To begin an FTP session, control connection requests are sent to the server using destination TCP port 21. When the session is opened, the server uses TCP port 20 to transfer the data files.

Most client operating systems such as Windows, Mac OS, and Linux include a command-line interface for FTP. There is also GUI-based FTP client software that provides a simple drag-and-drop interface for FTP.

Virtual Terminals

Telnet provides a standard method of emulating text-based terminal devices over the data network. Both the protocol itself and the client software that implements the protocol are commonly referred to as Telnet. Telnet servers listen for client requests on TCP port 23. A connection using Telnet is called a vty session, or connection. Rather than using a physical device to connect to the server, Telnet uses software to create a virtual device that provides the same features of a terminal session with access to the server’s CLI.

Telnet is not considered to be a secure protocol. Although the Telnet protocol can require a user to login, it does not support transporting encrypted data. All data exchanged during Telnet sessions is transported as plaintext across the network. This means that the data can be easily intercepted and understood.

SSH provides the structure for secure remote login and other secure network services. It also provides stronger authentication than Telnet and supports transporting session data using encryption. Network professionals should always use SSH in place of Telnet, whenever possible.

Email and Messaging

Each mail server receives and stores mail for users who have mailboxes configured on the mail server. Each user with a mailbox must then use an email client to access the mail server and read these messages. Many internet messaging systems use a web-based client to access email including Microsoft 365, Yahoo, and Gmail. Application protocols used in processing email include SMTP, POP3, and IMAP4.

SMTP is used by an email client to send messages to its local email server. The local server then decides if the message is destined for a local mailbox or if the message is addressed to a mailbox on another server. If the server must send the message to a different server, SMTP is used between those two servers. SMTP requests are sent to port 25. A server that supports POP clients receives and stores messages addressed to its users. When the client connects to the email server, the messages are downloaded to the client. By default, messages are not kept on the server after they have been accessed by the client. Clients contact POP3 servers on port 110.

A server that supports IMAP clients also receives and stores messages addressed to its users. However, unlike POP, IMAP keeps the messages in the mailboxes on the server, unless they are deleted by the user. The most current version of IMAP is IMAP4 which listens for client requests on port 143.

Text messages may be called instant messages, direct messages, private messages, and chat messages. Text messaging enables users to chat over the internet in real-time. Text messaging services on a computer are usually accessed through a web-based client that is integrated into a social media or information sharing site. These clients usually only connect to other users of the same site.

An internet telephony client uses peer-to-peer technology similar to that used by instant messaging. IP telephony uses VoIP, which converts analog voice signals into digital data. The voice data is encapsulated into IP packets which carry the phone call through the network.



16.8.2 Webster - Reflection Questions
As you now know, when you want to access a file or a website that is not located on your computer, your computer becomes the ‘client’ sending a request to a ‘server’. Maybe you are only looking at the file. What if you need to download a copy of it to your computer? Perhaps you are just visiting a website. All of this occurs at the application layer of the network. What else can you do online because of the protocols and services found in the application layer?



16.8.3 Application Layer Services Quiz
Incomplete Question 1Question 1
Multiple choice question
What two characteristics describe an FTP connection? (Choose two.)

[Go to Next Module](./17_Network_Testing_Utilities.md)
