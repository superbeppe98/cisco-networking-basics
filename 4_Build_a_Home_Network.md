[Back to Syllabus](./README.md#course-syllabus)

## 4.0.1 Webster - Why Should I Take this Module?

- Kishori and Shridhar are washing the dishes after dinner. Kishori is watching a favorite movie on her tablet while putting the dishes away. She asks Shridhar if her tablet works exactly as her mobile phone does. He explains that there are some tablets that do use a mobile network, but that her tablet is works on Wi-Fi network in her house. She tells him that she knows it must come in from that box in the corner of the living room. That is all she knows!

- Shridhar explains that the box in the corner is a home router. The router is connected to the internet. Home routers typically have two primary types of ports: ethernet ports and internet ports. In addition to the wired ports, many home routers include a radio antenna and a built-in wireless access point. Kishori mostly uses wireless at home. Now Shridhar is worried about his mother’s wireless security. Since she did not know what the router was, she probably did not change her default password on the router! Shridhar logs into the router and makes some changes to keep Kishori’s network and devices safer.

- Have you ever set up a router? Have you thought about having secure communications over wireless devices? This module will give you the knowledge to build a home network and configure wireless devices for secure communication

## 4.0.2 What Will I Learn in this Module?

- Module Title: Build a Home Network
- Module Objective: Configure an integrated wireless router and wireless client to connect securely to the internet

## 4.1.1 Video - Typical Home Network Setup

## 4.1.2 Components of a Home Network

- In addition to an integrated router, there are many different types of devices that might be connecting to a home network, as shown in the figure. Here are a few examples:
    - Desktop computers
    - Gaming systems
    - Smart TV systems
    - Printers
    - Scanners
    - Security cameras
    - Telephones
    - Climate control devices
- As the new technologies come on the market, more and more household functions will rely on the network to provide connectivity and control

## 4.1.3 Typical Home Network Routers

- Ethernet Ports
    - These ports connect to the internal switch portion of the router. These ports are usually labeled “Ethernet” or “LAN”, as shown in the figure. All devices connected to the switch ports are on the same local network

- Internet Port
    - This port is used to connect the device to another network. The internet port connects the router to a different network than the Ethernet ports. This port is often used to connect to the cable or DSL modem in order to access the internet

- In addition to the wired ports, many home routers include a radio antenna and a built-in wireless access point. By default, the wireless devices are on the same local network as the devices that are physically plugged into the LAN switch ports. The internet port is the only port that is on a different network in the default configuration

## 4.1.4 Check Your Understanding - Home Network Basics

## 4.2.1 LAN Wireless Frequencies

- The wireless technologies most frequently used in home networks are in the unlicensed 2.4 GHz and 5 GHz frequency ranges

- Bluetooth is a technology that makes use of the 2.4 GHz band. It is limited to low-speed, short-range communications, but has the advantage of communicating with many devices at the same time. This one-to-many communication has made Bluetooth technology the preferred method for connecting computer peripherals such as wireless mice, keyboards and printers. Bluetooth is a good method for transmitting audio to speakers or headphones

- Other technologies that use the 2.4 GHz and 5 GHz bands are the modern wireless LAN technologies that conform to the various IEEE 802.11 standards. Unlike Bluetooth technology, 802.11 devices transmit at a much higher power level giving them a great range and improved throughput. Certain areas of the electromagnetic spectrum can be used without a permit

- The figure shows where wireless technologies exist on the electromagnetic spectrum

## 4.2.2 Wired Network Technologies

- The most commonly implemented wired protocol is the Ethernet protocol. Ethernet uses a suite of protocols that allow network devices to communicate over a wired LAN connection. An Ethernet LAN can connect devices using many different types of wiring media
- Directly connected devices use an Ethernet patch cable, usually unshielded twisted pair. These cables can be purchased with the RJ-45 connectors already installed, and they come in various lengths. Recently constructed homes may have Ethernet jacks already wired in the walls of the home. For those homes that do not have UTP wiring, there are other technologies, such as powerline, that can distribute wired connectivity throughout the premises

- Category 5e Cable
    - Category 5e is the most common wiring used in a LAN. The cable is made up of 4 pairs of wires that are twisted to reduce electrical interference

- Coaxial Cable
    - Coaxial cable has an inner wire surrounded by a tubular insulating layer, that is then surrounded by a tubular conducting shield. Most coax cables also have an external insulating sheath or jacket

- Fiber-Optic Cable
    - Fiber-optic cables can be either glass or plastic with a diameter about the same as a human hair and it can carry digital information at very high speeds over long distances. Fiber-optic cables have a very high bandwidth, which enables them to carry very large amounts of data

## 4.2.3 Check Your Understanding - Network Technologies in the Home

## 4.3.1 Wi-Fi Networks

- A number of standards have been developed to ensure that wireless devices can communicate. They specify the RF spectrum used, data rates, how the information is transmitted, and more. The main organization responsible for the creation of wireless technical standards is the Institute of Electrical and Electronics Engineers (IEEE)
- The IEEE 802.11 standard governs the WLAN environment. There are amendments to the IEEE 802.11 standard that describe characteristics for different standards of wireless communications. Wireless standards for LANs use the 2.4 GHz and 5 GHz frequency bands. Collectively these technologies are referred to as Wi-Fi
- Another organization, known as the Wi-Fi Alliance, is responsible for testing wireless LAN devices from different manufacturers. The Wi-Fi logo on a device means that this equipment meets standards and should operate with other devices that use the same standard
- Wireless standards are constantly improving the connectivity and speed of Wi-Fi networks. It is important to be aware of new standards as they are introduced because manufacturers of wireless devices will implement these standards quickly in their new products
- Do you have a wireless network in your home? Do you know what standards are supported by your wireless router?

## 4.3.2 Wireless Settings

- Network mode
    - Determines the type of technology that must be supported. For example,802.11b,802.11g,802.11n or Mixed Mode.

- Network Name (SSID)
  - Used to identify the WLAN. All devices that wish to participate in the WLAN must have the same SSID.

- Standard Channel
    - Specifies the channel over which communication will occur. By default, this is set to Auto to allow the access point (AP) to determine the optimum channel to use.

- SSID Broadcast
    - Determines if the SSID will be broadcast to all devices within range. By default, set to Enabled
    - Note: SSID stands for Service Set Identifier

- The 802.11 protocol can provide increased throughput based on the wireless network environment. If all wireless devices connect with the same 802.11 standard, maximum speeds can be obtained for that standard. If the access point is configured to accept only one 802.11 standard, devices that do not use that standard cannot connect to the access point

- A mixed mode wireless network environment can include devices that use any of the existing Wi-Fi standards. This environment provides easy access for older devices that need a wireless connection but do not support the latest standards
When building a wireless network, it is important that the wireless components connect to the appropriate WLAN. This is done using the SSID

- The SSID is a case-sensitive, alphanumeric string that contains up to 32 characters. It is sent in the header of all frames transmitted over the WLAN. The SSID is used to tell wireless devices, called wireless stations (STAs), which WLAN they belong to and with which other devices they can communicate

- We use the SSID to identify a specific wireless network. It is essentially the name of the network. Wireless routers usually broadcast their configured SSIDs by default. The SSID broadcast allows other devices and wireless clients to automatically discover the name of the wireless network. When the SSID broadcast is disabled, you must manually enter the SSID on wireless devices
Disabling SSID broadcasting can make it more difficult for legitimate clients to find the wireless network. However, simply turning off the SSID broadcast is not sufficient to prevent unauthorized clients from connecting to the wireless network. All wireless networks should use the strongest available encryption to restrict unauthorized access

## 4.3.3 Check Your Understanding - Wireless Standards

## 4.4.1 First Time Setup

- Many wireless routers designed for home use have an automatic setup utility that can be used to configure the basic settings on the router. These utilities usually require a PC or laptop to be connected to a wired port on the router. If no device is available that has a wired connection, it may be necessary to configure the wireless client software on the laptop or tablet first

- To connect to the router using a wired connection, plug an Ethernet patch cable into the network port on the computer. Plug the other end into a LAN port on the router. Do not plug the cable into the port or interface that is labeled “Internet”. The internet port will connect to the DSL or cable modem. Some home routers may have a built-in modem for internet connections. If this is the case, verify that the type of connection is correct for your internet service. A cable modem connection will have a coaxial terminal to accept a BNC-type connector. A DSL connection will have a port for a telephone-type cable, usually an RJ-11 connector

- After confirming that the computer is connected to the network router and the link lights on the NIC indicate a working connection, the computer needs an IP address. Most network routers are set up so that the computer receives an IP address automatically from a local DHCP server automatically configured on the wireless router. If the computer does not have an IP address, check the router documentation and configure the PC or tablet with a unique IP address, subnet mask, default gateway, and DNS information

## 4.4.2 Design Considerations

- Before entering the configuration utility, or manually configuring the router through a web browser, you should consider how your network will be used. You do not want to configure the router and have that configuration limit what you are able to do on the network, nor do you want to leave your network unprotected

- What should my network be called?
    - If SSID broadcasting is on, the SSID name will be seen by all wireless clients within your signal range. Many times the SSID gives away too much information about the network to unknown client devices. It is not a good practice to include the device model or brand name as part of the SSID. Wireless devices have default settings that are easy to find on the internet, as well as known security weaknesses

- What types of devices will attach to my network?
    - Wireless devices contain radio transmitter/receivers that function within a specific frequency range. If a device only has the necessary radio for 802.11 b/g, it will not connect if the wireless router or access point is configured to only accept 802.11n or 802.11ac standards. If all devices support the same standard, the network will work at its optimum speed. If you have devices that do not support the n or ac standards, then you will have to enable legacy mode. A legacy mode wireless network environment varies between router models but can include a combination of 802.11a, 802.11b, 802.11g, 802.11n, and 802.11ac. This environment provides easy access for legacy devices that need a wireless connection

- How do I add new devices?
    - The decision regarding who can access your home network should be determined by how you plan to use the network. On some wireless routers, it is possible to set up guest access. This is a special SSID coverage area that allows open access but restricts that access to using the internet only
- The figure shows a wireless setup screen.
- Note: Some wireless routers may label legacy mode as mixed mode

## 4.4.3 Video - Wireless Router and Client Configuration

## 4.4.4 Packet Tracer - Configure a Wireless Router and Client

- In this Packet Tracer activity, you will complete the following objectives

- Part 1: Connect the Devices
- Part 2: Configure the Wireless Router
- Part 3: Configure IP Addressing and Test Connectivity

## 4.5.1 What Did I Learn in this Module?

- Home Network Basics
    - Most home networks consist of at least two separate networks. The public network coming in from the service provider. The router is connected to the internet. Most likely, the home router is equipped with both wired and wireless capabilities. A home network is a small LAN with devices that usually connect to an integrated router and to each other in order to exchange information
    - Wireless technology is fairly easy and inexpensive to install. Advantages of wireless LAN technology include mobility, scalability, flexibility, cost savings, reduced installation time, and reliability in harsh environments
    - In addition to an integrated router, there are many different types of devices that might be connecting to a home network, Examples include desktop computers, gaming systems, smart tv systems, printers, scanners, security cameras, and climate control devices
    - Small business and home routers typically have two primary types of ports: ethernet ports and internet ports. In addition to the wired ports, many home routers include a radio antenna and a built-in wireless access point

- Network Technologies in the Home
    - Wireless technologies use electromagnetic waves to carry information between devices. The electromagnetic spectrum includes such things as radio and television broadcast bands, visible light, x-rays, and gamma-rays. Some types of electromagnetic waves are not suitable for carrying data. Other parts of the spectrum are regulated by governments and licensed to various organizations for specific applications
    - Certain unlicensed sections of the spectrum are incorporated into consumer products, including the Wi-Fi routers found in most homes. The wireless technologies most frequently used in home networks are in the unlicensed 2.4 GHz and 5 GHz frequency ranges. Bluetooth is a technology that makes use of the 2.4 GHz band. Other technologies that use the 2.4 GHz and 5 GHz bands are the modern wireless LAN technologies that conform to the various IEEE 802.11 standards. Unlike Bluetooth technology, 802.11 devices transmit at a much higher power level giving them a great range and improved throughput

- Although many home network devices support wireless communications, there are still a few applications where devices benefit from a wired switch connection. The most commonly implemented wired protocol is the Ethernet protocol. Directly connected devices use an Ethernet patch cable, usually unshielded twisted pair. Category 5e is the most common wiring used in a LAN. The cable is made up of 4 pairs of wires that are twisted to reduce electrical interference. For those homes that do not have UTP wiring, there are other technologies, such as powerline, that can distribute wired connectivity throughout the premises

- Wireless standards
    - The IEEE 802.11 standard governs the WLAN environment. Wireless standards for LANs use the 2.4 GHz and 5 GHz frequency bands. Collectively these technologies are referred to as Wi-Fi. The Wi-Fi Alliance is responsible for testing wireless LAN devices from different manufacturers

- Wireless routers using the 802.11 standards have multiple settings that have to be configured. These settings include the following:

    - Network mode - Determines the type of technology that must be supported. For example, 802.11b, 802.11g, 802.11n or Mixed Mode
    - Network Name (SSID) - Used to identify the WLAN. All devices that wish to participate in the WLAN must have the same SSID
    - Standard Channel - Specifies the channel over which communication will occur. By default, this is set to Auto to allow the access point (AP) to determine the optimum channel to use
    - SSID Broadcast - Determines if the SSID will be broadcast to all devices within range. By default, set to Enabled
    - The 802.11 protocol can provide increased throughput based on the wireless network environment. If all wireless devices connect with the same 802.11 standard, maximum speeds can be obtained for that standard. If the access point is configured to accept only one 802.11 standard, devices that do not use that standard cannot connect to the access point. A mixed mode wireless network environment can include devices that use any of the existing Wi-Fi standards

- When building a wireless network, it is important that the wireless components connect to the appropriate WLAN. This is done using the SSID. The SSID is used to tell wireless devices, called STAs, which WLAN they belong to and with which other devices they can communicate. The SSID broadcast allows other devices and wireless clients to automatically discover the name of the wireless network. When the SSID broadcast is disabled, you must manually enter the SSID on wireless devices

- Set up a Home Router
- Many wireless routers designed for home use have an automatic setup utility that can be used to configure the basic settings on the router. To connect to the router using a wired connection, plug an Ethernet patch cable into the network port on the computer. Plug the other end into a LAN port on the router

- After the computer is connected to the network router and the link lights on the NIC indicate a working connection, the computer needs an IP address. Most network routers are set up so that the computer receives an IP address automatically from a local DHCP server automatically configured on the wireless router

- Before entering the configuration utility, or manually configuring the router through a web browser, you should consider how your network will be used. Consider what you will call your network and what devices should connect to your network. It is not a good practice to include the device model or brand name as part of the SSID since internet searches can expose security weaknesses

- The decision regarding who can access your home network should be determined by how you plan to use the network. Many routers support MAC address filtering. This enables you to specifically identify who is allowed on the wireless network. This makes the wireless network more secure, but it also less flexible when connecting new devices. On some wireless routers, it is possible to set up guest access. This is a special SSID coverage area that allows open access but restricts that access to using the internet only

## 4.5.2 Webster - Reflection Questions

- I had such a good time taking this module at the beach, that I think I’m going to set up a wireless network at home. That way, I can keep up with this course anywhere in my home. Building your home network to be a wireless network just makes sense. I can work in the west side of my web and catch the sun setting, then move back to the east side in the morning. It’s so much nicer than being stuck at my desk all day! Have you set up your own home network? If not, could you do it if you had to?

## 4.5.3 Build a Home Network Quiz

[Go to Next Module](./5_Communication_Principles.md)

