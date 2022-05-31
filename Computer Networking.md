<h1 align='center'>Computer Networking</h1>

<h2 align='center'>Introduction</h2>

**Computer Network -** 
Computers connected together is a computer network.

**Internet -**
The system of interconnected computers on a global scale, is called the Internet.

<h2 align='center'>How Internet Was Developed?</h2>

The cold war was going on between United States and the Soviet Union. The soviet union won in launching their first satelite, Sputnik 1 in 1957. The US Government then created a program called as ARPA (Advanced Research Projects Agency). They wanted to have a system of communication to communicate between the other buildings of the ARPA spread around the US. So, they created the ARPANET (The Advanced Research Projects Agency Network) which connected the MIT (Massachusetts Institute of Technology), Stanford University, UCLA (University of California, Los Angeles) and University of Utah. They used TCP/IP (Transmission Control Protocol) in the ARPANET. As time went by, more and more computers were connected. There was no way to automatically share the linked documents. Now, WWW (The World Wide Web) came up, which was developed by Timothy Berners-Lee. This project stored the documents and could be accessed across the web. Here's the [world's first website](http://info.cern.ch/hypertext/WWW/TheProject.html). But, there's no search engines. Now, search engines have been developed. The [Internet Society](https://www.internetsociety.org/) is responsible for maintaining the Internet.

<h2 align='center'>Client-Server Architecture</h2>

When we write [google.com](https://www.google.com/) in the address bar of the browser, our device sends a request to the google server which sends back a response.

<h2 align='center'>Protocols</h3>

1. **TCP (Transmission Control Protocol)** - It ensures that the complete data will reach the destination without any corruption.
2. **UDP (User Datagram Protocol) -** It does not ensure whether the complete data is reaching the destination or not. *Example -* in video calling systems.
3. **HTTP (HyperText Transfer Protocol) -** It defines the format of the data between the clients and servers. *Example -* in the World Wide Web.

<h2 align='center'>IP Address</h2>

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

<h2 align='center'>Port Numbers</h2>

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

<h2 align='center'>Data Transmission</h2>

Data transmission happens in two ways -
- The Guided Way (where path is defined) - *Example -* wired connections between computers.
- The Unguided Way (where path is not defined) - *Example -* Wi-Fi, Bluetooth, etc.

There are submarine cables lied in the oceans and waterbodies, connecting various places around the world. You can checkout the [submarine cable map website](https://www.submarinecablemap.com/).

![submarine cable map website](https://cdn.hashnode.com/res/hashnode/image/upload/v1653998279577/pjYpnHM1r.jpeg)

**Wired Connection -** Optical Fibre cables, coaxial cable </br>
**Wireless connection -** Bluetooth, Wi-Fi, 3G, 4G, LTE, 5G

<h2 align='center'>LAN, MAN and WAN</h2>

- **LAN** *(Local Area Network)* - small area coverage. Wifi and Ethernet are it's examples.
- **MAN** *(Metropolitan area network)* - Accross a city.
- **WAN** *(Wide Area network)* - Accross countries. Optical Fibre Cables are used.

    1. **SONET** *(Synchronous Optical Network)* - It carries the data using optical fibre cables, hence, it can carry data for large distances.
    2. **Frame Relay** - It connects all the Local Area Network with the Wide Area Network.

<h2 align='center'>Modem, Router and DNS</h2>

**Modem** - It is a device which converts the digital signals into analog signals and vice-versa. *Example -* it will convert the digital image in your computer into electrical signals (Analog Signals) which is transmitted over wires(for example).

**Router** - It is a device which routes the data packets.

**DNS** *(Domain Name Server)* - It is a type of phonebook which converts the domain name into the registered IP Address of that domain.

There are also something like Tier-1 ISP , Tier-2 ISP, etc.
In India, Tier-1 ISP is TATA.

<h2 align='center'>Topologies</h2>

1. **Bus Topology -** Only one person can send data at a time.
![Bus Topology Diagram](https://thumbs.dreamstime.com/b/bus-topology-diagram-29007878.jpg)
2. **Ring Topology -**