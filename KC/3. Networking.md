# Networking

## KC - Introduction to Networking

#### 1. Which statement describes a computer network?
- [ ] A computer network is a collection of services that run in the cloud.
- [ ] A computer network is a group of computers that are physically connected to each other through a cable.
- [ ] A computer network is a collection of routers and switches that share data with each other.
- [x] A computer network is a collection of computing devices that are logically connected to communicate and share resources. ✅

#### 2. What is the role of a server in the client-server computing model?
- [ ] The server does not have a role.
- [ ] The server stores responses to a request from the client.
- [ ] The server requests the response from the client.
- [x] The server responds to a request from the client. ✅


#### 3. On which layer of the Open Systems Interconnection (OSI) model is data considered a message or a frame?
- [ ] Layer 1
- [ ] Layer 4
- [ ] Layer 3
- [x] Layer 2 ✅

#### 4. Which statement describes a Media Access Control (MAC) address and how it's used by a network interface card (NIC)?
- [ ] It is an identifier that can be re-assigned or changed. The NIC uses it to identify data about the sender and the receiver.
- [ ] It is an identifier that can't be changed. The NIC uses it to identify only the sender.
- [x] It is a unique physical identifier that's assigned by the manufacturer. The NIC uses it to identify data about the sender and the receiver. ✅
- [ ] It is a unique logical identifier. The NIC uses it to identify data about the sender and the receiver.

#### 5. Which device transmits incoming data to the receiving device by using only Media Access Control (MAC) addresses?
- [x] Switch ✅
- [ ] Hub
- [ ] Firewall
- [ ] Peer

***

## KC - Networking Concepts

#### 1. Which statement accurately describes the function of a local area network (LAN) and a wide area network (WAN)?

- [ ] A LAN connects nodes and hosts over a large geographical area. A WAN connects nodes and hosts within a geographically limited area.
- [x] A LAN connects nodes and hosts within a geographically limited area. A WAN connects multiple LANs to create a more expansive network that can cover large geographical areas, such as cities. ✅
- [ ] A LAN connects servers, but a WAN connects computer devices.
- [ ] A LAN is used for wired networks, but a WAN is used for wireless networks.

#### 2. Consider the similarities between traditional network topologies and AWS services. Which of the following is not an AWS service comparable to a traditional network topology if these similarities are compared?
- [ ] Security groups and network access control lists (network ACLs)
- [x] AWS Transit Gateway ✅
- [ ] Internet gateway
- [ ] Route tables
- [ ] Subnets


#### 3. Which is the most common hybrid topology used today?
- [ ] Bus topology
- [x] Star-bus topology ✅
- [ ] Mesh topology
- [ ] Star topology


#### 4. Which statement describes a connectionless protocol?
- [ ] It will wait for a response from the destination when data is sent.
- [x] It sends a message to the destination without ensuring that the destination is available. ✅
- [ ] It is known as Transmission Control Protocol (TCP).
- [ ] It is known for its reliability and large overhead.


#### 5. Which statement describes a connection-oriented protocol?
- [ ] It is known as User Datagram Protocol (UDP).
- [ ] It doesn't require a session between the sender and receiver.
- [ ] Its best used for transmissions that rely on speed and not reliability.
- [x] It creates a session between the sender and the receiver. ✅

***

## KC - Internet Protocol [IP]

#### 1. Which device should be assigned a static IP address?
- [x] A printer ✅
- [ ] A mobile phone
- [ ] A work computer that is turned on
- [ ] A personal laptop that a network engineer occasionally brings to work
 
#### 2. A network has the following IP address range: 10.0.0.0-10.255.255.255. Which IP address is the network's broadcast address?
- [x] 10.255.255.255 ✅
- [ ] 10.0.0.1
- [ ] 10.0.0.254
- [ ] 10.0.255.254

#### 3. A network engineer wants to separate a network from the internet and from other networks. Which IP address type should the engineer use?
- [x] Private IP address ✅
- [ ] Static IP address
- [ ] Dynamic IP address
- [ ] Public IP address

#### 4. How many bits are in an IPv4 address?
- [x] 32 bits ✅
- [ ] 8 bits
- [ ] 16 bits
- [ ] 4 bits

#### 5. Which statement describes the purpose of a port number?
- [ ] A port number is used to uniquely identify a physical device on a network.
- [ ] A port number assigns a number to an IP address.
- [ ] The port number does not serve a purpose.
- [x] When a port number is combined with an IP address, it uniquely identifies a source or a destination for data communication. ✅

***

## KC - Amazon VPC

#### 1. Which statement describes Amazon Virtual Private Cloud (Amazon VPC)?
- [ ] It is a highly available and scalable Domain Name System (DNS) web service.
- [ ] It is used to manage only public networks in the AWS Cloud.
- [ ] It is an on-premises network.
- [x] It enables you to create a private network in the AWS Cloud. ✅

#### 2. Which resource must be specified when creating a virtual private cloud (VPC)?
- [ ] Linux system
- [x] IP address range ✅
- [ ] Elastic Load Balancing load balancer
- [ ] Amazon Elastic Compute Cloud (Amazon EC2) instance

#### 3. Which resource would benefit from being in a private subnet?
- [ ] An Amazon Elastic Compute Cloud (Amazon EC2) instance hosting a website with a public IP address that must be accessed from the internet
- [ ] A public website
- [ ] A company site that requires both external access and internal access from the public and its employees
- [x] A database ✅

#### 4. What is the purpose of a route table?
- [ ] It determines where all traffic is directed outside the virtual private cloud (VPC).
- [x] It determines where network traffic is directed within the virtual private cloud (VPC). ✅
- [ ] It is responsible for only the network traffic in a subnet.
- [ ] It limits traffic by allowing only specified IP addresses.

#### 5. Which statement describes a security group?
- [ ] It acts as a stateless firewall that controls inbound traffic only.
- [x] It acts as a stateful firewall that controls inbound network traffic and outbound network traffic. ✅
- [ ] It acts as a stateful firewall that allows all traffic by default.
- [ ] It acts as a stateless firewall that controls outbound network traffic only.

***

## KC - IP Subnetting

#### 1. What are some reasons for creating a subnet? (Select TWO.)
- [ ] To add additional IP addresses to an existing subnet
- [x] To reduce network traffic ✅
- [ ] To allocate a specific static IP address
- [x] To divide a network into smaller, more efficient subnets ✅
- [ ] To reduce the number of networks to manage

#### 2. Which IP address class provides for the most hosts?
- [ ] Class D
- [x] Class A ✅
- [ ] Class B
- [ ] Class C

#### 3. Which Classless Inter-Domain Routing (CIDR) notation defines the smallest range of IP addresses, where x represents a digit?
- [ ] xxx.xxx.xxx.xxx/16
- [x] xxx.xxx.xxx.xxx/31 ✅
- [ ] xxx.xxx.xxx.xxx/24
- [ ] xxx.xxx.xxx.xxx/8

#### 4. An administrator creates a subnet with a Classless Inter-Domain Routing (CIDR) range of 10.0.0.0/24. How many IP addresses can the administrator assign to hosts in this subnet?
- [x] 256 ✅
- [ ] 1,024
- [ ] 24
- [ ] 512

#### 5. Which statement describes a subnet mask?
- [ ] It defines the hosts in a network that have a static IP address.
- [ ] It hides the broadcast address in an IP address range.
- [ ] It is used to make a subnet private.
- [x] It defines which section of an IP address identifies the network and which section of an IP address identifies the hosts. ✅

***

## KC - Additional Networking Protocols

#### 1. Which protocols are used to secure web applications? (Select TWO.)
- [x] Transport Layer Security (TLS) ✅
- [ ] Wi-Fi Protected Access (WPA2)
- [x] Secure Sockets Layer (SSL) ✅
- [ ] Hypertext Transfer Text Protocol (HTTP)
- [ ] File Transfer Protocol (FTP)


#### 2. Which statements regarding HTTP are true? (Select TWO.)
- [ ] HTTP is more secure then HTTPS.
- [x] The default port number for HTTP is 80. ✅
- [ ] The default port number for HTTP is 443.
- [ ] HTTP works on layer 5 of the OSI model
- [x] HTTP is a client-server protocol. ✅

#### 3. Which messages are included in a TCP handshake? (Select THREE.)
- [ ] Repeat
- [ ] Finalized (FYN)
- [ ] Resend
- [x] Acknowledge (ACK) ✅
- [x] SYN/ACK ✅
- [x] Synchronize (SYN) ✅

#### 4. A network administrator is troubleshooting a network and wants to analyze packets to view TCP/IP and other packet information that is being transmitted or received over the network. Which command should the network administrator use?
- [ ] netstat
- [ ] whoami
- [x] tcpdump ✅
- [ ] ifconfig

#### 5. Which remote desktop protocol is popular with remote support technicians and is a proprietary Microsoft protocol?
- [ ] Independent Computing Architecture (ICA)
- [x] Remote Desktop Protocol (RDP) ✅
- [ ] Remote Framebuffer (RFB)
- [ ] Virtual Network Computing (VNC)

***

## KC - Additional Networking Technologies

#### 1. Devices communicate with cloud services by using various technologies and protocols. Which option do devices not use to communicate with cloud services?
- [ ] Wi-Fi or broadband internet
- [x] Post Office Protocol (POP) ✅
- [ ] Long-range Wide Area Network (LoRaWAN)
- [ ] Broadband cellular data
- [ ] Narrow-band cellular data

#### 2. Which communication protocols does AWS IoT Core use to communicate with devices? (Select TWO.)
- [ ] Wired Equivalent Privacy (WEP)
- [ ] Wi-Fi Protected Access (WPA)
- [x] MQ Telemetry Transport (MQTT) ✅
- [x] Hypertext Transfer Protocol Secure (HTTPS) ✅
- [ ] Hypertext Transfer Protocol (HTTP)

#### 3. What is the goal of the Internet of Things (IoT)?
- [ ] Provide a secure and robust network of household appliances to facilitate instant adjustments to operate parameters to ensure efficiency.
- [ ] Establish a one-stop wireless connectivity solution that incorporates all wireless devices, both at home and on the road.
- [x] Make devices that can connect to the internet to report data, be monitored, or be remotely controlled. ✅
- [ ] Allow everyday objects-such as refrigerators or heating, ventilation, and air conditioning (HVAC) systems—to take on dual roles as network devices, such as wireless access points, switches, and routers.

#### 4. Which solutions facilitate enterprise mobility for businesses that support remote- working options? (Select TWO.)
- [ ] Device gateways
- [x] Bring your own device (BYOD) ✅
- [ ] Long-range Wide Area Network (LoRaWAN)
- [ ] Internet of Things (IoT)
- [x] Mobile device management (MDM) ✅

#### 5. Which AWS service supports remote work and remote training by providing virtual Microsoft Windows and Linux desktops that can be accessed anywhere and from any device?
- [ ] Amazon Virtual Private Cloud (Amazon VPC)
- [x] Amazon WorkSpaces ✅
- [ ] AWS IoT Core
- [ ] Amazon Elastic Compute Cloud (Amazon EC2)

***
