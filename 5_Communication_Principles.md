[Back to Syllabus](./README.md#course-syllabus)

## 5.0.1 Webster - Why Should I Take this Module?

- The next day, Kishori has a new patient, Srinivas, who has just been admitted to a room. He is from Narayanpet and speaks Telugu. Kishori speaks Marathi. These two Indian languages are very different. Kishori and Srinivas do not speak each other's native language. However, they do both speak English. Therefore, they decide to communicate using English
- Before beginning to communicate with each other, we establish rules or agreements to govern the conversation. Just like Kishori and Srinivas, we decide what method of communication we should use, and what language we should use. We may also need to confirm that our messages are received. For example, Kishori may have Srinivas sign a document verifying that he has understood Kishori’s care instructions
- Networks also need rules, or protocols, to ensure successful communication. This module will cover the communication principles for networks

## 5.0.2 What Will I Learn in this Module?

- Module Title: Communication Principles
- Module Objective: Explain the importance of standards and protocols in network communications

## 5.1.1 Communication Protocols

- Communication in our daily lives takes many forms and occurs in many environments. We have different expectations depending on whether we are chatting via the internet or participating in a job interview. Each situation has its corresponding expected behaviors and styles
- Before beginning to communicate with each other, we establish rules or agreements to govern the conversation. These agreements include the following:
    - What method of communication should we use?
    - What language should we use?
    - Do we need to confirm that our messages are received?
- Click below for an example of determining the method, language, and confirmation strategies

- These rules, or protocols, must be followed in order for the message to be successfully delivered and understood. Among the protocols that govern successful human communication are these:
    - An identified sender and receiver
    - Agreed upon method of communicating (face-to-face, telephone, letter, photograph)
    - Common language and grammar
    - Speed and timing of delivery
    - Confirmation or acknowledgment requirements

- The techniques that are used in network communications share these fundamentals with human conversations
- Think about the commonly accepted protocols for sending text messages to your friends

## 5.1.2 Why Protocols Matter

- Just like humans, computers use rules, or protocols, in order to communicate. Protocols are required for computers to properly communicate across the network. In both a wired and wireless environment, a local network is defined as an area where all hosts must "speak the same language", which, in computer terms means they must "share a common protocol"
- If everyone in the same room spoke a different language, they would not be able to communicate. Likewise, if devices in a local network did not use the same protocols, they would not be able to communicate
- Networking protocols define many aspects of communication over the local network. As shown in the table, these include message format, message size, timing, encoding, encapsulation, and message patterns

![2023-06-13 21 03 15 skillsforall com c6a107092896](https://github.com/superbeppe98/cisco-networking-basics/assets/29455975/69b21878-d328-4ffc-8442-842eac4c12eb)

## 5.1.3 Check Your Understanding - Communication Protocols

- Check your understanding of communication protocols by choosing the correct answer to the following questions

## 5.2.1 Video - Devices in a Bubble

## 5.2.2 The Internet and Standards

- With the increasing number of new devices and technologies coming online, how is it possible to manage all the changes and still reliably deliver services such as email? The answer is internet standards
- A standard is a set of rules that determines how something must be done. Networking and internet standards ensure that all devices connecting to the network implement the same set of rules or protocols in the same manner. Using standards, it is possible for different types of devices to send information to each other over the internet. For example, the way in which an email is formatted, forwarded, and received by all devices is done according to a standard. If one person sends an email via a personal computer, another person can use a mobile phone to receive and read the email as long as the mobile phone uses the same standards as the personal computer

## 5.2.3 Network Standards Organizations

- An internet standard is the end result of a comprehensive cycle of discussion, problem solving, and testing. These different standards are developed, published, and maintained by a variety of organizations, as shown in the figure. When a new standard is proposed, each stage of the development and approval process is recorded in a numbered Request for Comments (RFC) document so that the evolution of the standard is tracked. RFCs for internet standards are published and managed by the Internet Engineering Task Force (IETF)
- Other standards organizations that support the internet are shown in the figure

## 5.2.4 Check Your Understanding - Communications Standards

- Check your understanding of communication standards by choosing the correct answer to the following questions

## 5.3.1 Video - Network Protocols

## 5.3.2 Video - The Protocol Stack

## 5.3.3 The TCP/IP Model

- Layered models help us visualize how the various protocols work together to enable network communications. A layered model depicts the operation of the protocols occurring within each layer, as well as the interaction with the layers above and below it.
- The layered model has many benefits:
    - Assists in protocol design, because protocols that operate at a specific layer have defined information that they act upon and a defined interface to the layers above and below
    - Fosters competition because products from different vendors can work together
    - Enables technology changes to occur at one level without affecting the other levels
    - Provides a common language to describe networking functions and capabilities
The first layered model for internetwork communications was created in the early 1970s and is referred to as the internet model. It defines four categories of functions that must occur in order for communications to be successful. The suite of TCP/IP protocols that are used for internet communications follows the structure of this model, as shown in the table. Because of this, the internet model is commonly referred to as the TCP/IP model

## 5.3.4 The OSI Reference Model

- There are two basic types of models that we use to describe the functions that must occur in order for network communications to be successful: protocol models and reference models
    - Protocol model - This model closely matches the structure of a particular protocol suite. A protocol suite includes the set of related protocols that typically provide all the functionality required for people to communicate with the data network. The TCP/IP model is a protocol model because it describes the functions that occur at each layer of protocols within the TCP/IP suite
    - Reference model - This type of model describes the functions that must be completed at a particular layer, but does not specify exactly how a function should be accomplished. A reference model is not intended to provide a sufficient level of detail to define precisely how each protocol should work at each layer. The primary purpose of a reference model is to aid in clearer understanding of the functions and processes necessary for network communications
- The most widely known internetwork reference model was created by the Open Systems Interconnection (OSI) project at the International Organization for Standardization (ISO). It is used for data network design, operation specifications, and troubleshooting. This model is commonly referred to as the OSI model

## 5.3.5 OSI Model and TCP/IP Model Comparison
- Because TCP/IP is the protocol suite in use for internet communications, why do we need to learn the OSI model as well?

- The TCP/IP model is a method of visualizing the interactions of the various protocols that make up the TCP/IP protocol suite. It does not describe general functions that are necessary for all networking communications. It describes the networking functions specific to those protocols in use in the TCP/IP protocol suite. For example, at the network access layer, the TCP/IP protocol suite does not specify which protocols to use when transmitting over a physical medium, nor the method of encoding the signals for transmission. OSI Layers 1 and 2 discuss the necessary procedures to access the media and the physical means to send data over a network

- The protocols that make up the TCP/IP protocol suite can be described in terms of the OSI reference model. The functions that occur at the internet layer in the TCP/IP model are contained in the network layer of the OSI Model, as shown in the figure. The transport layer functionality is the same between both models. However, the network access layer and the application layer of the TCP/IP model are further divided in the OSI model to describe discrete functions that must occur at these layers

- The key similarities are in the transport and network layers; however, the two models differ in how they relate to the layers above and below each layer:
    - OSI Layer 3, the network layer, maps directly to the TCP/IP internet layer. This layer is used to describe protocols that address and route messages through an internetwork
    - OSI Layer 4, the transport layer, maps directly to the TCP/IP transport layer. This layer describes general services and functions that provide ordered and reliable delivery of data between source and destination hosts
    - The TCP/IP application layer includes several protocols that provide specific functionality to a variety of end user applications. The OSI model Layers 5, 6, and 7 are used as references for application software developers and vendors to produce applications that operate on networks
    - Both the TCP/IP and OSI models are commonly used when referring to protocols at various layers. Because the OSI model separates the data link layer from the physical layer, it is commonly used when referring to these lower layers

## 5.3.6 Check Your Understanding - Network Communication Models

- Check your understanding of network communication models by choosing the correct answer to the following questions

## 5.4 Communication Principles Summary

- Communication Protocol
- Communication Standards
- Network Communication Models
- OSI Model Layer Description

## 5.4.2 Webster - Reflection Questions

- Recall that Kishori and Srivinas had to determine a common language... Do you have any friends or relatives whose first language is different than yours? Do you know anyone who uses sign language? How would you communicate with them if you did not know sign language? Did you realize that you were using a protocol (using a shared language or communicating in writing) to interact with family and friends?

## 5.4.3 Communications Principles Quiz

[Go to Next Module](./6_Network_Media.md)

