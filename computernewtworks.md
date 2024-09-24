->  A computer networks is a collection of devices  that are connected together to share resources and exchange data. 
    The devices in a network can be computers, printers.

    >>  Protocol -  A set of rules that govern how data is transmitted over a network. 
    >>   Network Topology -  The physical or logical arrangement of devices in a network. 

    OSI(open system  interconnection) model -  A 7-layered model that describes how data is transmitted over a  network. 
    
 # ** 7 layers of OSI model are : -**

        #### 1-  Physical layer =>   Defines how data is transmitted over a physical medium. It is responsible for transmitting bits from  one device to another. [ devices
         HUB(forward data to all the connected devices don't filter data ) , Repeater(2 ports amplify the strength of the signal )] 

        #### 2-  Data Link Layer =>    Provides error-free transfer of data frames between two devices on the same network. It is responsible  for framing, error detection and correction. [Switches ( forward data to the specific device using MAC Address also performs error checking ) , Bridges ( connect two or more networks together, 2-4 ports generally )] HOP To HOP delivery
        MAC(Media Access Control) = >   A unique address assigned to each device in a network. It is used to identify a device on  a network. consist of 12 digit hexadecimal number first 6 digits represents the manufacturer like HP,Huwaie next 6 digits represents the Network controller.
         -- 3 Types Unicast(LSB of 1st octate is set to  0), Multicast(LSB of 1st octate is set to 1), Broadcast (LSB of all digits is set to FF);

        #### 3-  Network Layer =>    Routes data between devices on different networks. It is responsible for  logical addressing, routing, congestion control.
         [Router (forward data to the specific device using IP address also selecting shorttest path to transfer data from sender to reciever)] Sender's and Reciever's IP address are placec in the header by the Network Layer.

        #### 4-  Transport Layer =>    Provides reliable data transfer between devices. It is responsible for end to end delivery of the complete message. It also provides
            aknowledegement of the data send and retransmits the data if aknowledgement donot came.

        #### 5-  Session Layer =>    Establishes, maintains, and terminates connections between applications running on different devices.  It is responsible for  synchronization, and session management and provides security. It uses encryption techniniqes to secure data to prevent  eavesdropping. It also  provides authentication and authorization means  to ensure that only authorized users can access the data. Dialogue control ensuring full duplex and halfduplex  communication. 

        #### 6-  Presentation Layer =>    Converts data into a format that can be understood by the  receiving device.It is responsible for encryption and decryption of
            data , data compression and decompression, and data formatting.  It also provides data conversion and translation for ex ASCII to Extended Binary coded decimal interchange code (EBCDIC)


         #### 7-  Application Layer =>    Provides services to end-user applications, such as email and  file transfer. It is responsible for   providing services to end-user applications, such as email and file transfer.


 # ** Network Topologies**

        1.  Bus Topology =>   All devices are connected to a single cable, called  the backbone. Data is transmitted over the backbone, and each device listens for data addressed to it.
        2.  Star Topology =>   All devices are connected to a central device, called  the hub. Data is transmitted from the sender to the hub, and the hub forwards the data to  the intended recipient.
        3.  Ring Topology =>   Devices are connected in a circular configuration, and data  is transmitted in one direction around the ring.  Each device acts as a repeater, amplifying the signal and forwarding it to the next device.
        4.  Mesh Topology =>   Each device is connected to every other device,  creating a web-like  structure. Data can be transmitted between any two devices, and each device acts  as a repeater, amplifying the signal and forwarding it to the next device.
        5.  Tree Topology =>   A combination of bus and star topologies, where  devices are  connected to a central device, and the central device is connected to a backbone cable.  Data is transmitted from the sender to the central device, and the central device forwards the data to the  intended recipient.

 ## Advanatges and Disadvantages of all  the topologies are as follows:
        Bus Topology =>   Advantages:  Easy to install and maintain,  cost-effective.  Disadvantages:  Difficult to troubleshoot,  prone to data corruption.
        Star Topology =>   Advantages:  Easy to install and maintain,  cost-effective,   easy to troubleshoot.  Disadvantages:  Central device can become a  single point  of failure.
        Ring Topology =>   Advantages:  High-speed data transfer,  reliable data transfer.   Disadvantages:  Difficult to install and maintain,  prone to data corruption.
        Mesh Topology =>   Advantages:  Highly reliable,  fault-tolerant,   high-speed data transfer.  Disadvantages:  Difficult to install and maintain,    cost-effective.
        Tree Topology =>   Advantages:  Easy to install and maintain,  cost-effective,    easy to troubleshoot.  Disadvantages:  Central device can become a  single point   of failure.

        Circuit Switching :  -  In this type of switching, a dedicated path is established between the sender and receiver before data  is transmitted. The path is held for the duration of the transmission, and then released.  This type of switching is  used in traditional telephone networks.
 ## Circuit Switching
 ![circuit](https://media.geeksforgeeks.org/wp-content/uploads/20240424165529/Circuit-Switching.webp)

        Packet Switching :   -  In this type of switching, data is divided into small packets, and each packet is  transmitted independently.  The packets are routed through the network, and reassembled at the receiver's  end.  This type of switching is used in modern computer networks. 
 ## Packet Switching
 ![packet](https://networkencyclopedia.com/wp-content/uploads/2019/10/packet-switching.png)

        **Advantages and Disadvantages of  Circuit Switching and Packet Switching are as follows:**
        Circuit Switching =>   Advantages:  Guaranteed bandwidth,  low latency.  Disadvantages:  Inefficient use of resources,  prone to congestion. 
        Packet Switching =>   Advantages:  Efficient use of resources,  flexible routing.   Disadvantages:  High latency,  prone to packet loss.
























