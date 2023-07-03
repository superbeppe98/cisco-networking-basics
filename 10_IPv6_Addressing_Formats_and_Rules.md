[Back to Syllabus](./README.md#course-syllabus)

## 10.0.1 Webster - Why Should I Take this Module?

- Kishori meets Rina for lunch again. Kishori is excited to tell Rina all that she has learned about IPv4 addresses. Rina congratulates her and asks her if she has heard about IPv6. IPv6? Kishori has no idea what IPv6 is! Do you? Let me help you out with that. Let's get started with this module! 

## 10.0.2 What Will I Learn in this Module?

- Module Title: IPv6 Addressing Formats and Rules
- Module Objective: Explain the features of IPv6 addressing

## 10.1.1 The Need for IPv6

- You already know that IPv4 is running out of addresses. That is why you need to learn about IPv6
- IPv6 is designed to be the successor to IPv4. IPv6 has a larger 128-bit address space, providing 340 undecillion (i.e., 340 followed by 36 zeroes) possible addresses. However, IPv6 is more than just larger addresses
- When the IETF began its development of a successor to IPv4, it used this opportunity to fix the limitations of IPv4 and include enhancements. One example is Internet Control Message Protocol version 6 (ICMPv6), which includes address resolution and address autoconfiguration not found in ICMP for IPv4 (ICMPv4)
- The depletion of IPv4 address space has been the motivating factor for moving to IPv6. As Africa, Asia and other areas of the world become more connected to the internet, there are not enough IPv4 addresses to accommodate this growth. As shown in the figure, four out of the five RIRs have run out of IPv4 addresse
- IPv4 has a theoretical maximum of 4.3 billion addresses. Private addresses in combination with Network Address Translation (NAT) have been instrumental in slowing the depletion of IPv4 address space. However, NAT is problematic for many applications, creates latency, and has limitations that severely impede peer-to-peer communications
- With the ever-increasing number of mobile devices, mobile providers have been leading the way with the transition to IPv6. The top two mobile providers in the United States report that over 90% of their traffic is over IPv6
- Most top ISPs and content providers such as YouTube, Facebook, and NetFlix, have also made the transition. Many companies like Microsoft, Facebook, and LinkedIn are transitioning to IPv6-only internally. In 2018, broadband ISP Comcast reported a deployment of over 65% and British Sky Broadcasting over 86%
- Internet of Things
    - The internet of today is significantly different than the internet of past decades. The internet of today is more than email, web pages, and file transfers between computers. The evolving internet is becoming an Internet of Things (IoT). No longer will the only devices accessing the internet be computers, tablets, and smartphones. The sensor-equipped, internet-ready devices of tomorrow will include everything from automobiles and biomedical devices, to household appliances and natural ecosystems
    - With an increasing internet population, a limited IPv4 address space, issues with NAT and the IoT, the time has come to begin the transition to IPv6

## 10.1.2 IPv4 and IPv6 Coexistence

- There is no specific date to move to IPv6. Both IPv4 and IPv6 will coexist in the near future and the transition will take several years. The IETF has created various protocols and tools to help network administrators migrate their networks to IPv6. 
- The migration techniques can be divided into three categories:
    - Dual stack
        - Dual stack allows IPv4 and IPv6 to coexist on the same network segment. Dual stack devices run both IPv4 and IPv6 protocol stacks simultaneously. Known as native IPv6, this means the customer network has an IPv6 connection to their ISP and is able to access content found on the internet over IPv6
    - Tunneling
        - Tunneling is a method of transporting an IPv6 packet over an IPv4 network. The IPv6 packet is encapsulated inside an IPv4 packet, similar to other types of data
    - Translation
    - Network Address Translation 64 (NAT64) allows IPv6-enabled devices to communicate with IPv4-enabled devices using a translation technique similar to NAT for IPv4. An IPv6 packet is translated to an IPv4 packet and an IPv4 packet is translated to an IPv6 packet
- The physical network topology shows on IPv6-only network on the left communication with an IPv4-only network on the right through a NAT64 router
- Note: Tunneling and translation are for transitioning to native IPv6 and should only be used where needed. The goal should be native IPv6 communications from source to destination

## 10.1.3 Check Your Understanding - IPv4 Issues

- Check your understanding of IPv4 issues by choosing the BEST answer to the following questions

## 10.2.1 Hexadecimal Number System

- Before you dive into IPv6 addressing, it's important that you know that IPv6 addresses are represented using hexadecimal numbers. This base sixteen number system uses the digits 0 to 9 and the letters A to F:

0 1 2 3 4 5 6 7 8 9 A B C D E F

In IPv6 addresses, these 16 digits are represented as hextets (discussed next) allowing us to represent these massive addresses in a much more readable format.

## 10.2.2 IPv6 Addressing Formats

The first step to learning about IPv6 in networks is to understand the way an IPv6 address is written and formatted. IPv6 addresses are much larger than IPv4 addresses, which is why we are unlikely to run out of them.

IPv6 addresses are 128 bits in length and written as a string of hexadecimal values. Every four bits is represented by a single hexadecimal digit; for a total of 32 hexadecimal values, as shown in the figure. IPv6 addresses are not case-sensitive and can be written in either lowercase or uppercase.

16-bit Segments or Hextets

Preferred Format

The previous figure also shows that the preferred format for writing an IPv6 address is x:x:x:x:x:x:x:x, with each “x” consisting of four hexadecimal values. The term octet refers to the eight bits of an IPv4 address. In IPv6, a hextet is the unofficial term used to refer to a segment of 16 bits, or four hexadecimal values. Each “x” is a single hextet which is 16 bits or four hexadecimal digits.

Preferred format means that you write IPv6 address using all 32 hexadecimal digits. It does not necessarily mean that it is the ideal method for representing the IPv6 address. In this module, you will see two rules that help to reduce the number of digits needed to represent an IPv6 address.

These are examples of IPv6 addresses in the preferred format.



## 10.2.3 Video - IPv6 Formatting Rules

## 10.2.4 Rule 1 – Omit Leading Zeros

- The first rule to help reduce the notation of IPv6 addresses is to omit any leading 0s (zeros) in any hextet. Here are four examples of ways to omit leading zeros:
    - 01ab can be represented as 1ab
    - 09f0 can be represented as 9f0
    - 0a00 can be represented as a00
    - 00ab can be represented as ab

This rule only applies to leading 0s, NOT to trailing 0s, otherwise the address would be ambiguous. For example, the hextet “abc” could be either “0abc” or “abc0”, but these do not represent the same value


## 10.2.5 Rule 2- Double Colon
The second rule to help reduce the notation of IPv6 addresses is that a double colon (::) can replace any single, contiguous string of one or more 16-bit hextets consisting of all zeros. For example, 2001:db8:cafe:1:0:0:0:1 (leading 0s omitted) could be represented as 2001:db8:cafe:1::1. The double colon (::) is used in place of the three all-0 hextets (0:0:0).

The double colon (::) can only be used once within an address, otherwise there would be more than one possible resulting address. When used with the omitting leading 0s technique, the notation of IPv6 address can often be greatly reduced. This is commonly known as the compressed format.

Here is an example of the incorrect use of the double colon: 2001:db8::abcd::1234.

The double colon is used twice in the example above. Here are the possible expansions of this incorrect compressed format address:

2001:db8::abcd:0000:0000:1234
2001:db8::abcd:0000:0000:0000:1234
2001:db8:0000:abcd::1234
2001:db8:0000:0000:abcd::1234
If an address has more than one contiguous string of all-0 hextets, best practice is to use the double colon (::) on the longest string. If the strings are equal, the first string should use the double colon (::).


## 10.2.6 Activity - IPv6 Address Representations
Instructions:

Convert the IPv6 addresses into short (omit the leading zeroes) and compressed forms. Enter letters in lowercase. Click Next to advance the activity to the next address.

## 10.3.1 What Did I Learn in this Module?

IPv4 Issues
The depletion of IPv4 address space has been the motivating factor for moving to IPv6. IPv6 has a larger 128-bit address space, providing 340 undecillion possible addresses. When the IETF began its development of a successor to IPv4, it used this opportunity to fix the limitations of IPv4 and include enhancements. One example is ICMPv6, which includes address resolution and address autoconfiguration not found in ICMPv4.

Both IPv4 and IPv6 coexist and the transition to only IPv6 will take several years. The IETF has created various protocols and tools to help network administrators migrate their networks to IPv6. The migration techniques can be divided into three categories: Dual Stack, Tunneling, and Translation. Dual stack devices run both IPv4 and IPv6 protocol stacks simultaneously. Tunneling is a method of transporting an IPv6 packet over an IPv4 network. The IPv6 packet is encapsulated inside an IPv4 packet, similar to other types of data. NAT64 allows IPv6-enabled devices to communicate with IPv4-enabled devices using a translation technique similar to NAT for IPv4. An IPv6 packet is translated to an IPv4 packet and an IPv4 packet is translated to an IPv6 packet.


## 10.3.1 What Did I Learn in this Module?

- IPv6 Addressing
    - IPv6 addresses are 128 bits in length and written as a string of hexadecimal values. Every four bits is represented by a single hexadecimal digit; for a total of 32 hexadecimal values. IPv6 addresses are not case-sensitive and can be written in either lowercase or uppercase. In IPv6, a hextet that refers to a segment of 16 bits, or four hexadecimal values. Each “x” is a single hextet, which is 16 bits or four hexadecimal digits. Preferred format means that you write IPv6 address using all 32 hexadecimal digits. Here is one example - fe80:0000:0000:0000:0123:4567:89ab:cdef
    - There are two rules that help to reduce the number of digits needed to represent an IPv6 address

Rule 1 – Omit Leading Zeros. You can only omit leading zeros, not trailing zeros.

01ab can be represented as 1ab
09f0 can be represented as 9f0
0a00 can be represented as a00
00ab can be represented as ab

Rule 2 – Double Colon. A double colon (::) can replace any single, contiguous string of one or more 16-bit hextets consisting of all zeros. For example, 2001:db8:cafe:1:0:0:0:1 (leading 0s omitted) could be represented as 2001:db8:cafe:1::1. The double colon (::) is used in place of the three all-0 hextets (0:0:0). The double colon (::) can only be used once within an address, otherwise there would be more than one possible resulting address. If an address has more than one contiguous string of all-0 hextets, best practice is to use the double colon (::) on the longest string. If the strings are equal, the first string should use the double colon (::).


## 10.3.2 Webster - Reflection Questions

Just when I was starting to get the hang of IPv4 addresses, I learned about IPv6 addresses! But since it looks like most networks use both types of addresses, I’m glad that I know a bit about each type. I guess it’s like cars on the road. Some are old but they still run. Newer cars have many more features and options than the older cars. And both older and newer cars are all driving on the same road. What is one obvious advantage to using IPv6 addresses instead of using IPv4 addresses?


## 10.3.3 IPv6 Addressing Formats and Rules Quiz
