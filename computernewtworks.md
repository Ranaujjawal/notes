->  A computer networks is a collection of devices  that are connected together to share resources and exchange data. 
    The devices in a network can be computers, printers.

    >>  Protocol -  A set of rules that govern how data is transmitted over a network. 
    >>   Network Topology -  The physical or logical arrangement of devices in a network. 

    OSI(open system  interconnection) model -  A 7-layered model that describes how data is transmitted over a  network. 
    
 # ** 7 layers of OSI model are : -**

   #### 1-  Physical layer =>
        Defines how data is transmitted over a physical medium. It is responsible for transmitting bits from  one device to another. 
        [ devices HUB(forward data to all the connected devices don't filter data ) , Repeater(2 ports amplify the strength of the signal )] 

 #### 2-  Data Link Layer => 
        Provides error-free transfer of data frames between two devices on the same network. It is responsible  for framing, error detection and correction.
         [Switches ( forward data to the specific device using MAC Address also performs error checking ) , Bridges ( connect two or more networks together, 2-4 ports generally )] HOP To HOP delivery
        MAC(Media Access Control) = >   A unique address assigned to each device in a network. It is used to identify a device on  a network. consist of 12 digit
         hexadecimal number first 6 digits represents the manufacturer like HP,Huwaie next 6 digits represents the Network controller.
         -- 3 Types Unicast(LSB of 1st octate is set to  0), Multicast(LSB of 1st octate is set to 1), Broadcast (LSB of all digits is set to FF);

   #### 3-  Network Layer =>  
          Routes data between devices on different networks. It is responsible for  logical addressing, routing, congestion control.
         [Router (forward data to the specific device using IP address also selecting shorttest path to transfer data from sender to reciever)]
          Sender's and Reciever's IP address are placec in the header by the Network Layer.

   #### 4- Transport Layer =>   
           Provides reliable data transfer between devices. It is responsible for end to end delivery of the complete message.
            It also provides aknowledegement of the data send and retransmits the data if aknowledgement donot came.

   #### 5- Session Layer =>   
            Establishes, maintains, and terminates connections between applications running on different devices.
              It is responsible for  synchronization, and session management and provides security.
               It uses encryption techniniqes to secure data to prevent  eavesdropping.
                It also  provides authentication and authorization means  to ensure that only authorized users can access the data.
                 Dialogue control ensuring full duplex and halfduplex  communication. 

   #### 6-  Presentation Layer =>  
           Converts data into a format that can be understood by the  receiving device.It is responsible for encryption and decryption of data , 
           data compression and decompression, and data formatting.  It also provides data conversion and translation for ex ASCII to Extended 
           Binary coded decimal interchange code (EBCDIC)


   #### 7-  Application Layer =>
            Provides services to end-user applications, such as email and  file transfer. It is responsible for 
              providing services to end-user applications, such as email and file transfer.


 # ** Network Topologies**

        1.  Bus Topology =>   All devices are connected to a single cable, called  the backbone. Data is transmitted over the backbone,
         and each device listens for data addressed to it.

        2.  Star Topology =>   All devices are connected to a central device, called  the hub. Data is transmitted from the sender to the hub,
         and the hub forwards the data to  the intended recipient.

        3.  Ring Topology =>   Devices are connected in a circular configuration, and data  is transmitted in one direction around the ring.  
        Each device acts as a repeater, amplifying the signal and forwarding it to the next device.

        4.  Mesh Topology =>   Each device is connected to every other device,  creating a web-like  structure. Data can be transmitted between 
        any two devices, and each device acts  as a repeater, amplifying the signal and forwarding it to the next device.

        5.  Tree Topology =>   A combination of bus and star topologies, where  devices are  connected to a central device, 
        and the central device is connected to a backbone cable.  Data is transmitted from the sender to the central device, and
         the central device forwards the data to the  intended recipient.

 ## Advanatges and Disadvantages of all  the topologies are as follows:
        Bus Topology =>   Advantages:  Easy to install and maintain,  cost-effective.  Disadvantages:  Difficult to troubleshoot, 
         prone to data corruption.
        Star Topology =>   Advantages:  Easy to install and maintain,  cost-effective,   easy to troubleshoot.  Disadvantages:
          Central device can become a  single point  of failure.
        Ring Topology =>   Advantages:  High-speed data transfer,  reliable data transfer.   Disadvantages:  Difficult to install and maintain,
          prone to data corruption.
        Mesh Topology =>   Advantages:  Highly reliable,  fault-tolerant,   high-speed data transfer.  Disadvantages:  Difficult to install
         and maintain,    cost-effective.
        Tree Topology =>   Advantages:  Easy to install and maintain,  cost-effective,    easy to troubleshoot.  Disadvantages:  Central
         device can become a  single point   of failure.

# Switching

 ## Circuit Switching
 ![circuit](https://media.geeksforgeeks.org/wp-content/uploads/20240424165529/Circuit-Switching.webp)

               Circuit Switching :  -  In this type of switching, a dedicated path is established between the sender and receiver 
               before data  is transmitted. The path is held for the duration of the transmission, and then released.  This type of 
               switching is  used in traditional telephone networks.
     
 ## **Packet Switching
 ![packet](https://networkencyclopedia.com/wp-content/uploads/2019/10/packet-switching.png)

          Packet Switching :   -  In this type of switching, data is divided into small packets, and each packet is 
           transmitted independently.  The packets are routed through the network, and reassembled at the receiver's end. 
           This type of switching is used in modern computer networks. 
       
  **Types of Packet switching
  1.  Connection-Oriented Packet Switching(Virtual circuit) =>   A dedicated path / virtual connection is established between
   the sender and receiver before data is transmitted.   The path is held for the duration of the transmission, and then released.
      This type of packet switching is used in traditional telephone networks. 

  2.   Connectionless Packet Switching (Datagram) =>   No dedicated path is established between the sender and receiver.  
   Each packet is transmitted independently, and the receiver reassembles the packets.  This type of  packet switching is used in modern computer networks. 

## **Advantages and Disadvantages of  Circuit Switching and Packet Switching are as follows:**
       () Circuit Switching =>   Advantages:  Guaranteed bandwidth,  low latency, enhanced security as only two parties are included.
         Disadvantages:  Inefficient use of resources,Expensive, high latency as delay in establishing the dedicated path. 
        () Packet Switching =>   Advantages:  Efficient use of resources,  flexible routing.   Disadvantages:  High latency,  
        prone to packet loss.
 
### Message Switching
![message](https://media.geeksforgeeks.org/wp-content/uploads/20240425133145/Message-swithcing.webp)      

      () Message switching => In this type of switching , a message is transmitted as a single unit, and the entire message is stored 
      in a buffer until  it is transmitted.  This type of switching is used in traditional telex networks. Their is no limit on  the 
      size of the message block. Entire message is transmittedin one go. Message do not directly reach the destination and reach 
      intermidate nodes before reaching the destination.

       ## **Advantages and Disadvantages of Message swithcing and Packet switching 

       Message Switching =>    Advantages:  Guaranteed delivery, message length is not limited, prority can be assigned to messages.  
                               Disadvantages:  Inefficient  use of resources, prone to congestion(accumumulation of messages at node),
                                 cannot be used for real-time applications as storing messages cause.


## Data link Layer Protocols
### Protocols : 

       1) Stop-wait :-   In this protocol, the sender sends a frame and waits for an acknowledgement from the receiver before sending the next frame.
       If the acknowledgement is not received, the sender retransmits the frame.  This protocol is  simple to implement but has low throughput(amount of 
       data transmitted per unit time. It is measured in bits per second (bps).) It is used in low-speed networks. 
       2)  Go-back-N :-   In this protocol, the sender sends a frame and continues sending frames until it  receives an acknowledgement from the receiver. 
       If the acknowledgement is not received, the sender retransmits all the frames sent since the last  acknowledgement.  This protocol is used in high-speed networks. 
       3) Selective Repeat :-    In this protocol, the receiver sends an acknowledgement for each frame it receives.  If the acknowledgement  is not received, the sender retransmits the frame.  This protocol is used in high-speed  networks. 

### Difference between Stop-wait and Go-back-N and Selective Repeat : 
      # Comparison of Stop and Wait, Go-Back-N, and Selective Repeat Protocols

| Key                      | Stop and Wait Protocol                             | Go-Back-N Protocol                           | Selective Repeat Protocol                                      |
|--------------------------|--------------------------------------------------------------|---------------------------------------------------------|----------------------------------------------------------------|
| **Sender Window Size**   | 1                                                            | N                                                       | N                                                              |
| **Receiver Window Size** | 1                                                            | 1                                                       | N                                                              |
| **Minimum Sequence Number** | 2                                                         | N + 1 (where N is the number of packets sent)           | 2N (where N is the number of packets transmitted)              |
| **Acknowledgement Type** | Individual                                                  | Cumulative                                              | Individual                                                      |
| **Supported Order**      | No specific order required at receiver                      | Only in-order delivery accepted at receiver             | Out-of-order deliveries accepted at receiver                   |
| **Retransmissions**      | 1 retransmission in case of packet drop                     | N retransmissions in case of packet drop                | 1 retransmission in case of packet drop                        |

       
### Bit stuffing  and Byte  stuffing : 

       =>  Bit stuffing:  the delimiting flag sequence generally contains six or more consecutive 1s. Most protocols use the 8-bit pattern 01111110
               as flag. In order to differentiate the message from the flag in case of same sequence, a single bit is stuffed in the message. Whenever a 0
               bit is followed by five consecutive 1bits in the message, an extra 0 bit is stuffed at the end of the five 1s. When the receiver receives 
               the message, it removes the stuffed 0s after each sequence of five 1s. The un-stuffed message is then sent to the upper layers.

 
       =>  Byte stuffing:   If the pattern of the flag byte is present in the message byte sequence, there should be a strategy so that the
              receiver does not consider the pattern as the end of the frame. Here, a special byte called the escape character (ESC) is stuffed
               before every byte in the message with the same pattern as the flag byte. If the ESC sequence is found in the message byte, then 
               another ESC byte is stuffed before it.


# ERROR Corrections Types :

### CRC(Cyclic Redundancy Check)
       CRC => In  this method, a polynomial is used to generate a checksum for the data. The checksum is appended to  the data and sent to the receiver. The reciever
       calculates the checksum using the same polynomial and compares it with the received checksum. If they match,  the data is accepted, otherwise it is rejected.
       Advantages:  Simple to implement, fast, and efficient.  Disadvantages:   Not suitable for long data streams.
       For N length data and M length divisor (M-1) 0s are appedend and then R is calculted and then then N+R is sent reciver cheks by peforming XOR with the D
       If 0 accept otherwise reject.
![](https://th.bing.com/th/id/OIP.gAioh2aSWc73Im5BqBXW6AHaHd?pid=ImgDet&w=195&h=196&c=7&dpr=1.4)

### Hamming Distance
       Hamming => Hamming Code is simply the use of extra parity bits to allow the identification of an error.

              Step 1: Write the bit positions starting from 1 in binary form (1, 10, 11, 100, etc).

              Step 2: All the bit positions that are a power of 2 are marked as parity bits (1, 2, 4, 8, etc).

              Step 3: All the other bit positions are marked as data bits.

              Step 4: Each data bit is included in a unique set of parity bits, as determined its bit position in binary form:

              a. Parity bit 1 covers all the bits positions whose binary representation includes a 1 in the least
               significant position (1, 3, 5, 7, 9, 11, etc).
              b. Parity bit 2 covers all the bits positions whose binary representation includes a 1 in the second position from the least
               significant bit (2, 3, 6, 7, 10, 11, etc).
              c. Parity bit 4 covers all the bits positions whose binary representation includes a 1 in the third position from the least 
              significant bit (4–7, 12–15, 20–23, etc).
              d. Parity bit 8 covers all the bits positions whose binary representation includes a 1 in the fourth position from the least 
              significant bit bits (8–15, 24–31, 40–47, etc).

              resoective even parity is calculated by couting the ones if even 0 else 1 then data is sent n data bits k redundant bits 
              reciever checks the data by again calcultaing the redudant bits if 0000  accept else covert it to binary to get the error bit.
![](https://th.bing.com/th/id/R.27b3885dfae2ddbab394d9f1cc1e32ad?rik=7YY0%2bpFg6FMKBg&riu=http%3a%2f%2fecomputernotes.com%2fimages%2fError-Detection--Correction.jpg&ehk=7vKPbPtsJeJAddg%2b4uUZ8f38xoB8wIqNMWEkBCYbpU0%3d&risl=&pid=ImgRaw&r=0)


## Access Control Protocols

### Pure Aloha
**Pure Aloha** is a simple, early random access protocol used for data transmission in networks. It does not coordinate when stations should transmit,
 which leads to a high probability of packet collision:
- **How It Works**: Nodes transmit data whenever they have data to send. If a collision occurs (two or more stations transmitting simultaneously), packets are destroyed, and each station must retransmit the packet after waiting a random amount of time.
- **Collision Handling**: If a collision is detected, the node will wait for a random backoff period before retransmitting. The random wait period reduces the likelihood of repeated collisions.
- **Efficiency**: Pure Aloha has a very low efficiency, with a theoretical maximum throughput of about 18.4%. It works best under low network loads.

### Slotted Aloha
**Slotted Aloha** improves Pure Aloha by reducing the chances of packet collision:
- **How It Works**: Time is divided into discrete slots. A node can only transmit at the beginning of a time slot. If two nodes attempt
 to send data in the same time slot, a collision occurs.
- **Collision Handling**: Similar to Pure Aloha, nodes will back off for a random period if a collision occurs. 
- **Efficiency**: Slotted Aloha has a higher efficiency than Pure Aloha, with a theoretical maximum throughput of about 36.8%.

### CSMA/CD (Carrier Sense Multiple Access with Collision Detection)
**CSMA/CD** is a network protocol used in wired Ethernet networks to manage collisions and ensure efficient communication:
- **Carrier Sense**: Before a device transmits, it checks if the medium is free (i.e., no other device is transmitting).
- **Multiple Access**: Multiple devices share the same communication channel.
- **Collision Detection**: If two devices transmit simultaneously, a collision occurs. Devices detect this collision, stop transmitting,
 and wait for a random time before retransmitting.
- **Usage**: CSMA/CD is mainly used in Ethernet (IEEE 802.3) networks and operates in half-duplex environments.

### CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance)
**CSMA/CA** is primarily used in wireless networks (e.g., Wi-Fi) to avoid collisions:
- **Carrier Sense**: Devices listen to the channel before transmitting to ensure it's idle.
- **Collision Avoidance**: Instead of detecting collisions, devices use techniques such as RTS (Request to Send) and 
CTS (Clear to Send) messages to avoid them. This is important in wireless networks where collisions are harder to detect.
- **Backoff Mechanism**: If the medium is busy, the device waits for a random backoff time to try again.
``` 
```
## Network Layer

### IP Addressing

#### Classful IP Addressing
- **Class A, B, C, D, E**: In classful addressing, IP addresses are divided into five classes:
  - **Class A**: Intended for large networks with a few hosts. IP range: `1.0.0.0` - `126.255.255.255`. Default subnet mask: `255.0.0.0`.
  - **Class B**: Designed for medium-sized networks. IP range: `128.0.0.0` - `191.255.255.255`. Default subnet mask: `255.255.0.0`.
  - **Class C**: For small networks. IP range: `192.0.0.0` - `223.255.255.255`. Default subnet mask: `255.255.255.0`.
  - **Class D**: Reserved for multicast groups. IP range: `224.0.0.0` - `239.255.255.255`.
  - **Class E**: Reserved for experimental purposes. IP range: `240.0.0.0` - `255.255.255.255`.

## Classful IP Addressing

In classful IP addressing, IP addresses are divided into five classes: **A, B, C, D, and E**. You can determine the class of 
an IP address based on the **first octet** (the first 8 bits of the address). The table below helps identify which class an IP address belongs to.

## IP Address Class Identification Table

| Class | First Octet Range | Binary Representation Start | Default Subnet Mask | Usage                   |
|-------|-------------------|-----------------------------|---------------------|-------------------------|
| A     | 1 - 126           | Starts with `0`             | 255.0.0.0           | Large networks          |
| B     | 128 - 191         | Starts with `10`            | 255.255.0.0         | Medium-sized networks   |
| C     | 192 - 223         | Starts with `110`           | 255.255.255.0       | Small networks          |
| D     | 224 - 239         | Starts with `1110`          | N/A                 | Multicast               |
| E     | 240 - 255         | Starts with `1111`          | N/A                 | Experimental purposes   |

### Special IP Addresses
- **127.x.x.x**: Reserved for **loopback** testing (e.g., `127.0.0.1` is the loopback address).
- **0.x.x.x**: Reserved and not assigned to any network.

### How to Identify the Class
- Look at the **first octet** of the IP address.
- Match the first octet to the appropriate **range** in the table above to determine the class.

### Examples
- **Class A**: `10.0.0.1` (First octet is `10`, which falls within `1 - 126`).
- **Class B**: `172.16.0.1` (First octet is `172`, which falls within `128 - 191`).
- **Class C**: `192.168.1.1` (First octet is `192`, which falls within `192 - 223`).
- **Class D**: `224.0.0.5` (First octet is `224`, which falls within `224 - 239`).
- **Class E**: `250.1.1.1` (First octet is `250`, which falls within `240 - 255`).

This table helps you easily identify the class of an IP address and understand its usage.

#### Classless IP Addressing (CIDR)
**Classless Inter-Domain Routing (CIDR)** is used for more efficient allocation of IP addresses:
- **Prefix Length**: Addresses use a `/` notation to indicate the length of the network prefix (e.g., `192.168.1.0/24` means the
 first 24 bits are for the network).
- **Advantages**: CIDR allows for more flexible subnetting, reduces the wastage of IP addresses, and improves routing efficiency.

```
```
# Understanding `192.168.0.0/22` in Detail

`192.168.0.0/22` is a representation of an IP address block in CIDR notation. The `/22` specifies that the first 22 bits are the **network portion**, 
and the remaining bits are for **hosts**. Let's break down how this notation provides **1024 IP addresses** in detail.

## Understanding CIDR Notation
- **CIDR Notation**: `192.168.0.0/22`
  - The `/22` means that the **first 22 bits** are fixed for the **network portion**.
  - The remaining **10 bits** are available for **hosts**.
  - Since an IPv4 address is 32 bits long:
    - **22 bits** are for the **network**.
    - **10 bits** are for **hosts**.

## Converting IP Address to Binary
To better understand, let's convert `192.168.0.0` into binary form:

- **192** in binary: `11000000`
- **168** in binary: `10101000`
- **0** in binary: `00000000`
- **0** in binary: `00000000`

Thus, `192.168.0.0` in binary is:
`11000000 10101000 00000000 00000000`

### Network and Host Portion
- In CIDR notation, `/22` means the **first 22 bits** are fixed for the network.
- The first 22 bits of `192.168.0.0` are:
`11000000.10101000.000000`
This represents the **network portion**.
- The remaining **10 bits** are for the **host portion**, which can vary to create unique IP addresses within the range.

## Calculating the Number of IP Addresses
- **10 bits** are available for the **host portion**.
- The total number of possible addresses is `2^10 = 1024`.

## Address Range
Let's determine the **range** of IP addresses:

- **Network Address**: `192.168.0.0`
- **Broadcast Address**: The last address in the range, where all host bits are `1`.

### Binary Representation for the Range
- **Network Address**: `11000000.10101000.00000000.00000000` (192.168.0.0)
- **First Host Address**: Increment the last 10 bits to `0000000001`:
- Result: `192.168.0.1`
- **Last Host Address**: Set the last 10 bits to all `1`s except for the broadcast bit:
- Result: `192.168.3.254`
- **Broadcast Address**: All 10 bits set to `1`:
- Result: `192.168.3.255`

### IP Address Range
- **Network Address**: `192.168.0.0`
- **First Usable Host**: `192.168.0.1`
- **Last Usable Host**: `192.168.3.254`
- **Broadcast Address**: `192.168.3.255`

Thus, there are **1024 IP addresses** in total, with **1022 usable addresses** for hosts (excluding the network and broadcast addresses).

## Breaking Down the Range
- The `/22` subnet spans across **4 Class C subnets**:
- `192.168.0.0` to `192.168.0.255` (256 addresses)
- `192.168.1.0` to `192.168.1.255` (256 addresses)
- `192.168.2.0` to `192.168.2.255` (256 addresses)
- `192.168.3.0` to `192.168.3.255` (256 addresses)
- Adding all of these gives `4 * 256 = 1024` addresses.

## Summary
- In `192.168.0.0/22`:
- **22 bits** are fixed for the **network** portion, and the remaining **10 bits** are for **hosts**.
- This results in `2^10 = 1024` possible IP addresses.
- The **range** of addresses is from `192.168.0.0` to `192.168.3.255`.
- **1022** of these addresses are **usable** for devices, with the rest reserved for the network and broadcast addresses.

CIDR addressing allows IP addresses to be allocated efficiently by letting network administrators adjust the subnet mask according to
 specific requirements. This flexibility helps reduce wastage of IP addresses compared to traditional classful addressing.


#### Subnet Mask
- A **subnet mask** is used to divide an IP address into network and host portions. It determines which part of the IP address refers to 
the network and which refers to the host.
  - **Example**: A subnet mask of `255.255.255.0` means the first 24 bits are used for the network, and the last 8 bits are for hosts.

#### Default Gateway
- The **default gateway** is the device (usually a router) that connects a local network to other networks, including the Internet.
 It is used by devices to send data to a different network when they do not have a specific route.

### Routing Protocols

#### RIP (Routing Information Protocol)
- **RIP** is a distance-vector routing protocol that uses hop count to determine the best path to a destination. It updates its 
routing tables every 30 seconds.
- **Hop Count Limit**: The maximum hop count is 15, making RIP suitable for smaller networks.
- **Issues**: Slow convergence and the potential for routing loops are significant drawbacks.

#### IPv4 vs IPv6
- **IPv4**: Uses 32-bit addresses, providing around 4.3 billion unique addresses. It supports fragmentation, options, and padding.
 Due to address exhaustion, alternatives like NAT are used to extend its usability.
- **IPv6**: Uses 128-bit addresses, providing a nearly unlimited address space. IPv6 simplifies the packet header, eliminates the 
need for NAT, and has built-in support for IPsec.

#### Fragmentation in IPv4
- **Fragmentation** occurs when a packet is larger than the MTU of the network path. The packet is divided into smaller fragments
 for transmission. Each fragment is reassembled by the destination device.

#### Options and Padding in IPv4
- **Options**: IPv4 allows optional fields in the header, such as security or timestamp.
- **Padding**: Padding bytes are added to ensure the IPv4 header is a multiple of 4 bytes in length.

#### Distance Vector Routing & Count to Infinity Problem
- **Distance Vector Routing**: Routers share their routing tables with neighboring routers at regular intervals. Routes are 
chosen based on metrics like hop count.
- **Count to Infinity Problem**: This issue arises in distance-vector routing when incorrect routing information loops between 
routers, causing infinite increases in route cost until it stabilizes.

#### ARP (Address Resolution Protocol)
- **ARP** is used to map a known IP address to a MAC address in a local network. It sends out an ARP request to find the physical
 address associated with an IP address.

#### NAT (Network Address Translation)
- **NAT** allows multiple devices on a local network to share a single public IP address by translating private IP addresses to a
 public one and vice versa. It improves security by hiding internal IP addresses.

## Transport Layer Protocols

### TCP (Transmission Control Protocol)
**TCP** is a connection-oriented, reliable transport layer protocol:
- **Connection Establishment**: Uses a three-way handshake to establish a connection before transmitting data.
- **Reliability**: Ensures reliable data delivery through error checking, acknowledgments, and retransmissions.
- **Flow Control**: Uses mechanisms like sliding window protocol to control data flow between sender and receiver.

### UDP (User Datagram Protocol)
**UDP** is a connectionless, unreliable protocol:
- **No Connection Establishment**: Data is sent without establishing a connection, making it faster but less reliable.
- **Use Cases**: Suitable for applications requiring low latency (e.g., video streaming, gaming).

### TCP vs UDP
- **TCP**: Reliable, ordered delivery, slower, connection-oriented (e.g., HTTP, FTP).
- **UDP**: Unreliable, unordered delivery, faster, connectionless (e.g., DNS, VoIP).

## Application Layer Protocols

### DNS (Domain Name System)
- **DNS** translates domain names (e.g., `www.example.com`) into IP addresses. It uses a hierarchical structure involving domain name servers.

### DHCP (Dynamic Host Configuration Protocol)
- **DHCP** is used to automatically assign IP addresses, subnet masks, gateways, and DNS server addresses to devices in a network, 
simplifying network administration.

### HTTP (HyperText Transfer Protocol)
- **HTTP** is the foundation of data communication on the web. It is a stateless protocol used for transferring hypertext (e.g., web pages).

### FTP (File Transfer Protocol)
- **FTP** is used for transferring files between a client and a server over a network. It uses two separate connections: one for commands
 and one for data transfer.

### SMTP (Simple Mail Transfer Protocol)
- **SMTP** is a protocol used to send emails from a client to a server or between servers.

### POP3 (Post Office Protocol 3)
- **POP3** allows clients to retrieve emails from a mail server. It downloads and usually deletes emails from the server, meaning messages
 cannot be accessed from multiple devices.

### IMAP (Internet Message Access Protocol)
- **IMAP** allows clients to retrieve and manage email messages on a server. Messages remain on the server and can be accessed from multiple devices, enabling synchronization.

### Telnet
- **Telnet** allows remote access to devices using a command-line interface. It lacks encryption, making it insecure for sensitive communication.

### SSH (Secure Shell)
- **SSH** provides secure, encrypted remote access to devices, making it a secure replacement for Telnet.

## IPv6

### Need for IPv6
IPv6 addresses several limitations of IPv4:
- **Address Exhaustion**: IPv4’s 32-bit addresses (approximately 4.3 billion addresses) have been exhausted. IPv6, with 128-bit addresses,
 provides a vastly larger address space.
- **Simplified Header**: IPv6 headers are designed to be simpler and more efficient.
- **Built-in Security**: IPv6 integrates IPsec, providing secure data exchange.
- **Efficient Routing**: IPv6 reduces the size of routing tables, making routing more efficient.

## Network Metrics

### Bandwidth vs Throughput vs Latency
- **Bandwidth**: The maximum rate at which data can be transferred over a network connection, usually measured in Mbps or Gbps.
- **Throughput**: The actual rate of successful data transfer over a network. It depends on various factors like network congestion and hardware limitations.
- **Latency**: The delay or time taken for a packet to travel from source to destination. It is usually measured in milliseconds (ms).

### Ping and Loopback
- **Ping**: A network diagnostic tool used to test connectivity between two devices. It measures round-trip time and packet loss.
- **Loopback**: The loopback address (`127.0.0.1`) is used to test the network functionality of the local machine.

## VPN (Virtual Private Network)
- A **VPN** is a service that allows users to create a secure, encrypted connection over a public network. It allows users to access resources
 on a private network securely.
- **Benefits**:
  - **Privacy**: Encrypts the data transmitted over the network.
  - **Security**: Allows secure access to corporate resources over an unsecured network.
  - **Remote Access**: Employees can securely access the company’s internal network from anywhere.


```
```
 # What Happens When You Type `google.com` in the Browser?
 ![](https://miro.medium.com/v2/resize:fit:1200/1*b1zrZoaJPq_FBdQkAsNJng.jpeg)

       When you type `google.com` in your browser and press Enter, a series of processes occur behind the scenes to display the Google homepage. 
       Here is a detailed, step-by-step explanation:

## 1. DNS Resolution
- **Domain Name System (DNS)**: The browser needs to find the IP address of `google.com`. Since humans use domain names but computers use IP addresses, a DNS query is made to resolve `google.com` into an IP address.
- **Cache Lookup**:
  - The **browser cache** is checked first to see if the IP address has been stored from a previous visit.
  - If not found, the **operating system cache** is checked.
  - If still not found, the **router cache** is queried.
  - Finally, the **ISP DNS server** is queried.
- **Recursive Lookup**: If necessary, the DNS server performs recursive lookups, querying other DNS servers until it finds the IP address of `google.com`.

## 2. Establishing a Connection
- After getting the IP address, your computer starts establishing a connection using **TCP/IP**.
- **TCP Three-Way Handshake**:
  1. **SYN**: The browser sends a **SYN** packet to the server.
  2. **SYN-ACK**: The server responds with a **SYN-ACK** packet.
  3. **ACK**: The browser sends an **ACK** packet, and the connection is established.

## 3. TLS Handshake (HTTPS)
- Since `google.com` uses **HTTPS**, a **TLS (Transport Layer Security)** handshake occurs to secure the communication.
- **Certificate Exchange**: The server sends its SSL/TLS certificate, and the browser verifies its validity.
- **Session Keys**: The browser and server generate **session keys** for encrypting the subsequent communication.

## 4. HTTP Request
- Once a secure connection is established, the browser sends an **HTTP GET request** to the server, requesting the homepage of `google.com`.
- The request includes headers with details like the browser type (user-agent), accepted formats, and cookies.

## 5. Server Processing
- The Google server processes the request. It may query databases, apply customizations based on cookies or user sessions.
- Once ready, the server generates an **HTTP response** containing the HTML code, CSS, JavaScript, and other resources required to render the page.

## 6. HTTP Response
- The server sends the **HTTP response** back to the browser, which includes:
  - **HTML**: The structure of the webpage.
  - **CSS**: The styling information.
  - **JavaScript**: Scripts to add interactivity.
  - **Cookies**: Data that identifies the user or maintains session state.

## 7. Rendering the Page
- **HTML Parsing**: The browser parses the HTML, creating a **DOM (Document Object Model)**.
- **CSS Parsing**: CSS files are fetched and parsed, determining how the elements are styled.
- **JavaScript Execution**: JavaScript code is executed to add interactivity. External scripts are fetched and executed unless they are marked as deferred or asynchronous.
- **Resource Fetching**: The browser fetches additional resources like images, videos, and fonts as needed.

## 8. Rendering Engine
- The **rendering engine** combines the parsed HTML, CSS, and JavaScript to render the webpage.
- **Layout Calculation**: The browser calculates the layout of each element.
- **Painting and Compositing**: The browser paints the pixels on the screen, using the **GPU** when necessary.

## 9. Handling JavaScript and Additional Requests
- JavaScript on the page may make **AJAX requests** to get more data from the server without a full page reload.
- **Event Listeners**: JavaScript adds event listeners, making the page interactive (e.g., responding to button clicks).

## 10. User Interaction
- After the page is loaded, any interaction, such as typing in the search bar or clicking links, triggers new **HTTP requests** and **responses**.

## Summary of Key Components Involved
1. **DNS Resolution**: Converts `google.com` to an IP address.
2. **TCP Handshake**: Establishes a reliable connection.
3. **TLS Handshake**: Secures the connection.
4. **HTTP Request/Response**: Requests the web page and receives content.
5. **Rendering Engine**: Parses and displays the webpage.

These processes occur quickly, often in milliseconds, creating the illusion of an almost instantaneous response.
```
```
### Python program to convert  a URL to an IP address using the `socket` library
  
```py

import socket

def get_ip_address(domain_name):
    try:
        # Get the IP address for the given domain name
        ip_address = socket.gethostbyname(domain_name)
        print(f"The IP address of {domain_name} is: {ip_address}")
    except socket.gaierror:
        print(f"Unable to resolve the domain name: {domain_name}")

# Get domain name input from user
domain_name = input("Enter a domain name (e.g., google.com): ")
get_ip_address(domain_name)

```

This program takes a domain name as input, attempts to resolve it to an IP address using the `

### ip address class checker 
``` cpp

string check_ip_class(string& ip_address) {
   istringstream ss(ip_address);
    string octet;
    vector<int> octets;

    // Split the IP address into octets
    while (getline(ss, octet, '.')) {
        // Convert the octet to an integer
        octets.push_back(std::stoi(octet));
    }

    // Check if there are exactly 4 octets
    if (octets.size() != 4) {
        return "Invalid IP address format.";
    }

    int first_octet = octets[0];

    if (first_octet >= 1 && first_octet <= 126) {
        return "Class A";
    } else if (first_octet >= 128 && first_octet <= 191) {
        return "Class B";
    } else if (first_octet >= 192 && first_octet <= 223) {
        return "Class C";
    } else if (first_octet >= 224 && first_octet <= 239) {
        return "Class D (Multicast)";
    } else if (first_octet >= 240 && first_octet <= 255) {
        return "Class E (Experimental)";
    } else {
        return "Invalid IP address range.";
    }
}

```
# Comparison of Classful and Classless IP Addressing

| Feature                     | Classful Addressing                         | Classless Addressing                       |
|-----------------------------|---------------------------------------------|--------------------------------------------|
| **Addressing Scheme**       | Fixed classes (A, B, C, D, E)               | Variable-length subnet masks (CIDR)        |
| **Network Size**            | Predefined network sizes based on class     | Flexible network sizes, based on requirements |
| **Subnet Mask**             | Implied by the class (e.g., /8 for Class A) | Defined by the network prefix (e.g., /22)  |
| **IP Address Utilization**  | Wastes addresses due to rigid class sizes   | Efficient use of IP addresses              |
| **Route Summarization**     | Limited capability                          | Allows for route aggregation (supernetting) |
| **Routing Table Size**      | Larger due to multiple routes               | Smaller due to route summarization         |
| **Network Prefix**          | Fixed by class (A, B, C)                    | Customizable network prefix                |
| **Scalability**             | Limited, as fixed classes restrict flexibility | High scalability with customized subnetting |

## Advantages and Disadvantages

### Classful Addressing

| **Advantages**                                 | **Disadvantages**                                |
|------------------------------------------------|--------------------------------------------------|
| Simple to understand and implement.            | Fixed network sizes lead to inefficient use of IP addresses.(wastage) |
| No need for additional subnet information.     | Limited scalability due to predefined class sizes. |
| Routing was simpler due to fixed structure.    | Large routing tables because of a lack of route summarization. |

### Classless Addressing (CIDR)

| **Advantages**                                 | **Disadvantages**                                |
|------------------------------------------------|--------------------------------------------------|
| Efficient use of IP address space.             | More complex to understand and configure.        |
| Allows for variable-length subnets (VLSM).     | Network management can be challenging for beginners. |
| Enables route aggregation, reducing routing table size. | Migration from classful to classless can be complex for older systems. |
| Better suited for modern networks and IPv4 conservation. | Increased processing for routing updates due to more flexible subnet masks. |

```
```
# vpn working 
VPN (Virtual Private Network) works by creating a secure, encrypted connection between two endpoints over the internet
## Example: Browsing with a VPN
Imagine Alice wants to securely browse a website (e.g., `example.com`) while connected to public Wi-Fi at a coffee shop. Here’s how a VPN keeps her safe:

1. **Alice Connects to a VPN**:
   - Alice opens her VPN app and connects to a VPN server. This establishes an encrypted tunnel between her device and the server.

2. **Alice Browses the Website**:
   - Alice types `example.com` into her browser. The request is **encrypted** and sent through the secure VPN tunnel to the VPN server.

3. **VPN Server Processes the Request**:
   - The VPN server receives the request and forwards it to `example.com`.
   - Since the request originates from the VPN server, `example.com` only sees the **IP address of the VPN server** and not Alice's real IP.

4. **Data Sent Back**:
   - `example.com` responds with the requested content, which is sent to the VPN server.
   - The VPN server **encrypts** the data and sends it back to Alice's device through the tunnel.
   - The VPN app on Alice's device decrypts the data so she can view it in her browser.

























