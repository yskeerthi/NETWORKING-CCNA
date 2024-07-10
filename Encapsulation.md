# Encapsulation and Decapsulation :

![image](https://github.com/karthikeya03/NETWORKING/assets/120096427/436f20a9-749f-4a20-9c0f-ebe6237c0274)


## 1.**Definitions:**  :

- **Encapsulation**: The process of adding headers and trailers to data as it moves down the layers of the OSI or TCP/IP model before transmission.
  - **Example**: When an email is sent, the data is encapsulated with an email header, TCP header, IP header, and Ethernet header as it moves through the layers.
- **Decapsulation**: The process of removing headers and trailers as data moves up the layers of the OSI or TCP/IP model upon reception.
  - **Example**: When the email reaches the recipient, the Ethernet header, IP header, and TCP header are removed to access the email data.

## 2.**Message Delivery Options:**  :

- **Unicast**: One-to-one communication between a single sender and a single receiver.
  - **Example**: A direct video call between two people.
- **Multicast**: One-to-many communication where a single sender transmits data to multiple specific receivers.
  - **Example**: A live webinar streamed to multiple registered participants.
- **Broadcast**: One-to-all communication where data is sent from a single sender to all possible receivers in the network.
  - **Example**: A TV station broadcasting a signal to all TVs within its range.

# Protocol Suite :

## OSI Model and TCP/IP Model :

![image](https://github.com/karthikeya03/NETWORKING/assets/120096427/9b3e4074-6eda-425c-ad7c-20a7545f4272)

**OSI Model** stands for Open Systems Interconnection.

| Layer   | OSI Model    | TCP/IP Model   | Example Protocols | Data Unit |
| ------- | ------------ | -------------- | ----------------- | --------- |
| Layer 7 | Application  | Application    | HTTP, FTP, SMTP   | Data      |
| Layer 6 | Presentation | -              | SSL, JPEG         | Data      |
| Layer 5 | Session      | -              | NetBIOS, RPC      | Data      |
| Layer 4 | Transport    | Transport      | TCP, UDP          | Segment   |
| Layer 3 | Network      | Internet       | IP, ICMP          | Packet    |
| Layer 2 | Data Link    | Network Access | Ethernet, PPP     | Frame     |
| Layer 1 | Physical     | Network Access | DSL, T1           | Bits      |

## Layer 7: Application (OSI) / Application (TCP/IP) :

- **Purpose**: This layer interacts directly with user applications.
- **Example Protocols**: 
  - **HTTP (Hypertext Transfer Protocol)**: Used for transferring web pages on the internet.
  - **FTP (File Transfer Protocol)**: Used for transferring files between a client and server.
  - **SMTP (Simple Mail Transfer Protocol)**: Used for sending emails.

## Layer 6: Presentation (OSI) :

- **Purpose**: This layer translates data between the application layer and the network.
- **Example Protocols**: 
  - **SSL (Secure Sockets Layer)**: Used for encrypting data for secure transmission.
  - **JPEG (Joint Photographic Experts Group)**: Used for image compression.

## Layer 5: Session (OSI) :

- **Purpose**: This layer manages sessions between applications.
- **Example Protocols**: 
  - **NetBIOS (Network Basic Input/Output System)**: Used for network communication in older systems.
  - **RPC (Remote Procedure Call)**: Used for executing code on a remote server.

## Layer 4: Transport (OSI and TCP/IP) :

- **Purpose**: This layer ensures reliable data transfer.
- **Example Protocols**: 
  - **TCP (Transmission Control Protocol)**: Ensures reliable, ordered delivery of data.
  - **UDP (User Datagram Protocol)**: Provides faster, but less reliable delivery of data.
  - Sequence numbers are added by the transport layer.

## Layer 3: Network (OSI) / Internet (TCP/IP) :

- **Purpose**: This layer handles routing of data between devices.
- **Example Protocols**: 
  - **IP (Internet Protocol)**: Responsible for addressing and routing packets of data.
  - **ICMP (Internet Control Message Protocol)**: Used for error messages and operational information.

## Layer 2: Data Link (OSI) / Network Access (TCP/IP) :

- **Purpose**: This layer handles error detection and correction from the physical layer.
- **Example Protocols**: 
  - **Ethernet**: Used for wired local area networks.
  - **PPP (Point-to-Point Protocol)**: Used for direct communication between two nodes.

## Layer 1: Physical (OSI) / Network Access (TCP/IP) :

- **Purpose**: This layer transmits raw bit streams over a physical medium.
- **Example Protocols**: 
  - **DSL (Digital Subscriber Line)**: Used for internet access over telephone lines.
  - **T1**: A type of fiber optic telephone line that can handle more data than DSL lines.
  - 1024 messages with trail go to the physical.

## Example: Encapsulation and Decapsulation in WhatsApp :

Let's take an example of sending a WhatsApp message.

### Encapsulation :

1. **Application Layer (Layer 7)**: The user types a message in WhatsApp and sends it. The message is converted into data that can be processed by the application layer.
2. **Transport Layer (Layer 4)**: The message data is divided into segments. TCP adds a header to each segment, including sequence numbers, to ensure that segments can be reassembled in the correct order at the destination.
3. **Network Layer (Layer 3)**: Each TCP segment is encapsulated in an IP packet. The IP packet includes source and destination IP addresses.
4. **Data Link Layer (Layer 2)**: The IP packet is encapsulated in a frame. The frame includes source and destination MAC addresses for delivery within the local network.
5. **Physical Layer (Layer 1)**: The frame is converted into bits and transmitted over the physical medium (e.g., Wi-Fi or cellular network).

### Decapsulation :

1. **Physical Layer (Layer 1)**: The receiver's device captures the bits from the physical medium and converts them back into a frame.
2. **Data Link Layer (Layer 2)**: The frame is processed, and the Data Link layer checks for errors. The MAC addresses are stripped off, and the remaining packet is passed up to the Network layer.
3. **Network Layer (Layer 3)**: The IP packet is examined, and the IP header is removed. The remaining segment is passed up to the Transport layer.
4. **Transport Layer (Layer 4)**: The TCP segment is processed. Sequence numbers are used to reassemble the message in the correct order. The TCP header is removed, and the data is passed up to the Application layer.
5. **Application Layer (Layer 7)**: The message data is converted into a format that can be displayed by the WhatsApp application, and the user sees the received message.

This process ensures that a message sent from one device can be received and understood by another device, even if they are connected via different networks and mediums.

![image](https://github.com/karthikeya03/NETWORKING/assets/120096427/f52f2dd3-c4d6-423a-9e62-859794a13e6f)

## 4. Globalization  :

- The process of enabling people around the world to communicate and interact with each other.
- **TCP/IP**: The fundamental protocol suite for the internet, enabling global connectivity.
-  **TCP** : transmission cloud protocol
-  **IP** : Internal protocol 
  - **IANA**: Internet Assigned Numbers Authority, responsible for managing IP address allocation, DNS root zone management, and other internet protocol resources.

## 5.Microsoft: NETBIOS  :

- **NETBIOS**: Network Basic Input/Output System, a protocol suite developed by IBM and adopted by Microsoft for communication within local area networks (LANs).

## 6.Apple  :

- **AppleTalk**: A proprietary suite of networking protocols developed by Apple for networking computers.

## 7.Netcall / Unix  :

- **UNIX**: A powerful, multiuser operating system with networking capabilities.

## 8. Useful Commands  :

- **Win+R**: Open the Run dialog box.
  - **services.msc**: Opens the Services management console, where you can start, stop, and manage services on a Windows machine.

- **tracert**: A command-line tool used to trace the path data takes from one network node to another.
  - **Example**: `tracert www.example.com` shows the route taken by packets to reach the example.com server.

- **netstat**: A command-line tool that displays network connections, routing tables, interface statistics, masquerade connections, and multicast memberships.
  - **Example**: `netstat -an` shows all active connections and listening ports.
