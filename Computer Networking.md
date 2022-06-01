<h1 align='center'>Computer Networking</h1>

<h2 align='center'><i><u>Introduction</i></u></h2>

**Computer Network -** 
Computers connected together is a computer network.

**Internet -**
The system of interconnected computers on a global scale, is called the Internet.

<h2 align='center'><i><u>How Internet Was Developed?</i></u></h2>

The cold war was going on between United States and the Soviet Union. The soviet union won in launching their first satelite, Sputnik 1 in 1957. The US Government then created a program called as ARPA (Advanced Research Projects Agency). They wanted to have a system of communication to communicate between the other buildings of the ARPA spread around the US. So, they created the ARPANET (The Advanced Research Projects Agency Network) which connected the MIT (Massachusetts Institute of Technology), Stanford University, UCLA (University of California, Los Angeles) and University of Utah. They used TCP/IP (Transmission Control Protocol) in the ARPANET. As time went by, more and more computers were connected. There was no way to automatically share the linked documents. Now, WWW (The World Wide Web) came up, which was developed by Timothy Berners-Lee. This project stored the documents and could be accessed across the web. Here's the [world's first website](http://info.cern.ch/hypertext/WWW/TheProject.html). But, there's no search engines. Now, search engines have been developed. The [Internet Society](https://www.internetsociety.org/) is responsible for maintaining the Internet.

<h2 align='center'><i><u>Client-Server Architecture</i></u></h2>

When we write [google.com](https://www.google.com/) in the address bar of the browser, our device sends a request to the google server which sends back a response.

<h2 align='center'><i><u>Protocols</i></u></h2>

1. **TCP (Transmission Control Protocol)** - It ensures that the complete data will reach the destination without any corruption.
2. **UDP (User Datagram Protocol) -** It does not ensure whether the complete data is reaching the destination or not. *Example -* in video calling systems.
3. **HTTP (HyperText Transfer Protocol) -** It defines the format of the data between the clients and servers. *Example -* in the World Wide Web.

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

Port Number is a 16-bit number. Total port numbers possible are 2<sup>16</sup> = 65536. All the HTTP stuffs that we do are done on port 80. 

Port Numbers from -
 - **0 - 1023** are reserved already for HTTP stuffs.
 - **1024 - 49152** are registered for some specific applications. *Example -* SQL runs on port **1433**.
 - **49152 - 65536** can be used by you.

**What it means by Network speed?** </br>
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
    - **Session Layer** - The Session Layer helps in setting up and managing the connections. It enables the sending and recieving of data followed by termination of connected sessions. Authentication is done in this layer. Then, authorization (Checking whether you have the permission to access any file on the server) is done.
    - **Transport Layer** - UDP and TCP Protocol is used in this layer. The transport layer transports the data in three ways -
        - **Segmentation :** The data that is recieved from the session layer, is segmented. Every segment of the data will contain the sender's and reciever's port numbers, and the sequence numbers. Sequence number helps to reassemble the data in the correct order. 
        - **Flow Control :** The transport layer controls the amount of data that is transmitted.
        - **Error Control :** It checks whether the data is corrupted or missing or not using checksums attached to each data packets. 
    - **Network Layer** - It is responsible for the transmission of the data from one computer to another computer that is located in a different network. Here, router is present. The function os network layer is **Logical addressing**. Logical addressing is the assigning of sender's and reciever's IP Address to each of the data segments and it forms an **IP Packet**, so that all the data packets can reach the correct destination. It performs **routing** which is the movement of the data packet from source to destination. Load balancing also happens here.
    - **Data Link Layer** - It helps to directly communicate with the computers. Physical Addressing happens here. It is the assigning of MAC Address of the sender and reciever's device to the data packets, forming **frames**. MAC address is a 12 digit alphanumeric number of the network interface of your device. It also controls how the data is recieved using Media Access Control.
    - **Physical Layer** - This is the hardware layer which transports the data through wires to the reciever.
    