[Back to Syllabus](./README.md#course-syllabus)

## 2.0.1 Webster - Why Should I Take this Module?

- Kishori does not yet understand network infrastructure device roles in the network, including end devices, intermediate devices, and network media. When she first started her nursing career, she was writing patient medical notes in a paper notebook! At home, Kishori only has a laptop, a smartphone, and a tablet. This makes her most familiar with end devices, or hosts. She understands that those devices are connected to the internet somehow through that box in the corner of her living room. At work she uses a laptop, a desktop, a printer, and other network-connected hospital equipment. She wants to learn more about network components and how they all connect
- Kishori leaves her patient's room, sets down her laptop, and continues her work on the desktop computer at the nursing station. She wonders how the electronic notes she just took on the laptop appear on the patient’s record on the desktop computer. How are they connected? How does the computer reach the internet in the first place? Kishori has a lot to learn, and you might too!

## 2.0.2 What Will I Learn in this Module?

- Module Title: Network Components, Types, and Connections
- Module Objective: Explain network types, components, and connections

## 2.1.1 Video - Clients and Servers

## 2.1.2 Client and Server Roles

- All computers connected to a network that participate directly in network communication are classified as hosts. Hosts can send and receive messages on the network. In modern networks, computer hosts can act as a client, a server, or both, as shown in the figure. The software installed on the computer determines which role the computer plays
- Servers are hosts that have software installed which enable them to provide information, like email or web pages, to other hosts on the network. Each service requires separate server software. For example, a host requires web server software in order to provide web services to the network. Every destination that you visit online is provided to you by a server located somewhere on a network that is connected to the global internet
- Clients are computer hosts that have software installed that enables the hosts to request and display the information obtained from the server. An example of client software is a web browser, such as Internet Explorer, Safari, Mozilla Firefox, or Chrome

## 2.1.3 Peer-to-Peer Networks

- Client and server software usually run on separate computers, but it is also possible for one computer to run both client and server software at the same time. In small businesses and homes, many computers function as the servers and clients on the network. This type of network is called a peer-to-peer (P2P) network
- The simplest P2P network consists of two directly connected computers using either a wired or wireless connection. Both computers are then able to use this simple network to exchange data and services with each other, acting as either a client or a server as necessary
- Multiple PCs can also be connected to create a larger P2P network, but this requires a network device, such as a switch, to interconnect the computers
- The main disadvantage of a P2P environment is that the performance of a host can be slowed down if it is acting as both a client and a server at the same time. The figure lists some of the advantages and disadvantages of peer-to-peer networks
- In larger businesses, because of the potential for high amounts of network traffic, it is often necessary to have dedicated servers to support the number of service requests
- The advantages and disadvantages of P2P networking are summarized in the figure

- The advantages of peer-to-peer networking:
    - Easy to set up
    - Less complex
    - Lower cost because network devices and dedicated servers may not be required
    - Can be used for simple tasks such as transferring files and sharing printers

- The disadvantages of peer-to-peer networking:
    - No centralized administration
    - Not as secure
    - Not scalable
    - All devices may act as both clients and servers which can slow their performance

## 2.1.4 Peer-to-Peer Applications

- A P2P application allows a device to act as both a client and a server within the same communication, as shown in the figure. In this model, every client is a server and every server is a client. P2P applications require that each end device provide a user interface and run a background service
- Some P2P applications use a hybrid system where resource sharing is decentralized, but the indexes that point to resource locations are stored in a centralized directory. In a hybrid system, each peer accesses an index server to get the location of a resource stored on another peer.
Both clients can simultaneously send and receive messages

## 2.1.5 Multiple Roles in the Network

- A computer with server software can provide services simultaneously to one or many clients, as shown in the figure
- Additionally, a single computer can run multiple types of server software. In a home or small business, it may be necessary for one computer to act as a file server, a web server, and an email server
- A single computer can also run multiple types of client software. There must be client software for every service required. With multiple clients installed, a host can connect to multiple servers at the same time. For example, a user can check email and view a web page while instant messaging and listening to internet radio

## 2.1.6 Check Your Understanding - Clients and Servers

## 2.2.2 Network Infrastructure

- The path that a message takes from its source to destination can be as simple as a single cable connecting one computer to another, or as complex as a network that literally spans the globe. This network infrastructure is the platform that supports the network. It provides the stable and reliable channel over which our communications can occur

- The network infrastructure contains three categories of hardware components, as shown in the figure:
    - End devices
    - Intermediate devices
    - Network media

- Devices and media are the physical elements, or hardware, of the network. Hardware is often the visible components of the network platform such as a laptop, PC, switch, router, wireless access point, or the cabling used to connect the devices. Occasionally, some components may not be so visible. In the case of wireless media, messages are transmitted through the air using invisible radio frequencies or infrared waves
- Make a list of the network infrastructure components installed in your home network. Include the cables or wireless access points that provide your network connections

## 2.2.3 End Devices

- The network devices that people are most familiar with are called end devices, or hosts. These devices form the interface between users and the underlying communication network

- Some examples of end devices are as follows:
    - Computers (workstations, laptops, file servers, web servers)
    - Network printers
    - Telephones and teleconferencing equipment
    - Security cameras
    - Mobile devices (such as smart phones, tablets, PDAs, and wireless debit/credit card readers and barcode scanners)
    - An end device (or host) is either the source or destination of a message transmitted over the network, as shown in the animation. In order to uniquely identify hosts, addresses are used. When a host initiates communication, it uses the address of the destination host to specify where the message should be sent

- Click Play in the figure to see an animation of data flowing through a network.

## 2.2.4 Check Your Understanding - Network Components

## 2.3.1 ISP Services

- An Internet Service Provider (ISP) provides the link between the home network and the internet. An ISP can be the local cable provider, a landline telephone service provider, the cellular network that provides your smartphone service, or an independent provider who leases bandwidth on the physical network infrastructure of another company
- Many ISPs also offer additional services to their contract subscribers, as shown in the figure. These services can include email accounts, network storage, and website hosting and automated backup or security services
- ISPs are critical to communications across the global internet. Each ISP connects to other ISPs to form a network of links that interconnect users all over the world. ISPs are connected in a hierarchical manner that ensures that internet traffic generally takes the shortest path from the source to the destination
- The internet backbone is like an information super highway that provides high-speed data links to connect the various service provider networks in major metropolitan areas around the world. The primary medium that connects the internet backbone is fiber-optic cable. This cable is typically installed underground to connect cities within continents. Fiber-optic cables also run under the sea to connect continents, countries, and cities

## 2.3.2 ISP Connections
- The interconnection of ISPs that forms the backbone of the internet is a complex web of fiber-optic cables with expensive networking switches and routers that direct the flow of information between source and destination hosts. Average home users are not aware of the infrastructure outside of their network. For a home user, connecting to the ISP is a fairly uncomplicated process
- The top portion of the figure displays the simplest ISP connection option. It consists of a modem that provides a direct connection between a computer and the ISP. This option should not be used though, because your computer is not protected on the internet
- As shown in the bottom portion of the figure, a router is required to securely connect a computer to an ISP. This is the most common connection option. It consists of using a wireless integrated router to connect to the ISP. The router includes a switch to connect wired hosts and a wireless AP to connect wireless hosts. The router also provides client IP addressing information and security for inside hosts

## 2.3.3 Cable and DSL Connections
- Most home network users do not connect to their service providers with fiber-optic cables. The figure illustrates common connection options for small office and home users. The two most common methods are as follows:
    - Cable - Typically offered by cable television service providers, the internet data signal is carried on the same coaxial cable that delivers cable television. It provides a high bandwidth, always on, connection to the internet. A special cable modem separates the internet data signal from the other signals carried on the cable and provides an Ethernet connection to a host computer or LAN
    - DSL - Digital Subscriber Line provides a high bandwidth, always on, connection to the internet. It requires a special high-speed modem that separates the DSL signal from the telephone signal and provides an Ethernet connection to a host computer or LAN. DSL runs over a telephone line, with the line split into three channels. One channel is used for voice telephone calls. This channel allows an individual to receive phone calls without disconnecting from the internet. A second channel is a faster download channel, used to receive information from the internet. The third channel is used for sending or uploading information. This channel is usually slightly slower than the download channel. The quality and speed of the DSL connection depends mainly on the quality of the phone line and the distance from the central office of your phone company The farther you are from the central office, the slower the connection

## 2.3.4 Additional Connectivity Options

- Other ISP connection options for home users include the following:
        - Cellular
            - Cellular internet access uses a cell phone network to connect. Wherever you can get a cellular signal, you can get cellular internet access. Performance will be limited by the capabilities of the phone and the cell tower to which it is connected. The availability of cellular internet access is a real benefit for people in areas that would otherwise have no internet connectivity at all, or for people who are constantly on the move. The downside of cellular connectivity is that the carrier usually meters the bandwidth usage of the connection and may charge extra for bandwidth that exceeds the contract data plan
        - Satellite
            - Satellite service is a good option for homes or offices that do not have access to DSL or cable. Satellite dishes (see figure) require a clear line of sight to the satellite and so might be difficult in heavily wooded areas or places with other overhead obstructions. Speeds will vary depending on the contract, though they are generally good. Equipment and installation costs can be high (although check the provider for special deals), with a moderate monthly fee thereafter. Like cellular access, the availability of satellite internet access is a real benefit in areas that would otherwise have no internet connectivity at all
        - Dial-up Telephone
            - An inexpensive option that uses any phone line and a modem. To connect to the ISP, a user calls the ISP access phone number. The low bandwidth provided by a dial-up modem connection is usually not sufficient for large data transfer, although it is useful for mobile access while traveling. A modem dial-up connection should only be considered when higher speed connection options are not available

- In metropolitan areas, many apartments and small offices are being connected directly with fiber-optic cables. This enables an internet service provider to provide higher bandwidth speeds and support more services such as internet, phone, and TV

- The choice of connection varies depending on geographical location and service provider availability.
- Satellite Connection

## 2.3.5 Check Your Understanding - ISP Connectivity Options

## 2.4.1 What Did I Learn in this Module?

- Clients and Servers
    - All computers connected to a network that participate directly in network communication are classified as hosts. Hosts can send and receive messages on the network. In modern networks, computer hosts can act as a client, a server, or both. The software installed on the computer determines which role the computer plays
    - Client and server software usually run on separate computers, but it is also possible for one computer to run both client and server software at the same time. In small businesses and homes, many computers function as the servers and clients on the network. This type of network is called a P2P network. In larger businesses, because of the potential for high amounts of network traffic, it is often necessary to have dedicated servers to support the number of service requests. P2P networks are easy to set up, less complex, lower in cost, and can be used for simple tasks such as transferring files and sharing printers. However, there is no centralized administration. They have less security, are not scalable, and can perform slower

- Network Components
    - There are symbols that represent various types of networking equipment. The network infrastructure is the platform that supports the network. It provides the stable and reliable channel over which our communications can occur. The network infrastructure contains three categories of hardware components: end devices, intermediate devices, and network media. Hardware is often the visible components of the network platform such as a laptop, PC, switch, router, wireless access point, or the cabling used to connect the devices. Components that are not visible include wireless media
    - End devices, or hosts, form the interface between users and the underlying communication network - Some examples of end devices include:
        - Computers (workstations, laptops, file servers, web servers)
        - Network printers
        - Telephones and teleconferencing equipment
        - Security cameras
        - Mobile devices (such as smartphones, tablets, PDAs, and wireless debit/credit card readers and barcode scanners)

- ISP Connectivity Options
    - An ISP provides the link between the home network and the internet. An ISP can be the local cable provider, a landline telephone service provider, the cellular network that provides your smartphone service, or an independent provider who leases bandwidth on the physical network infrastructure of another company. Each ISP connects to other ISPs to form a network of links that interconnect users all over the world. ISPs are connected in a hierarchical manner that ensures that internet traffic generally takes the shortest path from the source to the destination
    - The interconnection of ISPs that forms the backbone of the internet is a complex web of fiber-optic cables with expensive networking switches and routers that direct the flow of information between source and destination hosts
    - For a home user, connecting to the ISP is a fairly uncomplicated process. This is the most common connection option. It consists of using a wireless integrated router to connect to the ISP. The router includes a switch to connect wired hosts and a wireless AP to connect wireless hosts. The router also provides client IP addressing information and security for inside hosts. The two most common methods are cable and DSL. Other options include cellular, satellite, and dial-up telephone

## 2.4.2 Webster - Reflection Questions

Have you ever ordered a piece of furniture that you had to assemble yourself? The box has all the pieces and parts that you need along with the assembly instructions. It helps you to look at all these items while you read through the instructions. Think of your network. Did you know what all the different devices and connection types were before you took this module? Do you look at these pieces and parts differently now?

## 2.4.3 Network Components, Types, and Connections Quiz

[Go to Next Module](./3_Wireless_and_Mobile_Networks.mc)

