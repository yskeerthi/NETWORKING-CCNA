# Learning Networking :

## 1. Fiber Optic Cables :

Fiber optic cables are high-speed data transmission mediums. They contain strands of glass fibers inside an insulated casing. These cables are designed for long-distance and high-performance data networking and telecommunications.

**Example:** Fiber optic cables are used by ISPs (Internet Service Providers) to provide high-speed internet connections to homes and businesses.

## 2. Internet: Connection of Regions :

The Internet connects different regions worldwide through a network of physical cables, including fiber optics, copper cables, and satellite connections.

**Illustration:** Regions are interconnected through a global network of cables and satellite links, allowing data to travel across countries and continents.

## 3. Submarine Cable Map :

The Submarine Cable Map is a free and regularly updated resource from TeleGeography that shows the locations and connections of undersea cables worldwide. These submarine cables are crucial for international data transmission.

**Connected Undersea:** Submarine cables lie on the ocean floor, connecting different continents and enabling global communication.

## 4. Network Models :

### 1. Workgroup Model : (peer to peer)

> A workgroup model is a peer-to-peer network where each computer has equivalent capabilities and responsibilities. It is typically used in small networks.
> There is no security.

**Example:** A small office network where all computers can share files and printers directly with each other.

### 2. Server-Client Model : (client can only access)  

> In a server-client model, one central server provides resources and services to multiple client computers. This model is common in larger networks.
> The server can monitor, control, and take data from the client.

**Example:** A corporate network where a central server hosts applications, files, and data, which client computers access.

## 5. Commands :

1. `ipconfig` (cmd command): Displays the network configuration details of your computer, such as IP address, subnet mask, and default gateway.

   **Example:** Running `ipconfig` can help you find your computer's IP address.

2. `ncpa.cpl`: Opens the Network Connections window on a Windows computer, allowing you to view and manage network adapters.

   **Example:** Use `ncpa.cpl` to troubleshoot network connectivity issues.

3. `ping`: Checks the connectivity between two computers or IP addresses by sending packets and measuring response times.

   **Example:** `ping google.com` tests if your computer can reach Google's servers.

## 6. Sharing a File Through IP Addresses :

1. Right-click the file or folder you want to share.
2. Select "Share with".
3. Add "Everyone" to the list of people you want to share with.
4. Change permissions to "Read only" if you want others to view the file without making changes.

## 7. Manage Advanced Sharing Service :

- **Advanced network settings:** Turn on public and private network discovery and file sharing.
- **Turn on network discovery:** Allows your computer to see other computers and devices on the network and makes your computer visible to others.

**Example:** To access a shared folder on another computer, type `\\(IP Address)` in the Run dialog or File Explorer address bar.

## 8. RDP: Remote Desktop Protocol
- Can take control of another remote desktop.
- You have to know how to give access and take access.

### 1. To give access:
- Go to Settings: Go to Remote Desktop settings: Turn it on: Remove the check mark: Require computers to authenticate to connect.
- Go to Remote Desktop users.
- Add - type "Everyone".
- Go to Run.
- Type `mstsc`.
- Enter the IP and connect.

### 2. To take access:
- Open the Run dialog by pressing `Win + R`.
- Type `mstsc` and press Enter. This will open the Remote Desktop Connection client.
- In the Remote Desktop Connection window, enter the IP address or hostname of the remote machine you want to connect to.
- Click "Connect".
- You will be prompted to enter the username and password for the remote machine.
- After entering the credentials, click "OK".
- You should now be connected to the remote desktop.

## 9. Types of Devices

### 1. End Devices
> End devices include `PCs, laptops, and servers.` These are devices that users interact with directly. In computer language, a user interacting with an end device is referred to as an end user.

### 2. Intermediary Devices
> Intermediary devices include `switches and routers.` They play a crucial role in network communication, facilitating the flow of data from the source (where communication starts) to the destination (where communication ends). 

### 3. Connections
> Connections can be either wired or wireless, determining how devices are linked to the network infrastructure:

- **Wired Connections:** Devices are connected physically using cables such as Ethernet cables or fiber optic cables.
- **Wireless Connections:** Devices connect wirelessly using technologies like Wi-Fi or Bluetooth.

These connections enable data transmission across networks, ensuring communication between devices regardless of their physical location.

## 10. Network Media

### Physical Networking: Media Types

> Network media refers to the physical means through which data is transmitted from one device to another in a network. Different types of media include:

- **Copper Cables:** Utilized in Ethernet networks, copper cables are cost-effective and widely used for short to medium distance transmissions.
  Example: Cat5e, Cat6 cables.

- **Fiber Optics:** These cables use light pulses to transmit data over long distances at very high speeds and are immune to electromagnetic interference.
  Example: Single-mode fiber, multi-mode fiber.

- **Wireless:** Wireless media enable data transmission without physical cables, using radio waves or infrared signals.
  Examples: WiFi (802.11 standards), Bluetooth, NFC (Near Field Communication).

## 11. Network Sizes

### Various Network Sizes

> Networks come in different sizes depending on their scope and purpose:

1. **Small Home Network:** Typically includes devices like computers, printers, and smart devices connected within a household using WiFi or Ethernet.
   Example: Home WiFi network connecting laptops, smartphones, and smart TVs.

2. **Small Office / Home Office (SOHO):** Networks serving small businesses or home offices, often incorporating file sharing, printers, and basic network security.
   Example: A small office network with shared printers and centralized storage.

3. **Medium / Large Business Network:** More complex networks supporting larger organizations, involving multiple departments, servers, and advanced security measures.
   Example: Corporate network with multiple office locations connected via WAN, supporting thousands of users.

4. **Worldwide Network (Internet):** The largest network, connecting billions of devices globally, enabling communication and data exchange across continents.
   Example: The Internet, comprising interconnected networks of varying sizes and types worldwide.

## 12. LANs and WANs

### Local Area Networks (LANs) and Wide Area Networks (WANs)

> LANs and WANs are two fundamental types of networks:

- **LAN (Local Area Network):** A network confined to a small geographic area, typically within a single building or campus.
  Example: Office LAN connecting computers, printers, and servers within a company building.

- **WAN (Wide Area Network):** Spans a large geographical area, connecting LANs and other networks over long distances using leased lines or satellites.
  Example: Interconnection of multiple branch offices of a multinational corporation via leased lines or VPN over the Internet.

> All LANs connect to WANs to enable communication between geographically separated networks, facilitating global connectivity and data sharing.




