<h1 align='center'>Computer Networking</h1>

**Note :**
This documentation is made from [Kunal Kushwaha's Computer Networking course](https://www.youtube.com/watch?v=IPvYjXCsTg8) and resources from the Internet.

<h2 align='center'><i><u>Introduction</i></u></h2>

**Computer Network -** 
Computers connected together is a computer network.

**Internet -**
The system of interconnected computers on a global scale, is called the Internet.

<h2 align='center'><i><u>How Internet Was Developed?</i></u></h2>

The cold war was going on between United States and the Soviet Union. The soviet union won in launching their first satelite, Sputnik 1 in 1957. The US Government then created a program called as ARPA (Advanced Research Projects Agency). They wanted to have a system of communication to communicate between the other buildings of the ARPA spread around the US. So, they created the ARPANET (The Advanced Research Projects Agency Network) which connected the MIT (Massachusetts Institute of Technology), Stanford University, UCLA (University of California, Los Angeles) and University of Utah. They used TCP/IP (Transmission Control Protocol) in the ARPANET. As time went by, more and more computers were connected. There was no way to automatically share the linked documents. Now, WWW (The World Wide Web) came up, which was developed by Timothy Berners-Lee. This project stored the documents and could be accessed across the web. Here's the [world's first website](http://info.cern.ch/hypertext/WWW/TheProject.html). But, there's no search engines. Now, search engines have been developed. The [Internet Society](https://www.internetsociety.org/) is responsible for maintaining the Internet.

<h2 align='center'><i><u>IP Address</i></u></h2>

Every device which can connect to each other, have their own IP Addresses. It is in the format of " **X.X.X.X** ". Every single "X" can have value from **0** to **255**. When we write [google.com](https://www.google.com/) in the address bar, it resolves to the IP address of Google. 
</br>
To get your IP Address, type -

1. For **Windows** :

        ipconfig
    
    in the command prompt.

2. For **Mac** :
    
        $ curl ifconfig.me

    in the terminal.

Internet Service Provider (ISP) gives you a modem/router which has a global IP Address. The modem will then give IP Addresses to each of the device connected, and those IP Addresses are called Local IP Address using the DHCP (Dynamic Host Configuration Protocol).

When we request a server (Google server in this case), it can see the global IP Address and not the Local IP Address. It sends the response and the modem/router decides which device to send back the response, using NAT (Network Address Translation) Protocol. **IP Adddress** decides which device to send the data and **Port Number** determines which application requested the data. 

<h2 align='center'><i><u>Port Numbers</i></u></h2>
What it means by Network speed?
Suppose you are having an internet speed of -
- 1 mbps = 10<sup>6</sup> bits/second.
- 1 gbps = 10<sup>9</sup> bits/second.
- 1 kbps = 10<sup>3</sup> bits/second.

When we send data to another computer through the internet, it is called as **upload**.
When someone sends data to youand you recieve that, it is called as **download**. 

<h2 align='center'><i><u>Data Transmission</i></u></h2>

Data transmission happens in two ways -
- The Guided Way (where path is defined) - *Example -* wired connections between computers.
- The Unguided Way (where path is not defined) - *Example -* Wi-Fi, Bluetooth, etc.

There are submarine cables lied in the oceans and waterbodies, connecting various places around the world. You can checkout the [submarine cable map website](https://www.submarinecablemap.com/).

![submarine cable map website](https://cdn.hashnode.com/res/hashnode/image/upload/v1653998279577/pjYpnHM1r.jpeg)

**Wired Connection -** Optical Fibre cables, coaxial cable </br>
**Wireless connection -** Bluetooth, Wi-Fi, 3G, 4G, LTE, 5G

<h2 align='center'><i><u>LAN, MAN and WAN</i></u></h2>

- **LAN** *(Local Area Network)* - small area coverage. Wifi and Ethernet are it's examples.
- **MAN** *(Metropolitan area network)* - Accross a city.
- **WAN** *(Wide Area network)* - Accross countries. Optical Fibre Cables are used.

    1. **SONET** *(Synchronous Optical Network)* - It carries the data using optical fibre cables, hence, it can carry data for large distances.
    2. **Frame Relay** - It connects all the Local Area Network with the Wide Area Network.

<h2 align='center'><i><u>Modem, Router and DNS</i></u></h2>

**Modem** - It is a device which converts the digital signals into analog signals and vice-versa. *Example -* it will convert the digital image in your computer into electrical signals (Analog Signals) which is transmitted over wires(for example).

**Router** - It is a device which routes the data packets.

**DNS** *(Domain Name Server)* - It is a type of phonebook which converts the domain name into the registered IP Address of that domain.

There are also something like Tier-1 ISP , Tier-2 ISP, and so on.
In India, Tier-1 ISP is TATA, BSNL, etc.

<h2 align='center'><i><u>Topologies</u></i></h2>

1. **Bus Topology -** Bus topology is a network type in which every computer and network device is connected to a single cable.</br>
    **Advantages :**
    - If N devices are connected to each other in a bus topology, then the number of cables required to connect them is 1, which is known as backbone cable, and N drop lines are required.
    - The cost of the cable is less as compared to other topologies, but it is used to build small networks.  </br> 

    **Limitations :**
    - If the cable fails, the whole network crashes.
    - Only **one person** can send data at a time.
    - Data is transmitted from one end to another end in a **single direction**.
    - If the network traffic is heavy, it increases collisions in the network. To avoid this, various protocols are used in the MAC layer known as Pure Aloha, Slotted Aloha, CSMA/CD, etc. </p>

    ![Bus Topology Diagram](https://thumbs.dreamstime.com/b/bus-topology-diagram-29007878.jpg) <p>

2. **Ring Topology -** Ring Topology is a network type in which each computer is connected to the next in a circular way.</br>
    **Advantages :**
    - The possibility of collision is minimum in this type of topology.
    - Cheap to install and expand.</br>

    **Limitations :**
    - If one of the cable breaks, then the whole network crashes.
    - Lot of unnecessary calls are made.  <p>  

    ![Ring Topology Diagram](https://www.networkstraining.com/wp-content/uploads/2018/10/ring-topology.jpg) <p>

3. **Star Topology -** The star topology is a network type in which all computers are connected through a central device.</br>
    **Advantages :**
    - Star topology systems are highly scalable.
    - Multiple devices can be connected through the star topology.</br>
    
    **Limitations :**
    - If the central device fails, the whole network will crash.
    - Performance is based on the central device.
    - Star topology is very expensive to install. <p>
    
    ![Star Topology Diagram](https://i2.wp.com/hmhub.me/wp-content/uploads/2019/08/star-Topology.jpg?fit=1200%2C600&ssl=1) <p>

4. **Tree Topology -** The Tree Topology is a network type where many star topologies are connected using a bus topology.</br>
    **Advantages :**
    - It allows more devices to be attached to a single central hub thus it decreases the distance that is traveled by the signal to come to the devices.
    - It has higher [fault tolerance](https://www.imperva.com/learn/availability/fault-tolerance/).</br>
    
    **Limitations :**
    - A tree topology relies heavily on its main bus cable.
    - The installation of a tree topology is difficult.<p>

    ![Tree Topology Diagram](https://image.slidesharecdn.com/dc-lec-03topologies-150513143944-lva1-app6892/95/dc-lec03-topologies-34-638.jpg?cb=1431528194) <p>

5. **Mesh Topology -** The Mesh Topology is a network type where each and every computers are connected to each other. </br>
    **Advantages :**
    - Failure of one single device does not affect the network.
    - Adding new devices does not affect data transmission.</br>
    
    **Limitations :**
    - Expensive.
    - Time-consuming to build and maintain.
    - High risk of redundant connection. <p>

    ![Mesh Topology Diagram](https://techprojournal.com/wp-content/uploads/2020/08/mesh-topology-1-696x348.jpg) <p>

<h2 align='center'><i><u>Structure Of The Network</u></i></h2>

**Here's an example to understand the network :**
You order for something on Amazon US, they recieves your order and ships your order to the delivery company of US. Then it is transported and it has arrived India. It is sent to the delivery company who then sends the order to you.

<h2 align='center'><i><u>How The Internet Works?</u></i></h2>

- <h3 align='left'><b>OSI Model :</b></h3>
    The OSI Model stands for Open Systems Interconnection Model. It was developed as a standard of how people and computers interact. There are 7 layers in the OSI Model ~

    - **Application Layer** - It is implemented in softwares. Users will send the data to the software in this layer. Protocols used here include HTTP, FTP, Telnet etc.
    - **Presentation Layer** - The data is translated into machine representable binary code. This is known as **translation**. The data goes under encoding, compression and encryption. It also provides abstraction. Here, SSL (Secure Socket Layer) protocol is used.
    - **Session Layer** - The Session Layer helps in setting up and managing the connections. It enables the sending and recieving of data followed by termination of connected sessions. Authentication is done in this layer. Then, authorization (Checking whether you have the permission to access any resource on the server) is done.
    - **Transport Layer** - UDP and TCP Protocol is used in this layer. The transport layer transports the data in three ways -
        - **Segmentation :** The data recieved from the session layer, is segmented. Every segment of the data will contain the sender's and reciever's port numbers, and the sequence numbers. Sequence number helps to reassemble the data in the correct order. 
        - **Flow Control :** The transport layer controls the amount of data that is transmitted.
        - **Error Control :** It checks whether the data is corrupted or missing or not using **checksums** attached to each data packets. 

        **Connection-oriented service** and **connectionless service** takes place at the **reciever's end** in this layer.
    - **Network Layer** - It is responsible for the transmission of the data from one computer to another computer that is located in a different network. Here, router is present. The function of network layer is **Logical addressing**. Logical addressing is the assigning of sender's and reciever's IP Address to each of the data segments and it forms an **IP Packet**, so that all the data packets can reach the correct destination. It performs **routing** which is the movement of the data packet from source to destination. Load balancing also happens here.
    - **Data Link Layer** - It helps to directly communicate with the computers. Physical Addressing happens here. It is the assigning of MAC Address of the sender and reciever's device to the data packets, forming **frames**. MAC address is a 12 digit alphanumeric number of the network interface of your device. It also controls how the data is recieved using Media Access Control.
    - **Physical Layer** - This is the hardware layer which transports the data through wires to the reciever.<p>

    ![OSI Model](https://miro.medium.com/max/1200/1*17Zz6v0HWIzgiOzQYmO6lA.jpeg) <p>

<h2 align='center'><i><u>Client-Server Architecture</i></u></h2>

When we write [google.com](https://www.google.com/) in the address bar of the browser, our device sends a request to the google server which sends back a response.
Server is a system that controls the website you are hosting. There are processes running on client and server which communicate with each other.
Client are the people who requests for something on the server.
Collection of huge number servers in a company on a global scale is called a data centre. It might have static IP Address and has high upload speed. 
Ping measures the round-trip time from the client to the server and back to it.

<h2 align='center'><i><u>Peer To Peer (P2P) Architecture</i></u></h2>

Applications running on various devices get connected to each other, and there is no large server or data centre. *For Example* - In college, computers can be connected to each other without having a dedicated server. It is a decentralized network.
The advantage is it is easily scalable. *Example* - BitTorrent.
It might have centralized database as well.

<h2 align='center'><i><u>Network Devices</i></u></h2>

There are lots of devices which are use to communicate with devices these devices
called Networking Devices. There are **Internal**, **External** and **Portable** Devices.

**Internal Devices** :
- Network interface controller (NIC)
- Wireless Network Interface Controller
- Bluetooth Dongle

**External Devices**
- Hub
- Switches
- Routers
- Brouters
- Bridges
- Repeater
- Modem
- Gateway
- WIFI-Routers or Broadband Routers

**Portable Devices**
- WIFI-Hotspot
- Portable Modem Dongle <p>

Here is those devices in details :
1. <u>**Repeater**</u> - Repeater is use to extend the range of radio signal so that the signal can cover longer distances. **A repeater is an electronic device that receives a signal and re transmits it**. **It does not amplify the signal**. Repeater is used for wired medium (example - telephone line repeater, fiber optical cable repeater etc.) as well as wireless medium (example - satellite repeater, microwave repeater, wifi repeater, LTE repeater etc.).

    **Types of Repeater** :
    - Analog Repeater
    - Digital Repeater
    - Microwave Repeater
    - Satellite Repeater
    - WiFI Repeater | WLAN Repeater
    - LTE Repeater
    - Optical Repeater <p>
    
    ![Repeater](https://th.bing.com/th/id/R.7a67341a896ba87e216748a90b8732c2?rik=m3CPQ1%2bPq7doPA&riu=http%3a%2f%2fd1unzhqf5a606m.cloudfront.net%2fimages%2flarge%2fhoneywell-wrex-wifi-repeater-extender.png%3f1389738305&ehk=LlBNJN1QOEwZQU1qEoYw%2bEnut%2bOG0hZ3WwEIZXhZibE%3d&risl=&pid=ImgRaw&r=0)

2. <u>**Modems**</u> - Modems are electronic devices which convert digital information of computers into analog signals and are also capable of again converting the analog signals to the digital information at the receiving end. Modems can be classified in various ways. Some of the common types include - **half-duplex modem**, **full-duplex modem**, **2-wire modem**, **4-wire modem**, **synchronous** and **asynchronous modem**.
Modem stands for **Modulator and Demodulator device** which assists computer in transferring data and information over telephone lines. This is done by changing the **digital data into
analog signal** which can be transferred over the phone lines. In the receiver end, it again **converts the analog signal into the digital data**. Therefore simply, it acts as a modulator when it converts digital data into analog signal and it works as a demodulator when it converts analog signal to digital data.
There are modems having **Asymmetric digital subscriber line (ADSL)** and some not supporting ADSL (identified with DSL led blinker on panel).

    **Types of Modems :** 
    - based on location
        - Onboard Modem
        - Internal Modem
        - External Modem
        - Removable Modem

    - based on its working
        - Half duplex Modem
        - Full Duplex Modem
        - 2 wire modem
        - 4 wire modem
        - Synchronous Modem
        - Asynchronous Modem <p>

    ![Modem](https://www.samm.com/userfiles/editor/image/optical-modem-gpon-fk-ont-g400b-poe-s2-furukawa-2.png)


3. <u>**Gateway**</u> - A gateway is not a hardware device. It is **software firmware** which saves the **configuration setting of a device**. Mostly the gateway address in routers is **192.168.0.1** or **192 168.1.1**.
Its acts as a "**gate**" between two networks. It may be a router, firewall, server, or other device that enables traffic to flow in and out of the network. While a gateway protects
the nodes within network, it itself is also a node.

    ![Gateway](https://5.imimg.com/data5/JA/YO/MY-10051435/industrial-iot-gateway-with-lora-500x500.png)

4. <u>**WIFI-Routers**</u> - Similar to a modem with the additional feature of Wireless connectivity called as "WIFI ".It generally has 4 ethernet ports and it is having routing DHCP to connect 240 pc and devices providing internet with wired and wireless options.
    ![WiFi Router](https://www.netgear.com/images/Products/Networking/WirelessRouters/R6230/R6230_Hero_Transparent.png)

5. <u>**Hubs**</u> - It is basically a multiport hub. A hub is a device to which all the devices sharing a physical network can be physically connected to form a "Local Area Network" or "LAN". Hubs enable the electric currents from a computer to pass to all other devices connected to it. Since a hub was the electronic equivalent of shouting in a room as necessary, as the number of devices increased, the number of collisions increased and LAN performance ground to a hault. In a hub-centric environment, the message packets being sent by each device that is connected to the hub can be "seen" by every other
device on the hub whether they are involved in the conversation or not. So, hubs can facilitate message eavesdropping.

    **Types of Hub** :
    - **Active Hub** :- These are the hubs which **have their own power supply** and can **clean , boost and relay the signal** along the network. It serves **both as a repeater as well as wiring center**. These are used to **extend maximum distance between nodes**.
    - **Passive Hub** :- These are the hubs which **collect wiring from nodes** and **power supply from active hub**. These hubs **relay signals** onto the network **without cleaning and boosting them** and **can't be used to extend distance between nodes**.
    - **Intelligent Hubs** :- An intelligent hub can help in **troubleshooting by pinpointing** the actual location of the problem and help **identify the root cause and resolution**. It is **very adaptable to different technologies without any need to change its configuration**. The intelligent hub performs different functions such as **bridging, routing, switching and network management**.

    ![Hub](https://eu.dlink.com/uk/en/products/-/media/product-pages/dub/h7/g1/dubh7g1image-lfrontpowerlight.png)

6. <u>**Switches**</u> - A switch serves as a controller, enabling networked devices to talk to each other
efficiently. A switches use to connect computers, printers, phones, cameras, lights, and servers in a building or campus.

    **Types of Switches** :
    - **Unmanaged switches** :- An unmanaged switch works right out of the box. It's not designed to be configured. so you don't have to worry about installing or setting it up correctly. Unmanaged switches have fewer features and less network capacity than managed switches. You'll usually find unmanaged switches in home networking equipments.

    - **Managed switches** :- A managed network switch is configurable, offering greater security, flexibility and capacity than an unmanaged switch. You can monitor and adjust a managed switch locally or remotely, to give you greater network control.

        ![Switch](https://hw-egypt.com/wp-content/uploads/2017/11/1450367494000_1204486.png)

7. <u>**Routers**</u> - When a device in a Local Area Network needs to communicate with a device on another LAN, it must send that traffic to a specialized device connected to the LAN called a "router" whose purpose is to find the best path for the message to take to arrive at the intended target device, and to send the message along its way following that path.

    In order to allow the billions of devices on the Internet to find each other, routers regularly need to communicate among themselves using protocols that enable them to share routing information so that, when a device needs to send a communication message to a target device, the routers work together to determine the best path for the message packet to use to arrive at the intended target device.
    
    Each router port is configured with a specific routing protocol that is associated with that port's function. For example, a router port that connects to the Internet must learn how to efficiently route communication messages to destinations around the world. Protocols that facilitate this are called **"gateway routing protocols"** and have names such as the **Border Gateway Protocol ("BGP")** or **Exterior Gateway Protocol ("EGP")**. A router port that connects to an organization's internal networks must learn how the organization's network is configured to efficiently route traffic throughout the organization. Protocols that serve this purpose are called **"interior routing protocols"** and have names such as **Enhanced Interior Gateway Routing Protocol ("EIGRP")**, **Interior Gateway Routing Protocol ("IGRP")**, **Open Shortest Path First (OSPF")**, **Routing Information Protocol I and II ("RIP" /"RIP II")**, etc.

    **Types of Routers** :
    - Broadband Routers
    - Wireless Routers
    - Edge Router
    - Subscriber Edge Router
    - Inter-provider Border Router
    - Core Router

    ![Router](https://www.netgear.com/images/Products/Networking/WirelessRouters/R6230/R6230_Front_Transparent.png)

8. <u>**Brouter**</U> - It is also known as bridging router which is a device which combines features of both bridge and router. It can work either at data link layer or at network layer. Working as router, it is capable of routing packets across networks and working as bridge, it is capable of filtering local area network traffic.
    
    A bridge router or brouter is a network device that works as a bridge and as a router. The brouter routes packets for known protocols and simply forwards all other packets as a bridge would. 

    Brouters operate at both the network layer for routable protocols and at the data link layer for non-routable protocols. As network continue to become more complex, a mix of routable and non-routable protocols has led to the need for the combined features of bridges and routers.Brouters handle both routable and non-routable features by acting as routers for routable protocols and bridges for non-routable protocols.
    
9. <u>**Bridge**</u> - A network bridge device is primarily used in local area networks because they can potentially flood and clog a large network, thanks to their ability to broadcast data to all the nodes if they don't know the destination node's MAC address.
    
    A bridge is a type of computer network device that provides interconnection with other bridge networks that use the same protocol.
    
    Bridge devices work at the data link layer of the Open System Interconnection (OSI) model, connecting two different networks together and providing communication between them. Bridges are similar to repeaters and hubs in that they broadcast data to every node. However, bridges maintain the Media Access control (MAC) address table as soon as they discover new segments, so subsequent transmission are sent only to the desired recipient.
    
    A bridge uses a database to ascertain where to pass, transmit or discard the data frame.

    1. If the frame received by the bridge is meant for a segment that resides on the same host network, it will pass the frame to that node and the receiving bridge will then discard it.

    2. If the bridge receives a frame whose node MAC address is of the connected network, it will forward the frame toward it.

- <h3 align='left'><b>TCP/IP Model :</b></h2>
    This model was developed by ARPA. There are 5 layers in this model ~

    1. **<u>Application Layer</u>** - Users interact with this. Whatsapp, browsers etc. lie here. It is on your devices.
        - ***Application Layer Network Protocols*** : Protocols are set of rules used in the internet. The Protocols which are commonly used in the Application Layer are given below.
            - **DNS (Domain Name System protocol)** - The DNS protocol helps in **translating or mapping host names to IP addresses**. DNS works on a **client-server model**, and uses a **distributed database** over a hierarchy of name servers. When we visit a website for the first time, the IP Address of the website is stored in the local cache. Suppose, the IP Address is not found in the local cache, then it will be looked in the local DNS Server (ISP has all info about all websites you visit even if in incognito mode) which is the first point of contact. If the IP Address is not found there, it will be looked for in the root server and if not found even, it will be looked in the top-level domain. After getting the IP, the website server is connected.


                <u>**Classes of Domains**</u>

                ![Part/Class of Domain](https://searchfacts.com/wp-content/uploads/2019/07/domain-name-parts.png)

                - **Top-level domain** - Root DNS Servers. They have top-level domains like .io, .org, .com, etc. The authorities maintaing this root DNS server can be seen in this website - [Root-servers.org](https://root-servers.org/). The top-level domains are registered by [ICANN](https://www.icann.org/) (The Internet Corporation for Assigned Names and Numbers).

                - **Second level Domain** - The top-level domains themselves have domains like student.io, commclassroom.org, google.com, etc.

                Hosts are identified based on their IP addresses, but memorizing an IP address is difficult due to its complexity. IPs are also dynamic, making it all the more necessary to map domain names to IP addresses. DNS helps resolve this issue by **converting the domain names of websites into numerical IP addresses**.

                <u>**Advantages :**</u>

                    • DNS facilitates internet access.
                    • Eliminates the need to memorize IP addresses.

                <u>**Disadvantages :**</u>

                    • DNS queries don't carry information pertaining to the client who initiated it. This is because the DNS server only sees the IP from where the query came from, making the server susceptible to manipulation from hackers.
                    • DNS root servers, if compromised, could enable hackers to redirect to other pages for phishing data.
            <p>

            - **FTP (File Transfer Protocol)** - File Transfer Protocol enables **file sharing between hosts, both local and remote**, and **runs on top of TCP**. For file transfer, FTP **creates two TCP connections: control and data connection**. 

                The control connection is used to **transfer control information like passwords, commands to retrieve and store files, etc.**, and the data connection is used to **transfer the actual file**. Both of these connections run in **parallel** during the entire file transfer process.

                <u>**Advantages :**</u>

                    • Enables sharing large files and multiple directories at the same time.
                    • Lets you resume file sharing if it was interrupted.
                    • Lets you recover lost data, and schedule a file transfer.

                <u>**Disadvantages :**</u>

                    • FTP lacks security. Data, usernames, and passwords are transferred in plain text, making them vulnerable to malicious actors.
                    • FTP lacks encryption capabilities, making it non-compliant with industry standards.
            <p>

            - **HTTP (Hyper Text Transfer Protocol)** - HTTP is an application layer protocol used for **distributed, collaborative, and hypermedia information systems**. It works on a **client-server model**, where the web browser acts as the client. Data such as text, images, and other multimedia files are shared over the World Wide Web using HTTP. As a request and response type protocol, the client sends a request to the server, which is then processed by the server before sending a response back to the client.

                HTTP is a **stateless protocol**, meaning the client and server are only aware of each other while the connection between them is intact. After that, both the client and server forget about each other's existence. Due to this phenomenon, the client and server **can't both retain information between requests**. 

                <u>**HTTP Methods**</u> - This tells the servers what to do.
                - GET : Requesting a data.
                - POST : Giving something to the server, like form data.
                - PUT : Puts data at a specific location in the server.
                - DELETE : It deletes a resource on the server. 

                <u>**Status Code**</u> - Status Code tells what happened to our request.

                - 1XX -> Informational.
                - 2XX -> Success codes.
                - 3XX -> Redirection purposes.
                - 4XX -> Client error.
                - 5XX -> Server error.

                <u>**Cookies**</u> - It is a file containing unique string stored in the client's browser. When a website is visited first, a cookie is set. Next time, whenever a new request is made to that website, the cookie will be set in the request headers.                    
                Third-party cookies : Cookies that are set for the URLs that you don't know.

                <u>**Advantages :**</u>

                    • Memory usage and CPU usage are low because of lesser concurrent connections.
                    • Errors can be reported without closing connections.
                    • Owing to lesser TCP connections, network congestion is reduced.

                <u>**Disadvantages :**</u>

                    • HTTP lacks encryption capabilities, making it less secure.
                    • HTTP requires more power to establish communication and transfer data.
            <p>

            - **IMAP and IMAP4 (Internet Message Access Protocol (version 4))** - IMAP is an **email protocol** that lets end users **access and manipulate messages** stored on a mail server from their email client as if they were present locally on their remote device. IMAP follows a **client-server model**, and **lets multiple clients access messages on a common mail server concurrently**. IMAP includes **operations for creating, deleting, and renaming mailboxes; checking for new messages; permanently removing messages; setting and removing flags**; and much more. The current version of IMAP is version 4 revision 1.

                <u>**Advantages :**</u>

                    • As the emails are stored on the mail server, local storage utilization is minimal.
                    • In case of accidental deletion of emails or data, it is always possible to retrieve them as they are stored on the mail server.

                <u>**Disadvantages :**</u>

                    • Emails won't work without an active internet connection.
                    • High utilization of emails by end users requires more mailbox storage, thereby augmenting costs.
            <p>

            - **POP and POP3 (Post Office Protocol (version 3))** - The Post Office Protocol is also **an email protocol**. Using this protocol, the end user can **download emails from the mail server to their own email client**. Once the emails are downloaded locally, they **can be read without an internet connection**. Also, **once the emails are moved locally, they get deleted from the mail server, freeing up space**. POP3 is **NOT designed to perform extensive manipulations with the messages on the mail server, unlike IMAP4**. POP3 is the latest version of the Post Office Protocol.

                <u>**Advantages :**</u>

                    • Read emails on local devices without internet connection.
                    • The mail server need not have high storage capacity, as the emails get deleted when they're moved locally.
                <u>**Disadvantages :**</u>

                    • If the local device on which the emails were downloaded crashes or gets stolen, the emails are lost.
            <p>

            - **SMTP (Simple Mail Transfer Protocol)** - SMTP is a protocol designed to **transfer electronic mail reliably and efficiently**. SMTP is a **push protocol** and is used to **send the email**, whereas **POP and IMAP are used to retrieve emails on the end user's side**. SMTP **transfers emails between systems, and notifies on incoming emails**. ***<u>Using SMTP, a client can transfer an email to another client on the same network or another network through a relay or gateway access available to both networks</u>***.

                <u>**How E-Mail works?**</u>

                For sending e-mail, SMTP protocol is used.
                Sender sends the e-mail to the sender's SMTP server. The e-mail stays the there for a while, then the sender's server connects to the reciever's SMTP server. This happens only when the sender and reciever are not using the same e-mail platform like only google, or only yahoo, etc. When the reciever logs in to the recievers client, the e-mail from the reciever's server is downloaded into the client which the reciever can view. For recieving e-mails, POP (Post Office Protocol) protocol is used. At first, the client authorizes with the reciever's POP server and then transact the e-mails. Later, the e-mails are updated. The folders like sent items and draft folder is NOT downloaded by POP. 

                <u>**Advantages :**</u>

                    • Ease of installation.
                    • Connects to any system without any restriction.
                    • It doesn't need any development from your side.

                <u>**Disadvantages :**</u>

                    • Back and forth conversations between servers can delay sending a message, and also increases the chance of the message not being delivered.
                    • Certain firewalls can block the ports used with SMTP.
            <p>

            - **Telnet (Terminal emulation protocol)** - Telnet is an application layer protocol that enables a user to **communicate with a remote device**. A Telnet client is installed on the user's machine, which **accesses the command line interface of another remote machine that runs a Telnet server program**.

                Telnet is mostly used by **network administrators to access and manage remote devices**. To access a remote device, a network admin needs to enter the **IP or host name of the remote device**, after which they will be presented with a **virtual terminal that can interact with the host**.

                <u>**Advantages :**</u>

                    • Compatible with multiple operating systems.
                    • Saves a lot of time due to its swift connectivity with remote devices.

                <u>**Disadvantages :**</u>

                    • Telnet lacks encryption capabilities and sends across critical information in clear text, making it easier for malicious actors.
                    • Expensive due to slow typing speeds.
            <p>

            - **SNMP (Simple Network Management Protocol)** - SNMP is an application layer protocol used to **manage nodes, like servers, workstations, routers, switches**, etc., on an IP network. SNMP enables network admins to **monitor network performance, identify network glitches, and troubleshoot them**. SNMP protocol is comprised of three components: a **managed device**, an **SNMP agent**, and an **SNMP manager**.

                The SNMP agent resides on the **managed device**. The agent is a **software module** that has local knowledge of management information, and **translates that information into a form compatible with the SNMP manager**. The SNMP manager presents the data obtained from the SNMP agent, helping network admins **manage nodes effectively**.

                Currently, there are **three versions** of SNMP: SNMP **v1**, SNMP **v2**, and SNMP **v3**. Both versions 1 and 2 have many features in common, but SNMP v2 offers enhancements such as additional protocol operations. **SNMP version 3 (SNMP v3) adds security and remote configuration capabilities** to the previous versions.
            </p>
            </br>

        - **Sockets** : Socket is the interface between two processes for the purpose of communication. Each socket has a **specific address**. This address is composed of an **IP address and a port number**. Socket are generally employed in **client server applications**.

            <u>**Types of Sockets**</u> - There are two types of Sockets - the **datagram socket** and the **stream socket**.

            1. **Datagram Socket :** This is a type of network which has **connection less point** for sending and receiving packets. It is similar to mailbox. The letters (data) posted into the box are collected and delivered (transmitted) to a letterbox (receiving socket).

            2. **Stream Socket :** In Computer operating system, a stream socket is type of **interprocess communications socket** or **network socket** which provides a **connection-oriented**, **sequenced**, and **unique flow of data** without record boundaries with well defined mechanisms for creating and destroying connections and for detecting errors. It is similar to phone. A connection is established between the phones (two ends) and a conversation (transfer of data) takes place.
    
        - **Ports** : Port Number is a 16-bit number. Total port numbers possible are 2<sup>16</sup> = 65536. All the HTTP stuffs that we do are done on port 80. 
        
            Port Numbers from -
            - **0 - 1023** are reserved already for HTTP stuffs.
            - **1024 - 49151** are registered for some specific applications. *Example -* SQL runs on port **1433**.
            - **49152 - 65536** can be used by you.Ports tell us which application we are working on/ which application the data should go. 

            **Ephemeral Ports** determine which process / instance the data will be recieved in the client side. Servers at most times have fixed port numbers.


    2. **<u>Transport Layer</u>** - The transport layer is responsible for the **transportation of the data from the *network* to the *application***. It is located in your device. When a resource needs to be send, it is given to the socket which gives to the transport layer multiplexer. **Multiplexer** allows us to send multiple things to multiple destinations (might be in the same device). This is called **multiplexing**. **De-multiplexer** allows us to recieve multiple things from multiple destinations. This is called **demultiplexing**. De-multiplexer gives the data to the cocerned socket. The Transport Layer attaches the socket port numbers to the data packets. It also take care of congestion control using congestion control algorithms built in TCP.        
        - ***Checksum*** : A particular string value is created from the data sent. When the data is recieved at the other end, it's checksum is calculated. As the sender has attached the checksum calculated by him in the data packets, then, if the checksums match, it's okay, else, something has gone wrong.

        - ***Timers*** : When a data packet is sent, the timer is started in the sender's device. When the confirmation is recieved, the timer ends. Suppose the second packet sent gets lost, the timer once started, expires after sometime. That's how you can know which data packet has been lost. This timer is known as **Retransmission timer**.

        - ***Sequence Numbers*** : A value/number for the unique identification of data packets, is called sequence numbers. This is useful for identification of duplicate data packets at the reciever's end, if the same packet is retransmitted by the sender for not recieving the acknowledgement message for that packet.
        - ***Transport layer network protocols*** : The protocols used in the transport layer are - 
            - **TCP (Transmission Control Protocol)** - TCP is a transport layer protocol that provides a **reliable stream delivery and virtual connection service to applications through the use of sequenced acknowledgement**. TCP is a **connection-oriented protocol**, as it requires a **connection to be established between applications before data transfer**. Through flow control and acknowledgement of data, **TCP provides extensive error checking**. TCP ensures **sequencing of data**, meaning the data packets arrive in order at the receiving end. **Retransmission of lost data packets is also feasible with TCP**. TCP segments (divides into chunks) the data recieved from the application layer and add headers to it, and re-assemble and put the data recieved into one. Congestion in the network and error is controlled. It maintains the order of data using sequence numbers. It is bi-directional. There can be only two end-points. It adds sequence and acknowledgement number to the data.

                <U>**3-way handshake**</u>
                The client sends a connection request to the server with a **sychronization flag** (a value added in the header) and a **sequence number** (**Random Numbers** to prevent hackers to guess the number)(Suppose, 32). The server then sends the sychronization flag (as it is a new connection), **acknowledgement flag** and acknowledgement number(1 added to the previous sequence number, here, 32 + 1 = 33) along with the new **sequence number**(Suppose, 56) generated after some mathametical operations done on the previous sequence number. Client then sends the **Acknowledgement flag** along with the new sequence number (1 added to the first sequence number sent by it, here, 32 + 1 = 33) and the acknowledgement number (1 added to the previous sequence number, here, 56 + 1 = 57). Then, the connection is established. There are other flags like reset and finish.

                <u>**Advantages :**</u>

                    • TCP ensures three things: data reaches the destination, reaches it on time, and reaches it without duplication.
                    • TCP automatically breaks data into packets before transmission.

                <u>**Disadvantages :**</u>

                    • TCP cannot be used for broadcast and multicast connections.
            </p>

            - **UDP (User Datagram Protocol)** - UDP is a **connection-less protocol** that provides a **simple but unreliable message service**. Unlike TCP, UDP adds **NO reliability, flow control, or error recovery functions**. UDP is useful in situations where the reliability mechanisms of TCP are not necessary. Retransmission of lost data packets **isn't possible** with UDP. Here, data ***may or may not be delivered, may change and may not be in order.*** UDP uses checksum to know whether the data is corrupted or not, but does nothing about those.

                One UDP packet sontains the **data(65536 bytes)** along with the headers containing the **source and destination port numbers(2 + 2 = 4 bytes), length of the datagram(2 bytes) and the checksum (2 bytes)**.

                *<u>Uses of UDP</u>* - Video Conference, DNS and gaming.

                <u>**Advantages :**</u>

                    • Broadcast and multicast connections are possible with UDP.
                    • UDP is faster than TCP.

                <u>**Disadvantages :**</u>

                    • In UDP, it's possible that a packet may not be delivered, be delivered twice, or not be delivered at all.
                    • Manual disintegration of data packets is needed.

    3. **<u>Network layer</u> :** Here, we work with routers. This layer helps in the data transmission from source to destination. The **routing table** is a table inside the router containing information about the topology of the network immediately around it. The data packet will contain the data along with the source network layer address. The router checks whether the data is for a device connected to it or not. If not, then the router checks it's **forwarding table(Or MAC Table)** to find in which direction and to which router the data should go. This goes on until the data recieves the correct router. This is called **hop-by-hop** architecture. This hoping happens at ISPs. Routing table contains multiple paths, whereas forwarding table contains one path, thus it's more faster. Every router has it's own network addresses or Logical addresses.
        - ***Parts Of IP Addresses*** -         
            ![Parts Of IP Addresses](https://www.howtogeek.com/wp-content/uploads/2018/01/ximage-2-1.png.pagespeed.gp+jp+jw+pj+ws+js+rj+rp+rw+ri+cp+md.ic.-bu1fG8j7u.png)
            Here, the Network ID also known as Network address, tells which network your device resides in. The Device ID is your device address.

        - ***Control Plane*** - Control plane is used to create the routing tables. **Control Plane is like a very big graph** in which the **nodes are the routers** and the **edges are the links between routers**. Two types of routing are used to create routing tables :
            - **Static Routing** - Addresses are added ***manually***. This is time consuming and not adaptable easily.
            - **Dynamic Routing** - If there is a change in the addresses or network, addresses are modified ***automatically***. Algorithms used here include Bellman-Ford algorithm, Dijkstra's algorithm, etc.

        - ***Subnetting*** - ![Parts Of IP Addresses](https://www.howtogeek.com/wp-content/uploads/2018/01/ximage-2-1.png.pagespeed.gp+jp+jw+pj+ws+js+rj+rp+rw+ri+cp+md.ic.-bu1fG8j7u.png)
            Here, the Network ID is the subnet ID. All the devices connected to that router having that subnet ID, will have the same subnet IDs and differ only in Host IDs.

        - ***Class Of IP Addresses*** - There are five classes (basically denoting a range of IP addresses) of IP Addresses : 
            - ***Class A*** - from **0.0.0.0** to **127.255.255.255**
            - ***Class B*** - from **128.0.0.0** to **191.255.255.255**
            - ***Class C*** - from **192.0.0.0** to **223.255.255.255**
            - ***Class D*** - from **224.0.0.0** to **239.255.255.255**
            - ***Class E*** - from **240.0.0.0** to **255.255.255.255**

        - ***Subnet Masking*** - It means that the **subnet mask** is going to mask the network ID and leave the host ID for us to use. **Variable length subnets** mean that you can set your own length of the subnet ID. [The Internet Engineering Task Force (IETF)](https://www.ietf.org/) assigns the IP Addresses to the **ISP** without thinking of the classes of IP Addresses, but **based on REGIONS**.

        - ***Reserved IP Addresses*** - 127.0.0.0/8 means that the first 8 bits are reserved, the rest can be used. This are known as **loopback addresses** as the processes which are running on the same machine will allow us to contact the same processes, i.e, our computer acts both as a server and a client at the same time. *Example*: Localhost (127.0.0.1). You can have as many number of loopback addresses as you want.

        - ***Middle Boxes*** - This are devices that comes in between router and system endpoint, and interact with the datapackets. This can be present in network layer or even at transport layer. Example: **Firewall** and **NAT**.
            
            - **Firewall** - Two types are there - One connected to the global internet and the other connected to your own network. The packets coming to the network can be filtered and even modified (the headers and the destination can also be changed), flags can also be checked. There are stateless and stateful firewalls(uses cache so it's much faster).

            - **NAT (Network Address Translation)** - [Network address translation (NAT)](https://en.wikipedia.org/wiki/Network_address_translation) is a method of mapping an IP address space into another by modifying network address information in the IP header of packets while they are in transit across a traffic routing device. It is done to slow down the consumption of IP Addresses.
            ![NAT](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c7/NAT_Concept-en.svg/1280px-NAT_Concept-en.svg.png)

        - ***Network Layer Protocols*** : The protocols used by network layer are - 
            - **IP (Internet Protocol (IPv4))** - IPv4 is a network layer protocol that contains **addressing and control information**, which helps packets be routed in a network. **IP works in tandem with TCP** to deliver data packets across the network. Under IP, each host is assigned a ***<u>32-bit</u>*** address comprised of two major parts: **the network number and host number**. The **network number identifies a network and is assigned by the internet, while the host number identifies a host on the network and is assigned by a network admin**. The **IP is only responsible for delivering the packets, and TCP helps puts them back in the right order.**

                IPv4 data packets has headers(IP Version, identification numbers, length of data, checksum, addresses, ttl(time to leave), etc.) of 20 bytes apart from the data. If ttl(time to leave) is crossed and the data acknowledgement does not return, the packet will be dropped.

                <u>**Advantages :**</u>

                    • IPv4 encrypts data to ensure privacy and security.
                    • With IP, routing data becomes more scalable and economical.

                <u>**Disadvantages :**</u>

                    • IPv4 is labor intensive, complex, and prone to errors.
            <p>

            - **IPv6 (Internet Protocol version 6)** - IPv6 is the latest version of the Internet Protocol, a network layer protocol that possesses addressing and control information for enabling packets to be routed in the network. IPv6 was created to deal with IPv4 exhaustion. It increases the **IP address size from 32 bits to 128 bits** to support more levels of addressing.

                *There are 8 numbers in the IPv6 and each number is a hexa-decimal number and is of 16 bits.*

                <u>**Advantages :**</u>

                    • More efficient routing and packet processing compared to IPv4.
                    • Better security compared to IPv4.

                <u>**Disadvantages :**</u>

                    • IPv6 is not compatible with machines that run on IPv4.
                    • Challenge in upgrading the devices to IPv6.
            <p>

            - **ICMP (Internet Control Message Protocol)** - ICMP is a network layer supporting protocol used by network devices to **send error messages and operational information**. <u>***ICMP messages delivered in IP packets are used for out-of-band messages related to network operation or misoperation***</u>. ICMP is used to **announce network errors, congestion, and timeouts, as well assist in troubleshooting.**

                <u>**Advantages :**</u>

                    • ICMP is used to diagnose network issues.

                <u>**Disadvantages :**</u>

                    • Sending a lot of ICMP messages increases network traffic.
                    • End users are affected if malicious users send many ICMP destination unreachable packets.
            </p>
            </br>

    4. **<u>Data link layer</u> :** The data link layer is responsible for sending the data packets recieved from the network layer, over a physical layer. Router attaches the correct private IP Address to the data packets recieved, ensuring that the data recieves the correct destination.

    - **DHCP (Dynamic Host Configuration Protocol)** - DHCP is a **communication protocol** that enables network administrators to **automate the assignment of IP addresses** in a network. The DHCP server is a pool of IP Addresses and it assigns IP Addresses to the devices connected.
    
                In an IP network, every device connecting to the internet requires a unique IP. DHCP lets network admins distribute IP addresses from a central point and automatically send a new IP address when a device is plugged in from a different place in the network. DHCP works on a **client-server model**. </br>
    
                <u>**Advantages :**</u>

                    • Centralized management of IP addresses.
                    • Seamless addition of new clients into a network.
                    • Reuse of IP addresses, reducing the total number of IP addresses required.

                <u>**Disadvantages :**</u>

                    • Tracking internet activity becomes tedious, as the same device can have multiple IP addresses over a period of time.
                    • Computers with DHCP cannot be used as servers, as their IPs change over time.         

    - **Data Link Layer Address Or MAC Address** - MAC Address depend on the network interface. Two computers at the data link layer communicate with each other using the data link layer address, might happen manually or automatically. ARP(Address Resolution Protocol) cache is used to find out the data link layer address. the frames(Data link layer address of sender and IP Address of destination along with the data) are sent to all the devices connected to the same network.

    - **Data Link Layer Protocols** - The protocols used in data link layer are :
        - **ARP (Address Resolution Protocol)** - The Address Resolution Protocol helps **map IP addresses to physical machine addresses (or a MAC address for Ethernet) recognized in the local network**. A table called an **ARP cache is used to maintain a correlation between each IP address and its corresponding MAC address**. ***ARP offers the rules to make these correlations, and helps convert addresses in both directions.***

            <u>**Advantages :**</u>

                • MAC addresses need not be known or memorized, as the ARP cache contains all the MAC addresses and maps them automatically with IPs.

            <u>**Disadvantages :**</u>

                • ARP is susceptible to security attacks called ARP spoofing attacks.
                • When using ARP, sometimes a hacker might be able to stop the traffic altogether. This is also known as ARP denial-of-services.
        <p>

        - **SLIP (Serial Line IP)** - SLIP is used for **point-to-point serial connections using TCP/IP**. SLIP is used on **dedicated serial links**, and sometimes for **dial-up purposes**. SLIP is useful for **allowing mixes of hosts and routers to communicate with one another**; for example, **host-host, host-router, and router-router** are all common SLIP network configurations. SLIP is merely a **packet framing protocol**: It defines a **sequence of characters that frame IP packets on a serial line**. It does **NOT provide addressing, packet type identification, error detection or correction, or compression mechanisms.**

            <u>**Advantages :**</u>

                • Since it has a small overhead, it is suitable for usage in microcontrollers.
                • It reuses existing dial-up connections and telephone lines.
                • It's easy to deploy since it's based on the Internet Protocol.

            <u>**Disadvantages :**</u>

                • SLIP doesn't support automatic setup of network connections in multiple OSI layers at the same time.
                • SLIP does not support synchronous connections, such as a connection created through the internet from a modem to an internet service provider (ISP).


    5. **Physical Layer** - Network layer works **very close** to the physical layer. This layer contains the physical devices like routers which transports the data to the destination. This is where the **bit synchronization**(number of bits sent and received per unit of time remains consistent) takes place.

<h1 align='center'></h1>
<h1 align='center'>END</br>Thank You ! Hope It Helps!</h1>

# Please share as much as possible.