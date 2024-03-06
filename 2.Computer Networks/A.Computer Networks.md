# Computer Networks
Computer networks are intricate systems composed of interconnected nodes linked through communication channels. These nodes encompass a variety of devices like computers, printers, and other peripherals, all capable of exchanging data within the network. The primary goal of a computer network is to facilitate efficient sharing of resources and information among its interconnected components. These networks are categorized based on size, geographical coverage, and the communication technologies they employ.


## Key Objectives of Creating and Deploying a Computer Network

1. **Resource Sharing:** Modern enterprises operate on a global scale, distributing crucial assets across various departments, geographic locations, and time zones. Clients are no longer constrained by physical boundaries. Networks play a pivotal role in ensuring that data and hardware are accessible to relevant users, facilitating seamless collaboration and interdepartmental data processing. As an illustration, the marketing team utilizes customer data and product development timelines to inform executive decisions at the highest levels of the organization.

2. **Resource Availability & Reliability:** A network ensures that resources are not present in inaccessible silos and are available from multiple points. The high reliability comes from the fact that there are usually different supply authorities. Important resources must be backed up across multiple machines to be accessible in case of incidents such as hardware outages.

3. **Performance Management:** As a company expands, its workload naturally grows. Introducing additional processors to the network not only enhances the overall system performance but also facilitates accommodating this expansion. Efficiently storing data in well-architected databases can significantly enhance the speed of lookup and retrieval processes.

4. **Cost Savings:** Cost savings are achieved through strategic placement of processors in the system instead of investing in expensive mainframe computers. This approach not only enhances performance but also reduces costs. Networks allow employees to access information quickly, saving operational time and expenses. Centralized network administration minimizes the need for additional investments in IT support.

5. **Increased Storage Capacity:** Network-attached storage devices are a boon for employees who work with high volumes of data. For example, every member in the data science team does not need individual data stores for the huge number of records they crunch. Centralized repositories get the job done in an even more efficient way. With businesses seeing record levels of customer data flowing into their systems, the ability to increase storage capacity is necessary in today’s world.

6. **Streamlined Collaboration & Communication:** Networks have a major impact on the day-to-day functioning of a company. Employees can share files, view each other’s work, sync their calendars, and exchange ideas more effectively. Every modern enterprise runs on internal messaging systems such as Slack for the uninhibited flow of information and conversations. However, emails are still the formal mode of communication with clients, partners, and vendors.

7. **Reduction of Errors:** Networks reduce errors by ensuring that all involved parties acquire information from a single source, even if they are viewing it from different locations. Backed-up data provides consistency and continuity. Standard versions of customer and employee manuals can be made available to a large number of people without much hassle.

8. **Secured Remote Access:** Computer networks promote flexibility, which is important in uncertain times like now when natural disasters and pandemics are ravaging the world. A secure network ensures that users have a safe way of accessing and working on sensitive data, even when they’re away from the company premises. Mobile handheld devices registered to the network even enable multiple layers of authentication to ensure that no bad actors can access the system.


##  Types of Computer Network

1. **Local Area Network (LAN)**
    - **Scope:** Limited to a small geographic area, such as a single building, office, or campus.
    - **Topology:** Can be wired (Ethernet) or wireless (Wi-Fi).
    - **Purpose:** Facilitates communication and resource sharing among devices within the same organization or physical location.
    - **Examples:** Office networks, school networks, home networks.
    - **Characteristics:** High data transfer rates, low latency, and typically owned, set up, and maintained by a single organization.

2. **Wide Area Network (WAN)**
    - **Scope:** Spans a large geographic area, connecting multiple LANs across cities, countries, or continents.
    - **Topology:** Utilizes a variety of technologies, including leased lines, satellites, and public or private data networks.
    - **Purpose:** Enables long-distance communication and resource sharing between geographically dispersed locations.
    - **Examples:** The internet, global corporate networks.
    - **Characteristics:** Slower data transfer rates compared to LANs, higher latency, and often involves a mix of public and private infrastructure.

3. **Metropolitan Area Network (MAN)**
    - **Scope:** Covers a geographic area larger than a single LAN but smaller than a WAN, typically serving a metropolitan area like a city.
    - **Topology:** Similar to LANs, with the choice of wired or wireless technologies.
    - **Purpose:** Connects multiple LANs within a city, facilitating communication and data exchange between these local networks.
    - **Examples:** City-wide networks connecting government offices, universities, and businesses.
    - **Characteristics:** Faster data transfer rates compared to WANs, lower latency, and may involve high-speed connections like fiber optics.

4. **Personal Area Network (PAN)**
    - **Scope:** The smallest and most personal network, typically within the immediate proximity of an individual person.
    - **Topology:** Often wireless, using technologies like Bluetooth or infrared.
    - **Purpose:** Connects personal devices to facilitate communication and data exchange for an individual user.
    - **Examples:** Bluetooth-connected devices like smartphones, laptops, and wearable gadgets.
    - **Characteristics:** Very short-range, designed for personal and portable devices, enabling seamless connectivity in a limited space.

5. **Cloud Network**
    - **Definition:** A cloud network refers to a distributed computing environment that utilizes the internet to provide scalable, on-demand resources and services.
    - **Topology:** Virtualized infrastructure often spanning multiple physical locations.
    - **Purpose:** Facilitates access to computing resources, storage, and services without the need for local hardware.
    - **Examples:** Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform (GCP).
    - **Characteristics:** Highly scalable, flexible, and accessible remotely, allowing organizations to offload IT infrastructure and services to cloud providers.


## Computer Network Topologies
A Network Topology is the shape or arrangement of a Network with which computer systems or network devices are connected to each other. This arrangement is known as network topology, and it delineates how different network elements are interconnected. Topologies may define both physical and logical aspect of the network. Both logical and physical topologies could be same or different in a same network.

### Types of Computer Network Topology

1. **Bus Topology:** 
- In a bus topology, all devices (computers, printers, etc.) are connected to a single central cable called the "bus" or "backbone."
- Each device has a unique address, and data is transmitted along the bus. The data is received by all devices, but only the one with the matching address processes it.
- The main drawback is that if the central cable fails or breaks, the entire network is affected.

2. **Ring Topology:** In ring topology, each host machine connects to two other machines, creating a circular network structure. For any cause, if any host break down then whole network will break down. Thus, every connection in the ring is a point of failure.

3. **Star Topology:** In Star topology, all hosts are connected to a central device, known as a hub device, using a point-to-point connection. That is, there exists a point to point connection between hosts and hub. If the Hub fails for any cause, then the whole network will be broken.

4. **Tree Topology:** This topology is the combination of Bus and Star Topology. In this topology, each Star topology being connected via a single communication line or cable. This is the most common form of network topology in use presently. The main problem in this topology is if that single cable breaks then the whole network will break down.

5. **Mesh Topology:** In this topology, each host are interconnected with each other through various redundant connections. It does not contain the switch, hub or any central computer which acts as a central point. The Internet is the main example of Mesh Topology. But the main issue with this network is this topology, networks are very large and very difficult to maintain and manage. If the network is not monitored carefully, then the communication link failure goes undetected.

6. **Hybrid Topology:** Hybrid topology is a combination of two or more different types of topologies. Organizations often use a mix of topologies to meet specific networking needs. For example, combining the star and ring topologies creates a hybrid known as a star-ring topology. This approach aims to leverage the advantages of different topologies while mitigating their individual limitations.


## Comouter Network Models
Computer network models refer to conceptual frameworks that define the structure and functionality of computer networks. These models help in understanding, designing, and implementing communication systems that enable the exchange of data between devices. 

### Types of Computer Netwok Models

1. **OSI Model (Open Systems Interconnection):** The OSI model is a conceptual framework developed by the International Organization for Standardization (ISO) to standardize network communications. It consists of seven layers, each responsible for specific functions. The layers, from the lowest to the highest, are:
    - A. **Physical Layer**: Physical layer is the lowest layer of OSI model and is responsible for the physical connection between all the required devices. The information present in physical layer is in the form of bits. Physical layer performs various functions such as bit rate control, bit synchronization, transmission mode etc.
    - B. **Data Link Layer**: Data Link layer provides with successful delivery of message from one node to the another. It checks whether this delivery of message is error free. Other functions performed by data link layer are error control, framing, flow control etc.
    - C. **Network Layer**: Network Layer is responsible for the transmission of data from one host to the another host that is connected in different network. It performs other tasks such routing and logical addressing.
    - D. **Transport Layer**: Transport Layer is defined as a layer that takes services from network layer and provides services to application layer. Other tasks performed by transport layer are service point addressing, segmentation and reassembling.
    - E. **Session Layer**: Session layer is defined as a layer that is responsible for establishing a connection, maintenance of session and to provide with security. Other functions of session Layer are to establish session, termination and synchronisation.
    - F. **Presentation Layer**: The data from application layer is extracted at the presentation layer. This layer is also known as translation layer. The functions of presentation layer are encryption, decryption, compression and translation.
    - G. **Application Layer**: Application layer is the topmost layer of OSI Model. Application layer is also known as desktop layer. It provides with other functions such as directory services, mail services, network virtual terminal etc.

2. **TCP/IP Model:** The TCP/IP model is a more practical and widely used model in the context of the Internet. The layers, from the lowest to the highest, are:
    - A. **Network Access Layer**: Network access layer is the lowest layer of TCP/IP model. It is a combination of data link layer and physical layer present in the OSI model. The main function of network access layer is to transmit the information from one system to another that are connected in the same network.
    - B. **Internet Layer**: Internet layer is also known as network layer. Internet layer ensures that data is sent accurately and fastly by controlling the flow and routing of traffic. If the internet traffic is more it takes more time to transfer the data.
    - C. **Transport Layer**: Transport layer is responsible to provide a reliable connection between two communicating devices. In the incoming data is divided into packets by the transport layer and makes an acknowledgement when packet is received from the sender. UDP and TCP protocols are used in transport layer.
    - D. **Application Layer**: Application layer is the top most layer in TCP/IP model. Application layer provides the devices to access network and applications such as emails, cloud storage etc. While communicating from one application layer protocol to another application layer the information is forwarded to transport layer.


**NOTE**:
- `Computer Network Topology` refers to the layout or structure of a computer network, encompassing both the physical and logical arrangement of devices and their interconnections. The physical topology involves the actual physical placement of devices like computers, routers, switches, and cables, while the logical topology focuses on how data is transmitted between these devices. There are various types of network topologies, including bus, star, ring, mesh, and hybrid topologies. 
- `Computer Network Model` is a conceptual framework that defines how communication and data transmission occur within a network. It outlines the principles and rules governing the exchange of information between devices. Different network models exist, with the OSI (Open Systems Interconnection) model and the TCP/IP (Transmission Control Protocol/Internet Protocol) model being the most widely used.


## Computer Network Architecture
Computer Network Architecture refers to the comprehensive blueprint encompassing the intricate arrangement of software, hardware, communication protocols, and transmission media. It serves as the foundational framework dictating the organization of computers and the strategic allocation of tasks within a networked environment. Essentially, it delineates the structured and interconnected landscape through which data is exchanged, emphasizing both the physical and logical components that collectively enable seamless communication and collaboration among computing devices.

### Types of Computer Network Architecture

1. **Peer-To-Peer Network:** In a Peer-to-Peer (P2P) network architecture, each device, or node, in the network has an equal status and can both share and access resources without the need for a centralized server. This collaborative model allows for a more decentralized and flexible structure, making it well-suited for small to medium-sized networks. Peers in a P2P network can function both as clients and servers, facilitating direct communication and resource-sharing among them. While P2P networks are easy to set up and cost-effective, they may face challenges in terms of security and scalability.

2. **Client/Server Network:** The Client/Server network architecture is characterized by a clear division of roles between two distinct entities: clients and servers. Clients are devices that request services, resources, or information, while servers are dedicated to fulfilling these requests. This centralized model enhances efficiency, security, and management capabilities. Clients are typically end-user devices like computers or smartphones, and servers handle tasks such as storing data, running applications, or managing network resources. This architecture is well-suited for larger networks and enterprise-level operations due to its organized and scalable nature. While it offers robust security and centralized control, it may introduce potential points of failure and increased infrastructure costs.


## Key Components of a Computer Network

1. **Network Devices**
2. **Links**
3. **Communication Protocols** 
4. **Network Defense** 


## Network Devices
Computer network components consist of both physical parts as well as software in order to install computer networks. The hardware components include a server, client, hub, switch, bridge, peer, and connecting devices. Software components include the protocols and the Operating System (OS).

1. **Server:** A server is a powerful computer or system dedicated to managing network resources and providing services to other computers, known as clients, within the network. Servers can host various applications, files, and services such as email, web hosting, or databases. They typically have more processing power, storage capacity, and memory than regular computers. Servers are crucial components in client-server architecture, where clients request services, and servers fulfill those requests.

2. **Client:** A client is a computer or device that requests services or resources from a server within a network. Clients are the end-user devices, such as desktop computers, laptops, smartphones, or tablets, that access and utilize the resources provided by servers. Clients communicate with servers through a network, sending requests for data, applications, or services, and receiving responses from the server. In a client-server model, the server manages and provides resources, while the client consumes and interacts with these resources.

3. **Repeater:** A repeater operates at the physical layer. Its job is to regenerate the signal over the same network before the signal becomes too weak or corrupted to extend the length to which the signal can be transmitted over the same network. An important point to be noted about repeaters is that they not only amplify the signal but also regenerate it. When the signal becomes weak, they copy it bit by bit and regenerate it at its star topology connectors connecting following the original strength. It is a 2-port device. 

4. **Hub:**  A hub is a basically multi-port repeater. A hub connects multiple wires coming from different branches, for example, the connector in star topology which connects different stations. Hubs cannot filter data, so data packets are sent to all connected devices.  In other words, the collision domain of all hosts connected through Hub remains one.  Also, they do not have the intelligence to find out the best path for data packets which leads to inefficiencies and wastage. 

5. **Bridge:**  A bridge operates at the data link layer. A bridge is a repeater, with add on the functionality of filtering content by reading the MAC addresses of the source and destination. It is also used for interconnecting two LANs working on the same protocol. It has a single input and single output port, thus making it a 2 port device.

6. **Switch:**  A switch is a multiport bridge with a buffer and a design that can boost its efficiency(a large number of ports imply less traffic) and performance. A switch is a data link layer device. The switch can perform error checking before forwarding data, which makes it very efficient as it does not forward packets that have errors and forward good packets selectively to the correct port only.  In other words, the switch divides the collision domain of hosts, but the broadcast domain remains the same. 

7. **Routers:**  A router is a device like a switch that routes data packets based on their IP addresses. The router is mainly a Network Layer device. Routers normally connect LANs and WANs and have a dynamically updating routing table based on which they make decisions on routing the data packets. The router divides the broadcast domains of hosts connected through it.

8. **Gateway:** Gateways are hardware devices that act as ‘gates’ between two distinct networks. They can be firewalls, routers, or servers. They work as messenger agents that take data from one system, interpret it, and transfer it to another system. Gateways are also called protocol converters and can operate at any network layer. Gateways are generally more complex than switches or routers. A gateway is also called a protocol converter. 

9. **Brouter:** It is also known as the bridging router is a device that combines features of both bridge and router. It can work either at the data link layer or a network layer. Working as a router, it is capable of routing packets across networks and working as the bridge, it is capable of filtering local area network traffic. 

10. **NIC:** NIC or Network Interface Card is a network adapter that is used to connect the computer to the network. It is installed in the computer to establish a LAN.  It has a unique id that is written on the chip, and it has a connector to connect the cable to it. The cable acts as an interface between the computer and the router or modem. NIC card is a layer 2 device which means that it works on both the physical and data link layers of the network model.


## Links
"Links" refers to the connections or communication pathways that allow devices to communicate with each other. Links can be physical or logical connections, and they play a crucial role in establishing network connectivity.

1. **Physical Links:** Physical links can be established using either Wired Connection or Wireless Connections
    - **Wired Connection**: A computer network that connects devices using physical cables like coaxial, twisted-pair, or fiber optic cables. It offers reliability and faster data transmission, suitable for stationary environments like homes, offices, and data.
    - **Wireless Connection**: Wireless networks enable device communication without physical cables, using radio waves or electromagnetic signals. Examples include Wi-Fi, cellular, and satellite networks, providing mobility for devices like mobiles and laptops. Ideal for scenarios requiring flexibility and movement.

2. **Logical Links:**  Logical links, also known as virtual links, are pathways for communication between devices in a network, existing alongside physical connections. Unlike physical links that involve tangible cables or connections, logical links are established through protocols and addressing schemes at the network layer of the OSI model. These virtual connections allow devices to communicate seamlessly, and IP addresses are a key component in the establishment and maintenance of logical links within an IP network. By defining rules and pathways for data transfer, logical links ensure efficient and organized communication between devices in a networked environment.

**Types of Links:**
- **Point-to-Point Link**: Connects two devices directly, such as a link between two routers or a computer and a printer.
- **Multipoint Link**: Connects more than two devices, like a shared Ethernet network where multiple devices are connected to a common communication medium.


## Communication Protocols
A communication protocol is a set of rules followed by all nodes involved in the information transfer. Some common protocols include the internet protocol suite (TCP/IP), IEEE 802, Ethernet, wireless LAN, and cellular standards. TCP/IP is a conceptual model that standardizes communication in a modern network. It suggests four functional layers of these communication links:

- 1 . **Network Access Layer**: This layer defines how the data is physically transferred. It includes how hardware sends data bits through physical wires or fibers.    

    - A. **Ethernet:**
        - Ethernet is a widely used protocol for local area networks (LANs). It operates at the physical and data link layers of the OSI model.
        - Ethernet uses CSMA/CD (Carrier Sense Multiple Access with Collision Detection) to manage access to the network medium. Devices on the network listen for a clear channel before transmitting to avoid collisions.

     - B. **Wireless LAN (Wi-Fi):**
        - Wi-Fi protocols define wireless communication in local area networks. Standards include 802.11a, 802.11b, 802.11g, 802.11n, 802.11ac, and 802.11ax.
        - Wi-Fi provides wireless connectivity, with variations in speed, frequency, and range. Different standards offer improvements in performance and support for various applications.
    - C. **Bluetooth:**
        - Bluetooth is a short-range wireless communication standard for connecting devices like smartphones, laptops, and peripherals.
        - Bluetooth is known for low power consumption, short-range communication, and support for different profiles such as audio streaming and data transfer.

- 2 . **Internet Layer**: This layer is responsible for packaging the data into understandable packets and allowing it to be sent and received.

    - A. **Internet Protocol (IP):**
        - IP is fundamental for routing data across networks, assigning unique addresses to devices and handling packet routing.
        - IPv4 and IPv6 are the main versions. IPv6 addresses the limitations of IPv4, providing a larger address space to accommodate the growing number of devices on the internet.

    - B. **Internet Control Message Protocol (ICMP):**
        - ICMP is used for error reporting and diagnostics, working alongside IP to provide feedback on network issues.
        - ICMP is commonly used for tools like ping to test network connectivity by sending echo request messages and receiving echo replies.

- 3 . **Transport Layer**: This layer enables devices to maintain a conversation by ensuring the connection is valid and stable.

    - A. **Transmission Control Protocol (TCP):**
        - TCP provides reliable, connection-oriented communication, ensuring data integrity and order during transmission.
        - TCP employs a three-way handshake for connection establishment, flow control to manage data flow between sender and receiver, and error recovery mechanisms.

    - B. **User Datagram Protocol (UDP):**
        - UDP is a connectionless protocol, offering a faster but less reliable alternative to TCP, commonly used for real-time applications.
        - UDP does not establish a connection or provide error recovery. It is suitable for applications where some data loss is acceptable, such as streaming and online gaming.

- 4 . **Application Layer**: This layer defines how high-level applications can access the network to initiate data transfer.

    - A. **Hypertext Transfer Protocol (HTTP):**
        - HTTP is used for transmitting hypertext content on the web, facilitating communication between web clients and servers.
        - HTTP is a stateless protocol, often used in combination with secure variants like HTTPS for encrypted communication.

    - B. **File Transfer Protocol (FTP):**
        - FTP is a protocol for transferring files between computers on a network.
        - FTP supports various modes (e.g., active, passive), providing flexibility in data transfer. It allows users to upload and download files between a local and a remote system.

    - C. **Simple Mail Transfer Protocol (SMTP):**
        - SMTP is used for sending emails between servers, defining how email messages should be transmitted over the internet.
        - SMTP works in conjunction with other protocols like POP (Post Office Protocol) and IMAP (Internet Message Access Protocol) for email retrieval.
        
     - D. **Secure Shell (SSH):**
         - SSH is a protocol for secure remote access and control over a network, providing a secure channel for data communication.
         - SSH encrypts data during transmission, enhancing security. It is commonly used for secure access to servers and remote administration.


## OpenSSH
SSH, which stands for Secure Shell, is a cryptographic network protocol used to securely communicate over an unsecured network. It is commonly used for remote access to servers and other devices, allowing users to log in and execute commands remotely. SSH provides strong encryption and authentication mechanisms, making it suitable for securing network communications.

## Key Features

1. **Encryption**: SSH encrypts all data transmitted between the client and server, including passwords, commands, and data. This encryption helps protect sensitive information from being intercepted by malicious actors.

2. **Authentication**: SSH supports various authentication methods, including passwords, public key cryptography, and more advanced methods like multi-factor authentication. Public key authentication is commonly used for its enhanced security benefits.

3. **Secure Remote Access**: SSH enables users to securely access remote systems and execute commands as if they were directly interacting with the system locally. This feature is particularly useful for system administration and remote troubleshooting.

4. **Port Forwarding**: SSH supports port forwarding, allowing users to securely tunnel network connections over the encrypted SSH session. This feature is often used to bypass firewalls or securely access services hosted on remote machines.

5. **SFTP and SCP**: SSH includes protocols like SFTP (SSH File Transfer Protocol) and SCP (Secure Copy Protocol) for securely transferring files between systems. These protocols provide encryption and authentication, ensuring secure file transfers over the network.

6. **Tunneling**: SSH can be used to create secure tunnels between two hosts, allowing traffic to be securely routed through an encrypted connection. This feature is commonly used to secure connections to services such as databases or web servers.

### Techniques Used in SSH
There are majorly three major techniques used in SSH, which are

1. **Symmetric Cryptography**: In Symmetric key cryptography the same key used for encrypting and decrypting the message, a unique single shared key is kept between the sender and reciever. For ex: DES (Data Encryption Standard) and AES (Advanced Encryption Standard).

2. **Asymmetric Cryptography**: In Asymmetric key cryptography the key used for encrypting is different from the key used for decrypting the message. For ex: RSA (Rivest–Shamir–Adleman) and Digital Signature Algorithm.

3. **Hashing**: Hashing is a procedure used in cryptography which convert variable length string to a fixed length string, this fixed length value is called hash value which is generated by hash function.

### Components of SSH
The SSH (Secure Shell) protocol enables secure communication between two systems over an insecure network. The SSH protocol defines two main components: the SSH client and the SSH server. 

#### SSH Client

1. **Initiates Connection**: The SSH client is responsible for initiating the connection to a remote SSH server. It sends a request to connect to the server.

2. **Authentication**: Once the connection is established, the SSH client handles the authentication process. This involves proving the identity of the client to the server, typically using one of the following methods:

    A.**Password Authentication**: The client provides a password to authenticate itself to the server.

    B. **Public Key Authentication**: The client presents a cryptographic key pair, consisting of a public key and a private key. The server verifies the client's identity using the public key, and the client proves ownership of the private key.

3. **Secure Communication**: After successful authentication, the SSH client encrypts all communication with the server, ensuring confidentiality and integrity of data transmitted between the client and the server.

4. **Command Execution**: The SSH client allows the user to execute commands on the remote server securely. It sends the commands to the server and retrieves the output.

5. **File Transfer**: Some SSH clients support secure file transfer protocols such as SFTP (SSH File Transfer Protocol) or SCP (Secure Copy Protocol), allowing users to transfer files between the local system and the remote server.

#### SSH Server

1. **Listens for Connections**: The SSH server runs on a remote system and listens for incoming SSH connection requests from clients. It listens on a designated port (usually port 22 by default).

2. **Authentication**: Upon receiving a connection request, the SSH server verifies the identity of the client attempting to connect. It supports various authentication methods, including:

    A. **Password Authentication**: The server prompts the client to provide a password.

    B. **Public Key Authentication**: The server verifies the client's identity using the public key presented during the connection attempt.

3. **Secure Communication**: Once the client is successfully authenticated, the SSH server establishes a secure channel for communication with the client. All data transmitted between the client and the server is encrypted to prevent eavesdropping or tampering.

4. **Session Management**: The SSH server manages the client sessions, including executing commands requested by clients, managing file transfers, and handling other interactions with the client.

5. **Access Control**: The SSH server enforces access control policies to determine which clients are allowed to connect and what actions they are permitted to perform on the server. This may include user authentication, IP address whitelisting/blacklisting, and other security measures.


### Installing SSH

#### Installing SSH Client

1. **Update and Upgrade `apt` Package Manager**
```
sudo apt-get update -y && sudo apt-get upgrade -y
```

2. **Install SSH Client**
```
sudo apt install openssh-client
```

### Install SSH Server

1. **Update and Upgrade `apt` Package Manager**
```
sudo apt-get update -y && sudo apt-get upgrade -y
```
2. **Installing SSH Server**
```
sudo apt install openssh-server
```

### Managing SSH Service

1. **Starting SSH Client Services**
```
systemctl start ssh
```
2. **Starting SSH Server Services**
```
systemctl start sshd
```
3. **Stop SSH Client Services**
```
systemctl stop ssh
```
3. **Stop SSH Server Services**
```
systemctl stop sshd
```

### Conneting to Remote Server: Using Password Authentication

1. If Remote Server SSH is Runing on Default Port 22
```
ssh user_name@remote_serer_ip_address
```
- Enter Remoter Server Password to Authenticate when prompted to Enter Password.

2. If Remote Server SSH is not Runing on Default Port 22
```
ssh -p port_number user_name@remote_server_ip_address
```
- Enter Remoter Server Password to Authenticate when prompted to Enter Password.

**NOTE**: Using Aliases to Simplify Connection
- To simplify the SSH connection process, you can utilize host aliases in your SSH configuration file.

    A. **Access SSH Configuration File**
    ```
    nano ~/.ssh/config
    ```
    B. **Define Host Alias of Remote Server in `config` File and Save `config` File**
    ```
    Host Alias
         HostName IP_Address
         Port Port_Number
         User User_Name
    ```
    C. **Establish Connection Using Alias**
    ```
    ssh Alias
    ```

### Conneting to Remote Server: Using Public Key Authentication

1. **Generate SSH Key**
```
ssh-keygen
```
2. **Make Connection to Remote Server Using Password Authentication**
```
ssh user_name@remote_serer_ip_address
```
3. **Copy and Paste SSH Public Key to the Remote Server**
- Paste the Newly Generated SSH Public Key form Local Server in Remote Servers's `.ssh/authorized_keys` File.

**OR**

1. **Generate SSH Key**
```
ssh-keygen
``` 
2. **Paste the the Newly Gerenrated SSH Publik Key on Remote Server**
```
ssh-copy-id -i ~/.ssh/id_rsa.pub -p port_number user_name@ip_address
```

### Generating SSH Key
- **To generate SSH Key of Type **`RSA`** Incription with Custom Lableing**
```
ssh-keygen -t rsa -b 4096 -C "custom_lable"
```
- **`ssh-keygen`**: This is the command-line tool used to generate SSH keys.
- **`-b 4096`**: This flag sets the number of bits in the key to 4096, making it a high-security key due to its larger size.
- **`-C "custom_label"`**: This flag adds a comment to the key. In this case, the comment is "custom_label", which can help identify the key later if you have multiple keys.

- **To Generate SSH Key of Type **`ECC`** Incription with Custom Lableing**
```
ssh-keygen -t ed25519 -C "custom_name"
```
- **`ssh-keygen`**: This is the command-line tool used to generate SSH keys.
- **`-t ed25519`**: This flag specifies the type of key to create, in this case, Ed25519. Ed25519 is a type of elliptic curve cryptography (ECC) which provides strong security with relatively small key sizes.
- **`-C "custom_label"`**: This flag adds a comment to the key. In this case, the comment is "custom_label", which can help identify the key later if you have multiple keys.

A. **Choose the File Location**: When prompted, you can press Enter to accept the default file location or specify a different location. If a key already exists in the default location, it will be overwritten, potentially causing issues if it's being used elsewhere. To avoid this, you can specify a different location to save the key.

B. **Choose a Passphrase(Optional)**: You can choose to use a passphrase for additional security. It's not mandatory, but it's highly recommended.

**NOTE**
- You can verify that the keys were generated successfully by navigating to the directory where they were created and you should see id_rsa or custom_name (your private key) and id_rsa.pub or custom_name.pub (your public key) listed.
- The `ssh-keygen` command will generate `SSH Key Pair`. It will create two files: `Public Key` (id_rsa.pub or custom_name) and `Private Key` (id_rsa or custom_name.pub). The private key should be kept secure and never shared, while the public key can be distributed to servers you wish to access securely. 

### SSH Configuration

#### SSH Server Configuration

**Location: /etc/ssh/sshd_config**

1. **Port**: Specifies the port on which the SSH server listens for connections. Default is 22.
```
Port 22
```
2. **PermitRootLogin**: Controls whether root can log in directly using SSH. It's advisable to set this to no for security reasons.
```
PermitRootLogin no
```
3. **PasswordAuthentication**: Specifies whether password authentication is allowed for SSH connections. It's recommended to set this to no and use key-based authentication.
```
PasswordAuthentication no
```
4. **AllowUsers**: Specifies which users are allowed to connect via SSH. Only listed users will be permitted.
```
AllowUsers user1 user2
```
5. **PubkeyAuthentication**: Specifies whether public key authentication is allowed. It's recommended to set this to yes.
```
PubkeyAuthentication yes
```
6. **AllowTcpForwarding**: Specifies whether TCP forwarding is permitted. Default is usually yes.
```
AllowTcpForwarding yes
```

#### SSH Client Configuration

**Location: /etc/ssh/ssh_config**

1. **Host**: Defines configurations for specific hosts.
```
Host Alias
     HostName IP_Address
     Port Port_Number
     User User_Name
```
2. **IdentityFile**: Specifies the file from which the user's identity (private key) is read.
```
IdentityFile ~/.ssh/id_rsa
```
3. **ServerAliveInterval**: Sets a timeout interval in seconds after which if no data has been received from the server, SSH will send a message through the encrypted channel to request a response from the server.
```
ServerAliveInterval 60
```
4. **Compression**: Specifies whether to use compression. It's often beneficial to enable this to speed up data transfer, especially over slower connections.
```
Compression yes
```
5. **ForwardX11**: Specifies whether X11 forwarding is permitted. Default is usually no.
```
ForwardX11 yes
```

### SSH Logs
SSH logs typically contain records of login attempts, authentication failures, and other SSH-related activities on a system. These logs are crucial for monitoring and troubleshooting SSH access to a server. 
```
tail -n 50 /var/log/auth.log
```

## Network Defense
While nodes, links, and protocols form the foundation of a network, a modern network cannot exist without its defenses. Security is critical when unprecedented amounts of data are generated, moved, and processed across networks. A few examples of network defense tools include Firewall, Intrusion Detection Systems (IDS), Intrusion Prevention Systems (IPS), Network Access Control (NAC), Content Filters, Proxy Servers, Anti-DDoS Devices, and Load Balancers.

## Computer Network Utilities
Computer network utilities are software tools and applications designed to help manage, monitor, analyze, and troubleshoot computer networks. These utilities play a crucial role in ensuring the smooth operation and optimal performance of network infrastructure. 

### Common Computer Network Utilities

1. **Ping:** The Ping utility is used to test the reachability of a host on an Internet Protocol (IP) network. It sends a small packet of data to the target host and measures the round-trip time for the packet to travel from the source to the destination and back.

2. **Traceroute/Tracepath:** These utilities help to trace the route that packets take from the source to the destination. They provide information about each hop along the way, showing the IP addresses and response times for each intermediate device.

3. **Network Scanners:** Tools like Nmap or Angry IP Scanner are used to discover devices on a network and identify open ports and services running on those devices. They are essential for network reconnaissance and security auditing.

4. **Wireshark (Network Protocol Analyzer):** Wireshark is a powerful tool for capturing and analyzing network packets. It allows users to inspect the data in real-time or analyze saved capture files. Wireshark is commonly used for troubleshooting network issues and monitoring network traffic.

5. **Netstat(ns):** This command-line tool provides information about network connections, routing tables, interface statistics, masquerade connections, and more. It is available on most operating systems and helps in monitoring network activities.

6. **Netcat(nc):** Netcat is a versatile networking utility that can be used for reading and writing data across network connections. It's often used for debugging, port scanning, and transferring files.

7. **ipconfig/ifconfig:** These commands (ipconfig for Windows and ifconfig for Unix-based systems) provide information about the network interfaces on a computer, including IP addresses, subnet masks, and MAC addresses.

8. **DNS Lookup Tools:** Utilities like nslookup or dig help in querying Domain Name System (DNS) servers to obtain information about domain names, IP addresses, mail exchangers, and name servers.

9. **Bandwidth Monitoring Tools:** Applications like iperf or bandwidth monitoring tools help in measuring the available bandwidth between two network endpoints, aiding in network performance analysis.

10. **Firewall and Security Utilities:** Tools like iptables (for Linux) or Windows Firewall (for Windows) help in configuring and managing network security policies.

11. **Remote Desktop Utilities:** Tools like Remote Desktop Protocol (RDP) or Virtual Network Computing (VNC) allow users to connect to and control remote computers over a network.