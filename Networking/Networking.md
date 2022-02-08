# Networking Notes

**How it all Started?**

Cold war was going on between Soviet Union and USA, who will launch first satellite. Soviet won, so usa started a program `ARPA`. So as these buildings were on different places far away, they wanted something to communicate so they developed `ARPA net`. There were four computers, at MIT, Stanford, UCLA, utah connected. They were using TCP for this.

**What is Protocol?**

Protocol is a set of rules which has to be followed, while sending any data over the internet. Exanple of Protocol are: TCP,IP,UDP.

**World Wide Web**

The World wide web commonly known as web is an information system, where documents and other web resources are identified by URLs which may be interlinked by hyperlinks and are accessible over the internet.

Suppose there is a page A about Apple, it contain a different links [More about Apple](https://example.com), and this have a link [Some more about Apple](https://example.com) and so on.

So who write these rules how something will be send, it's the **Internet Society**.

**Client-Server Architecture**

Suppose you search for `google.com` it sends a request to the google server and server sends response back to the client.

TCP (Transmission Control Protocol) = It will ensure that data will reach the destination and it not get corrupted in the process.

UDP (User Datagram Protocol)= When you don't care about, if 100% data is reaching the destination or not, like video conferencing.

HTTP (Hyper text transfer protocol) = This is used by the web browsers. The data that is being transfered between clients and servers is done through rules in HTTP.

**IP Address**

Every single device on the internet, that can talk to each other, have an IP.

Format = X.X.X.X

X = 0-255

Check IP of your pc - `curl ifconfig.me -s`

ISP -> `Modem/Router` -> D1,D2,D3

All the devices connected to this wifi will have the same IP , called Global IP Address. Router gives separate local IP Addresses to all these devices using DHCP (Dynamic Host Configuration Protocol).

When any device connected to this wifi sends a request to `google.com` it has the global IP, then Modem/Router will decide who requested it, and show the response to them. It is done by `NAT`(Network Access Translator).

IP Address decides which device to send the data whereas port numbers are used to identify which application made that request.

**Ports**

Ports are 16 bit numbers, where each bit can contain 0 or 1 so there is total of 2<sup>16</sup> port numbers available.

HTTP = 80
MONGOGB = 27017
SQL = 1433
0-1023 = Reserved Ports
1024-49152 =  Applications

Remaining ports can be used.


### LAN, MAN, WAN  

LAN (Local Area Network)

A local area network (LAN) is a collection of devices connected together in one physical location, such as a building, office, or home. A LAN can be small or large, ranging from a home network with one user to an enterprise network with thousands of users and devices in an office or school. A LAN comprises cables, access points, switches, routers, and other components that enable devices to connect to internal servers, web servers, and other LANs via wide area networks.

MAN (Metropolatian Area Network)

A metropolitan area network (MAN) is a computer network that connects computers within a metropolitan area, which could be a single large city, multiple cities and towns, or any given large area with multiple buildings. A MAN is larger than a local area network (LAN) but smaller than a wide area network (WAN). MANs do not have to be in urban areas; the term "metropolitan" implies the size of the network, not the demographics of the area that it serves.


WAN (Wide Area Network)

A wide-area network (WAN) is a collection of local-area networks (LANs) or other networks that communicate with one another.  A WAN is essentially a network of networks, with the Internet the world's largest WAN.


**SONET** = Synchronous Optical Network. SONET is a communication protocol, developed by Bellcore – that is used to transmit a large amount of data over relatively large distances using optical fibre. SONET is used to convert an electrical signal into an optical signal so that it can travel longer distances.


**Frame Relay** = It is basically a way to connect LAN to WAN.


**MODEM** = Modulation Demodulation. It is sed to convert digital signals to analog signals and vice versa.

**Router** = Routes the packets based on the ip Address.

**ISP** = ISPs are the companies that provide us access to the internet.

### Topologies

- BUS = Bus topology, also known as line topology, is a type of network topology in which all devices in the network are connected by one central RJ-45 network cable or coaxial cable.

- RING = A ring topology is a network configuration where device connections create a circular data path. Each networked device is connected to two others, like points on a circle.

- STAR = Star topology is a network topology in which each network component is physically connected to a central node such as a router, hub or switch.
