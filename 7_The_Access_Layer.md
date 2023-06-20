[Back to Syllabus](./README.md#course-syllabus)


7.0.1 Webster - Why Should I Take this Module?
During a lunch break, Kishori sees her friend, Rina, and they decide to eat together. Rina works as an IT support technician at the hospital. Kishori thinks this might be a good opportunity to ask Rina a question she’s been pondering. Kishori now knows that her desktop computer in the nurses’ station connects to the network using a twisted-pair cable. Most other devices she uses connect to the network wirelessly. She wonders if there is any difference in the way wired and wireless devices communicate on the network. Rina knows that Kishori has relatives in the United States. She explains that the differences between wired and wireless network communication is similar to the differences in addressing formats used for mailing packages to different countries. The contents inside might be exactly the same, but the addressing and possibly packaging could be very different.

How does a message get delivered? When you write a letter and place it in the envelope, you need to make sure it has the correct address information to be delivered to the recipient. In your network, the process of placing one message format (the letter) inside another message format (the envelope) is called encapsulation. Ready to learn more? Take this module!


7.0.2 What Will I Learn in this Module?
Module Title: The Access Layer

Module Objective: Explain how communication occurs on Ethernet networks.


7.1.1 Video - The Fields of the Ethernet Frame
This is a media player component. Select the play / pause button to watch or listen.
Ethernet is technology commonly used in local area networks. Devices access the Ethernet LAN using an Ethernet Network Interface Card (NIC). Each Ethernet NIC has a unique address permanently embedded on the card known as a Media Access Control (MAC) address. The MAC address for both the source and destination are fields in an Ethernet frame.

Press the Play button to watch the video.


7.1.2 Encapsulation
List of expandable sections. Select each button to expand the content.
When sending a letter, the letter writer uses an accepted format to ensure that the letter is delivered and understood by the recipient. In the same way, a message that is sent over a computer network follows specific format rules in order for it to be delivered and processed.

The process of placing one message format (the letter) inside another message format (the envelope) is called encapsulation. De-encapsulation occurs when the process is reversed by the recipient and the letter is removed from the envelope. Just as a letter is encapsulated in an envelope for delivery, so computer messages are encapsulated.

Each computer message is encapsulated in a specific format, called a frame, before it is sent over the network. A frame acts like an envelope; it provides the address of the intended destination and the address of the source host. The format and contents of a frame are determined by the type of message being sent and the channel over which it is communicated. Messages that are not correctly formatted are not successfully delivered to or processed by the destination host.

Click each button for an analogy and a network example of message formatting and encapsulation.

analogy:A common example of requiring the correct format in human communications is when sending a letter. Click Play in the figure to view an animation of formatting and encapsulating a letter.

An envelope has the address of the sender and receiver, each located at the proper place on the envelope. If the destination address and formatting are not correct, the letter is not delivered.

The process of placing one message format (the letter) inside another message format (the envelope) is called encapsulation. De-encapsulation occurs when the process is reversed by the recipient and the letter is removed from the envelope.



network:Similar to sending a letter, a message that is sent over a computer network follows specific format rules for it to be delivered and processed.

Internet Protocol (IP) is a protocol with a similar function to the envelope example. In the figure, the fields of the Internet Protocol version 6 (IPv6) packet identify the source of the packet and its destination. IP is responsible for sending a message from the message source to destination over one or more networks.

Note: The fields of the IPv6 packet are discussed in detail in another module.


7.1.3 Check Your Understanding - Encapsulation and the Ethernet Frame
Check your understanding of encapsulation and the Ethernet frame by choosing the correct answer to the following questions.


7.2.1 Video - Ethernet Switches
This is a media player component. Select the play / pause button to watch or listen.
Press the Play button to watch the video.

7.2.2 Video - MAC Address Tables
This is a media player component. Select the play / pause button to watch or listen.
Press the Play button to watch the video.


7.2.3 Check Your Understanding - The Access Layer
Check your understanding of the access layer by choosing the correct answer to the following questions.

7.3.1 What Did I Learn in this Module?

encapslation and the ethernet frame:The process of placing one message format inside another message format is called encapsulation. De-encapsulation occurs when the process is reversed by the recipient and the letter is removed from the envelope. Just as a letter is encapsulated in an envelope for delivery, so computer messages are encapsulated. A message that is sent over a computer network follows specific format rules for it to be delivered and processed.

The Ethernet protocol standards define many aspects of network communication including frame format, frame size, timing, and encoding. The format for Ethernet frames specifies the location of the destination and source MAC addresses, and additional information including preamble for sequencing and timing, start of frame delimiter, length and type of frame, and frame check sequence to detect transmission errors.


the access layer:The access layer is the part of the network in which people gain access to other hosts and to shared files and printers. The access layer provides the first line of networking devices that connect hosts to the wired Ethernet network. Within an Ethernet network, each host can connect directly to an access layer networking device using an Ethernet cable. Ethernet hubs contain multiple ports that are used to connect hosts to the network. Only one message can be sent through an Ethernet hub at a time. Two or more messages sent at the same time will cause a collision. Because excessive retransmissions can clog up the network and slow down network traffic, hubs are now considered obsolete and have been replaced by Ethernet switches.

An Ethernet switch is a device that is used at Layer 2. When a host sends a message to another host connected to the same switched network, the switch accepts and decodes the frames to read the MAC address portion of the message. A table on the switch, called a MAC address table, contains a list of all the active ports and the host MAC addresses that are attached to them. When a message is sent between hosts, the switch checks to see if the destination MAC address is in the table. If it is, the switch builds a temporary connection, called a circuit, between the source and destination ports. Ethernet switches also allow for sending and receiving frames over the same Ethernet cable simultaneously. This improves the performance of the network by eliminating collisions.

A switch builds the MAC address table by examining the source MAC address of each frame that is sent between hosts. When a new host sends a message or responds to a flooded message, the switch immediately learns its MAC address and the port to which it is connected. The table is dynamically updated each time a new source MAC address is read by the switch.


7.3.2 Webster - Reflection Questions
There is a lot going on behind the scenes when I send an email to a friend. Way more than I knew about! Data gets encapsulated when I send an email and then it's de-encapsulated when my friend opens that email. The access layer of the OSI model is where all of this happens. Now that you know about encapsulation and the access layer, what else do you do on your computer, tablet, or smartphone that requires encapsulation and the protocols used at the access layer?


7.3.3 The Access Layer Quiz










[Go to Next Module](./)

