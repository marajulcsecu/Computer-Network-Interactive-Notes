# University of Chittagong
## Department of Computer Science and Engineering

---

# 6th Semester B.Sc. Engineering Examination, 2023
**Course Code:** CSE 613  **Course Title:** Computer Networks
**Total marks:** 54  **Time:** 4:00 hours

*[Answer any three questions from Section-A and any three questions from Section-B; Separate answer script must be used for Section-A and Section-B.]*

### Section-A

**1.a)** List six access technologies. Classify each one as home access, enterprise access, or wide-area wireless access. **(3)**

**b)** Suppose there is exactly one packet switch between a sending host and a receiving host. The transmission rates between the sending host and the switch and between the switch and the receiving host are R1 and R2, respectively. Assuming that the switch uses store-and-forward packet switching, what is the total end-to-end delay to send a packet of length L? (Ignore queuing, propagation delay, and processing delay.) **(3)**

**c)** Consider an application that transmits data at a steady rate (for example, the sender generates an N-bit unit of data every k time unit, where k is small and fixed). Also, when such an application starts, it will continue running for a relatively long period of time. Answer the following questions, briefly justifying your answer:
  i) Would a packet-switched network or a circuit-switched network be more appropriate for this application? Why?
  ii) Suppose that a packet-switched network is used and the only traffic in this network comes from such applications as described above. Furthermore, assume that the sum of the application data rates is less than the capacities of each and every link. Is some form of congestion control needed? Why? **(3)**

**2.a)** From a user's perspective, what is the difference between the download-and-delete mode and the download-and-keep mode in POP3? **(2)**

**b)** Is it possible for an organization's Web server and mail server to have exactly the same alias for a hostname (for example, *foo.com*)? What would be the type for the RR that contains the hostname of the mail server? **(2)**

**c)** Consider an e-commerce site that wants to keep a purchase record for each of its customers. Describe how this can be done with cookies. **(2)**

**d)** Suppose Alice, with a Web-based e-mail account (such as Hotmail or Gmail), sends a message to Bob, who accesses his mail from his mail server using POP3. Discuss how the message gets from Alice's host to Bob's host. Be sure to list the series of application-layer protocols that are used to move the message between the two hosts. **(3)**

**3.a)** List five nonproprietary Internet applications and the application-layer protocols that they use. **(2)**

**b)** For a P2P file-sharing application, do you agree with the statement, "There is no notion of client and server sides of a communication session"? Why or why not? **(2)**

**c)** Why do HTTP, SMTP, and POP3 run on top of TCP rather than on UDP? **(2)**

**d)** Suppose within your Web browser you click on a link to obtain a Web page. The IP address for the associated URL is not cached in your local host, so a DNS lookup is necessary to obtain the IP address. Suppose that n DNS servers are visited before your host receives the IP address from DNS; the successive visits incur an RTT of RTT1,...,RTTn. Further suppose that the Web page associated with the link contains exactly one object, consisting of a small amount of HTML text. Let RTT0 denote the RTT between the local host and the server containing the object. Assuming zero transmission time of the object, how much time elapses from when the client clicks on the link until the client receives the object? **(3)**

**4.a)** Suppose a process in Host C has a UDP socket with port number 6789. Suppose both Host A and Host B each send a UDP segment to Host C with destination port number 6789. Will both of these segments be directed to the same socket at Host C? If so, how will the process at Host C know that these two segments originated from two different hosts? **(2)**

**b)** Why is it that voice and video traffic is often sent over TCP rather than UDP in today's Internet? **(1)**

**c)** Suppose that the UDP receiver computes the Internet checksum for the received UDP segment and finds that it matches the value carried in the checksum field. Can the receiver be absolutely certain that no bit errors have occurred? Explain. **(2)**

**d)** Compare GBN, SR, and TCP (no delayed ACK). Assume that the timeout values for all three protocols are sufficiently long such that 5 consecutive data segments and their corresponding ACKs can be received (if not lost in the channel) by the receiving host (Host B) and the sending host (Host A) respectively. Suppose Host A sends 5 data segments to Host B, and the 2nd segment (sent from A) is lost. In the end, all 5 data segments have been correctly received by Host B.
  i) How many segments has Host A sent in total and how many ACKs has Host B sent in total? Answer this question for all three protocols.
  ii) If the timeout values for all three protocol are much longer than 5 RTT, then which protocol successfully delivers all five data segments in shortest time interval? **(4)**

### Section-B

**5.a)** What guarantees are made by the Internet's service model regarding the host-to-host delivery of datagrams? **(1)**

**b)** Suppose that a Web server runs in Host C on port 80. Suppose this Web server uses persistent connections, and is currently receiving requests from two different Hosts, A and B. Are all of the requests being sent through the same socket at Host C? If they are being passed through different sockets, do both of the sockets have port 80? Discuss and explain. **(1+2)**

**c)** Suppose that an arriving packet matches two or more entries in a router's forwarding table. With traditional destination-based forwarding, what rule does a router apply to determine which of these rules should be applied to determine the output port to which the arriving packet should be switched? **(2)**

**d)** Consider a router that interconnects three subnets: Subnet 1, Subnet 2, and Subnet 3. Suppose all of the interfaces in each of these three subnets are required to have the prefix 223.1.17/24. Also suppose that Subnet 1 is required to support at least 60 interfaces, Subnet 2 is to support at least 90 interfaces, and Subnet 3 is to support at least 12 interfaces. Provide three network addresses (of the form a.b.c.d/x) that satisfy these constraints. **(3)**

**6.a)** What is meant by a control plane that is based on per-router control? In such cases, when we say the network control and data planes are implemented "monolithically," what do we mean? **(2)**

**b)** Compare and contrast link-state and distance-vector routing algorithms. What is the "count to infinity" problem in distance vector routing? **(3)**

**c)** Consider the following network. With the indicated link costs, use Dijkstra's shortest-path algorithm to compute the shortest path from u to all network nodes. **(3)**

*(Network diagram with nodes u, v, w, x, y, z and edges: v-w:5(top arc), u-v:2, v-w:3, w-z:5, u-x:1, v-x:2, w-x:3, w-y:1, x-y:1, y-z:2)*

**d)** Determine whether the following statements are *true* or *false*? **(1)**
  i) When an OSPF route sends its link state information, it is sent only to those nodes directly attached neighbors.
  ii) When a BGP router receives an advertised path from its neighbor, it must add its own identity to the received path and then send that new path on to all of its neighbors.

**7.a)** Distinguish between the following multiple access protocol:
  (i) Pure Aloha and Slotted Aloha, (ii) Persistent and Nonpersistent CSMA. **(2)**

**b)** Suppose two nodes start to transmit at the same time a packet of length L over a broadcast channel of rate R. Denote the propagation delay between the two nodes as d_prop. Will there be a collision if d_prop < L/R? Why or why not? **(2)**

**c)** Suppose the information content of a packet is the bit pattern 1110 0110 1001 1101 and an even parity scheme is being used. What would the value of the field containing the parity bits be for the case of a two-dimensional parity scheme? **(2)**

**d)** Consider the 5-bit generator, G=10011, and suppose that D has the value 1010101010. What is the value of R? **(3)**

**8.a)** Suppose you purchase a wireless router and connect it to your cable modem. Also suppose that your ISP dynamically assigns your connected device (that is, your wireless router) one IP address. Also suppose that you have five PCs at home that use 802.11 to wirelessly connect to your wireless router. How are IP addresses assigned to the five PCs? Does the wireless router use NAT? Why or why not? **(4)**

**b)** Using RSA, choose p=3 and q=11, and encode the word "dog" by encrypting each letter separately. Apply the decryption algorithm to the encrypted version to recover the original plaintext message. **(3)**

**c)** Suppose Alice and Bob are sending packets to each other over a computer network. Suppose Trudy positions herself in the network so that she can capture all the packets sent by Alice and send whatever she wants to Bob; she can also capture all the packets sent by Bob and send whatever she wants to Alice. List some of the malicious things Trudy can do from this position. **(2)**

---

# 6th Semester B.Sc. (Engg) Examination-2022
**Course Code:** CSE-613  **Course Title:** Computer Networks
**Total marks:** 54 Marks  **Time:** 4.00 hours

*[Answer any three questions from each of the Section-A and Section-B. Figures in the right-hand margin indicate full marks]*

### Section A

**1.a)** Describe the most popular wireless Internet access technologies today. Compare and contrast them. **(2+2)**

**b)** It has been said that flow control and congestion are equivalent. Is this true for the Internet's connection-oriented service? **(2)**

**c)** Why will two ISPs at the same level of the hierarchy often peer with each other? How does an IXP earn money? **(2+1)**

**2.a)** Consider sending a packet from a source host to a destination host over a fixed route. List the delay components in the end-to-end delay. Which of these delays are constant and which are variable? **(2+1)**

**b)** Suppose end system A wants to send a large file to end system B. At a very high level, describe how end system A creates packets from the file. When one of these packets arrives to a router, what information in the packet does the router use to determine the link onto which the packet is forwarded? Why is packet switching in the Internet analogous to driving from one city to another and asking directions along the way? **(3)**

**c)** Describe how Web caching can reduce the delay in receiving a requested object. Will Web caching reduce the delay for all objects requested by a user or for only some of the objects? **(2)**

**d)** What is the difference between network architecture and application architecture? **(1)**

**3.a)** For a P2P file-sharing application, do you agree with the statement, "There is no notion of client and server sides of a communication session"? Why or why not? **(2)**

**b)** Why do HTTP, SMTP, and POP3 run on top of TCP rather than on UDP? **(2)**

**c)** In BitTorrent, suppose Alice provides chunks to Bob throughout a 30-second interval. Will Bob necessarily return the favor and provide chunks to Alice in this same interval? Why or why not? **(2)**

**d)** What is an overlay network? Does it include routers? What are the edges in the overlay network? **(3)**

**4.a)** Consider a planet where everyone belongs to a family of six, every family lives in its own house, each house has a unique address, and each person in a given house has a unique name. Suppose this planet has a mail service that delivers letters from source house to destination house. The mail service requires that (1) the letter be in an envelope, and that (2) the address of the destination house (and nothing more) be clearly written on the envelope. Suppose each family has a delegate family member who collects and distributes letters for the other family members. The letters do not necessarily provide any indication of the recipients of the letters.
  a. Describe a protocol that the delegates can use to deliver letters from a sending family member to a receiving family member.
  b. In your protocol, does the mail service ever have to open the envelope and examine the letter in order to provide its service? **(2+2)**

**b)** Is it possible for an application to enjoy reliable data transfer even when the application runs over UDP? If so, how? **(1+2)**

**c)** Suppose two TCP connections are present over some bottleneck link of rate R bps. Both connections have a huge file to send (in the same direction over the bottleneck link). The transmissions of the files start at the same time. What transmission rate would TCP like to give to each of the connections? **(2)**

### Section B

**5.a)** We made a distinction between the forwarding function and the routing function performed in the network layer. What are the key differences between routing and forwarding? What are the main functions of the data plane and control plane? **(1.5+1.5)**

**b)** Describe how packet loss can occur at input ports. Describe how packet loss at input ports can be eliminated **(2)**

**c)** Give an example showing why a network operator might want one class of packets to be given priority over another class of packets. **(2)**

**d)** Why are different inter-AS and intra-AS protocols used in the Internet? **(2)**

**6.a)** Write the possibilities for when the routers are used as mobile. **(2)**

**b)** What is an essential difference between RR and WFQ packet scheduling? Is there a case (Hint: Consider the WFQ weights) where RR and WFQ will behave exactly the same? **(3)**

**c)** What is meant by the term "route aggregation"? Why is it useful for a router to perform route aggregation? **(1.5+1.5)**

**d)** How does generalized forwarding differ from destination-based forwarding? **(1)**

**7.a)** What is meant by a control plane that is based on logically centralized control? In such cases, are the data plane and the control plane implemented within the same device or in separate devices? Explain. **(2+2)**

**b)** Is it necessary that every autonomous system use the same intra-AS routing algorithm? Why or why not? **(1.5)**

**c)** True or false: When an OSPF route sends its link state information, it is sent only to those nodes directly attached neighbors. Explain. **(1+1)**

**d)** What is meant by an area in an OSPF autonomous system? **(1.5)**

**8.a)** Define the following terms in the context of SNMP: managing server, managed device, network management agent and MIB. **(1.5+1.5+1.5+1.5)**

**b)** What are the purposes of the SNMP GetRequest and SetRequest messages? **(1.5)**

**c)** What is the purpose of the SNMP trap message? **(1.5)**

---

# Sixth Semester B.Sc. Engineering Examination 2020
**Course Code:** CSE 613
**Course Title:** Computer Networking
**Total Marks:** 52.5  **Time:** 04 hours

*[Answer any Three questions from Section-A and any Three question from Section-B. Figures in the right hand margin indicate full marks.]*

### Section-A

**1.a)** List four access technologies. Classify each one as home access, enterprise access, or wide-area wireless access. **(2)**

**b)** Suppose Host A wants to send a large file to Host B. The path from Host A to Host B has three links, of rates R1 = 500 kbps, R2 = 2 Mbps, and R3 = 1 Mbps.
  a. Assuming no other traffic in the network, what is the throughput for the file transfer?
  b. Suppose the file is 4 million bytes. Dividing the file size by the throughput, roughly how long will it take to transfer the file to Host B? **(2)**

**c)** What are the five layers in the Internet protocol stack? What are the principal responsibilities of each of these layers? **(2.75)**

**d)** Skype offers a service that allows you to make a phone call from a PC to an ordinary phone. This means that the voice call must pass through both the Internet and through a telephone network. Discuss how this might be done. **(2)**

**2.a)** Describe how Web caching can reduce the delay in receiving a requested object. Will Web caching reduce the delay for all objects requested by a user or for only some of the objects? Why? **(2)**

**b)** What is the HOL blocking issue in HTTP/1.1? How does HTTP/2 attempt to solve it? **(2)**

**c)** Consider a new peer Alice that joins BitTorrent without possessing any chunks. Without any chunks, she cannot become a top-four uploader for any of the other peers, since she has nothing to upload. How then will Alice get her first chunk? **(2)**

**d)** Suppose within your Web browser you click on a link to obtain a Web page. The IP address for the associated URL is not cached in your local host, so a DNS lookup is necessary to obtain the IP address. Suppose that n DNS servers are visited before your host receives the IP address from DNS; the successive visits incur an RTT of RTT1, . . . , RTTn. suppose the HTML file references eight very small objects on the same server. Let RTT0 denote the RTT between the local host and the server containing the object. Neglecting transmission times, how much time elapses with
  a. Non-persistent HTTP with no parallel TCP connections?
  b. Non-persistent HTTP with the browser configured for 6 parallel connections?
  c. Persistent HTTP? **(2.75)**

**3.a)** Suppose a process in Host C has a UDP socket with port number 6789. Suppose both Host A and Host B each send a UDP segment to Host C with destination port number 6789. Will both of these segments be directed to the same socket at Host C? If so, how will the process at Host C know that these two segments originated from two different hosts? **(2)**

**b)** Draw the FSM for sender side of reliable data transfer protocol over a lossy channel with a bit error. **(2)**

**c)** Host A and B are directly connected with a 100 Mbps link. There is one TCP connection between the two hosts, and Host A is sending to Host B an enormous file over this connection. Host A can send its application data into its TCP socket at a rate as high as 120 Mbps but Host B can read out of its TCP receive buffer at a maximum rate of 50 Mbps. Describe the effect of TCP flow control. **(2)**

**d)** Compare between GBN and SR protocol. **(2.75)**

**4.a)** What is the difference between network architecture and application architecture? **(1.25)**

**b)** Suppose you want to do a transaction from a remote client to a server as fast as possible. Would you use UDP or TCP? Why? **(2)**

**c)** Why do HTTP, SMTP and IMAP run on top of TCP rather than on UDP? **(1.5)**

**d)** Consider an e-commerce site that wants to keep a purchase record for each of its customers. Describe how this can be done with cookies. **(2)**

**e)** Describe three major components of TCP congestion control algorithm. **(2)**

### Section B

**5.a)** Suppose there are three routers between a source host and a destination host. Ignoring fragmentation, an IP datagram sent from the source host to the destination host will travel over how many interfaces? How many forwarding tables will be indexed to move the datagram from the source to the destination?

**b)** Suppose you purchase a wireless router and connect it to your cable modem. Also suppose that your ISP dynamically assigns your connected device (that is, your wireless router) one IP address. Also suppose that you have five PCs at home that use 802.11 to wirelessly connect to your wireless router. How are IP addresses assigned to the five PCs? Does the wireless router use NAT? Why or why not?

**c)** What is NAT? Describe the working procedure of NAT

**d)** Compare and contrast the IPv4 and the IPv6 header fields. Do they have any fields in common?

**6.a)** Consider a datagram network using 8-bit host addresses. Suppose a router uses longest prefix matching and has the following forwarding table:

| Prefix Match | Interface |
|---|---|
| 00 | 0 |
| 010 | 1 |
| 011 | 2 |
| 10 | 2 |
| 11 | 3 |

For each of the four interfaces, give the associated range of destination host addresses and the number of addresses in the range. **(3)**

**b)** Consider a router that interconnects three subnets: Subnet 1, Subnet 2, and Subnet 3. Suppose all of the interfaces in each of these three subnets are required to have the prefix 223.1.17/24. Also suppose that Subnet 1 is required to support at least 60 interfaces, Subnet 2 is to support at least 90 interfaces, and Subnet 3 is to support at least 12 interfaces. Provide three network addresses (of the form a.b.c.d/x) that satisfy these constraints. **(3)**

**c)** Write short note on DHCP. **(2.75)**

**7.a)** Consider the SDN OpenFlow network shown in following Figure. Suppose that the desired forwarding behavior for datagrams arriving at s2 is as follows:
  - any datagrams arriving on input port 1 from hosts h5 or h6 that are destined to hosts h1 or h2 should be forwarded over output port 2;
  - any datagrams arriving on input port 2 from hosts h1 or h2 that are destined to hosts h5 or h6 should be forwarded over output port 1;
  - any arriving datagrams on input ports 1 or 2 and destined to hosts h3 or h4 should be delivered to the host specified;
  - hosts h3 and h4 should be able to send datagrams to each other. Specify the flow table entries in s2 that implement this forwarding behavior **(4)**

  *Figure: OpenFlow match-plus-action network with three packet switches, 6 hosts, and an OpenFlow controller.*
  (Hosts h1 10.1.0.1, h2 10.1.0.2, h3 10.2.0.3, h4 10.2.0.4, h5 10.3.0.5, h6 10.3.0.6, three switches s1/s2/s3 connected to an OpenFlow controller)

**b)** Is it necessary that every autonomous system use the same intra-AS routing algorithm? Why or why not? Why are different inter-AS and intra-AS protocols used in the Internet? **(2)**

**c)** Consider the following network. With the indicated link costs, use Dijkstra's shortest-path algorithm to compute the shortest path from x to all network nodes. **(2.75)**

  *(Network diagram with nodes x, y, z, v, t, u, w and edges: z-y:12, x-z:8, x-y:6, x-v:3, y-v:8, y-t:7, v-t:4, v-u:3, t-u:2, x-w:4, w-u:3, w-v: — )*

**8.a)** Why would the token-ring protocol be inefficient if a LAN had a very large perimeter? **(1)**

**b)** Why is an ARP query sent within a broadcast frame? Why is an ARP response sent within a frame with a specific destination MAC address? **(2)**

**c)** Suppose that N switches supporting K VLAN groups are to be connected via a trunking protocol. How many ports are needed to connect the switches? Justify your answer. **(2)**

**d)** Briefly describe the scenario of a day in the life of a web page request. **(3.75)**

---

# 6th Semester B.Sc (Engineering) Examination 2019
**Course no:** CSE 613  **Course Title:** Computer Networks
**Full Marks:** 52.5  **Time:** 4 Hours

*[Answer any three questions from each section. Answer all parts of questions chronologically. Figures at right margin illustrate marks.]*

### SECTION-A

**1 a)** Suppose you walk into a room, connect to Ethernet, and want to download a Web page. What are all the protocol steps that take place, starting from powering on your PC to getting the Web page? Assume there is nothing in our DNS or browser caches when you power on your PC. (*Hint: the steps include the use of Ethernet, DHCP, ARP, DNS, TCP, and HTTP protocols.*) Explicitly indicate in your steps how you obtain the IP and MAC addresses of a gateway router. **(5)**

**b)** How does an end system access the edge router? Describe your answer. **(3)**

**c)** How big is the MAC address space? The IPv4 address space? The IPv6 address space? **(0.75)**

**2 a)** Suppose Host A wants to send a large file to Host B. The path from Host A to host B has three links, of rates R1 = 500 kbps, R2 = 2 Mbps, and R3 = 1 Mbps
  i) Assuming no other traffic in the network, what is the throughput for the file transfer?
  ii) Suppose the file is 4 million bytes. Dividing the file size by the throughput, roughly how long will it take to transfer the file to Host B?
  iii) Repeat (a) and (b), but now with R2 reduced to 100 kbps. **(3)**

**b)** Differentiate between Client-Server architecture and P2P architecture with example. **(2)**

**c)** Give short note on:
  i) Loss tolerant application. ii) Bandwidth sensitive application.
  iii) Elastic application iv) Real time application **(2)**

**d)** What is the difference between network architecture and application architecture? **(1.75)**

**3 a)** Suppose within your Web browser you click on a link to obtain a Web page. The IP address for the associated URL is not cached in your local host, so a DNS lookup is necessary to obtain the IP address. Suppose that n DNS servers are visited before your host receives the IP address from DNS; the successive visits incur an RTT of RTT1, . . ., RTTn. Further suppose that the Web page associated with the link contains exactly one object, consisting of a small amount of HTML text. Let RTT0 denote the RTT between the local host and the server containing the object. Assuming zero transmission time of the object,
  i) How much time elapses from when the client clicks on the link until the client receives the object?
  If the HTML file references eight very small objects on the same server. Neglecting transmission times, how much time elapses with
  ii) Non-persistent HTTP with no parallel TCP connections?
  iii) Non-persistent HTTP with the browser configured for 5 parallel connections?
  iv) Persistent HTTP? **(4)**

**b)** Compare between HTTP and SMTP protocol. **(2)**

**c)** Suppose you have configured your POP mail client to operate in the download-and-delete mode. Complete the following transaction:
```
C: list
S: 1 498
S: 2 912
S: .
C: retr 1
S: blah blah ...
S: .........blah
S: .
?
?
```
What is the problem with download and delete mode? How can you overcome it? **(2.75)**

**4. (a)** What are the general principles of congestion control? **(2.5)**

**(b)** Store-and-forward switches have an advantage over cut-through switches with respect to damaged frames. Explain what it is. **(2)**

**(c)** Explain virtual LANs. **(2)**

**(d)** Shortly discuss about Bluetooth architecture. **(2.25)**

### SECTION-B

**5. (a)** Why IPv6 is preferred than IPv4? **(1.5)**

**(b)** Discuss about ICMP, ARP, RARP, BOOTP and DHCP **(7.25)**

**6 a)** Consider the following configuration:
Network address 192.10.10.0. Number of needed subnets 14 and number of needed usable hosts 14
Fill in the gaps
  i) Number of bit borrowed ……………
  ii) Custom Subnets ……………
  iii) Total Number of Subnets ……………
  iv) Number of usable host add ……………
  v) 4th subnet range ……………
  vi) Network address for 5th subnet …………… **(3)**

**b)** Consider the following LAN configuration.
```
N1 : 192.168.5.64/26   N2: 192.168.5.128/26   N3: 192.168.5.23.6/28
L1: 192.168.5.224/30   L2: 192.168.5.228/30   L3: 192.168.5.232/30
L4: 192.168.5.236/30
```
**(3)**

*(Diagram: N1, N2, N3, N4 routers connected via L1, L2, L3, L4 in a diamond topology; N4 has 14 hosts)*
  i) Identify subnet mask for each subnet.
  ii) How many usable IP addresses for N1, N2 and N3 LAN.
  iii) Identify the IP address of LAN N4

**c)** Why are different inter-AS and intra-AS protocols used in the internet? **(2.75)**

**7 a)** How DHCP assign ip address to a newly arriving host? Describe with example. **(2)**

**b)** Describe the function of NAT. Why some people against to NAT? What is the function of UPnP protocol? **(3)**

**(c)** What is the use of SNMP protocol in a network? **(1.75)**

**(d)** Compare between channel partitioning and random access protocols. **(2)**

**8 a)** If all the links in the Internet were to provide reliable delivery service, would the TCP reliable delivery service be redundant? Why or why not? **(2.75)**

**b)** Define Ethernet. Which multiple access protocol is used by Ethernet? **(2)**

**c)** Describe the pros and cons of slotted ALOHA protocol **(2)**

**d)** What is the size of ARP packet when the protocol is IPv4 and the hardware is Ethernet? **(2)**

---

# 6th Semester B.Sc (Engineering) Examination 2018
**Course no:** CSE 613  **Course Title:** Computer Networks
**Full Marks:** 52.5  **Time:** 4 Hours

*[Answer any three questions from each section. Figures at right margin illustrate marks]*

### SECTION-A

**1. (a)** Briefly describe OSI reference model with necessary figure. **(3)**

**(b)** Internet's connection-oriented service provides reliable transport; explain it. **(2)**

**(c)** It has been said that flow control and congestion are equivalent. Is this true for the Internet's connection-oriented service? **(0.75)**

**(d)** What advantage does a circuit-switched network have over a packet-switched network? **(1)**

**(e)** Write short notes on POP and NAP. **(2)**

**2. (a)** In a P2P file sharing application, do you agree with this statement, "There is no notion of client and server sides of a communication session"? Why or why not? **(2)**

**(b)** What is the difference between persistent HTTP with pipelining and persistent HTTP without pipelining? Which of the two is used by HTTP/1.1? **(1.25)**

**(c)** Describe how Web caching can reduce the delay in receiving a requested object. Will Web caching reduce the delay for all objects requested by a user or for only some of the objects? **(2)**

**(d)** What is meant by handshaking protocol? **(1)**

**(e)** Why is it said that FTP sends control information "out-of-band"? **(1)**

**(f)** What are the main differences between TCP and UDP? **(1.5)**

**3. (a)** Consider a TCP connection between Host A and Host B. Suppose that the TCP segments traveling from Host A to Host B have source port number x and destination port number y. What are the source and destination port numbers for the segments traveling from Host B to Host A? **(2)**

**(b)** Draw the FSM for the receiver side of protocol rdt 2.2 **(2)**

**(c)** Write the possibilities for handling corrupted ACKs or NAKs **(1.5)**

**(d)** Differentiate between GBN and SR protocol with example. **(2)**

**(e)** Describe why an application developer might choose to run an application over UDP rather than TCP. **(1.5)**

**4. (a)** What is the fundamental difference between a router and link-layer packet? **(1.5)**

**(b)** What are the two most important network-layer functions in a datagram network? **(1.5)**

**(c)** Explain how DNS works. **(2)**

**(d)** What are the different types of DNS records and messages? **(2)**

**(e)** Do routers have IP addresses? If so, how many? **(1)**

**(f)** Write the use of IGMP protocol? **(0.75)**

### SECTION-B

**5. (a)** Why IP service model known as best-effort delivery service? **(2)**

**(b)** Compare and contrast the IPv4 and the IPv6 header fields. Do they have any fields in common? Which fields are no longer present in IPv6 datagram? **(2)**

**(c)** Explain the role of ARP. **(2)**

**(d)** Why are different inter-AS and intra-AS protocols used in the Internet? **(2)**

**(e)** Define topology of a network. **(0.75)**

**6. (a)** Define routing algorithm. Briefly describe the following routing algorithms with example:
  i. Shortest Path Routing.
  ii. Link State Routing **(3.5)**

**(b)** What is ICMP? Specify types of ICMP messages. **(2.25)**

**(c)** How does DNS resolve a remote name? **(3)**

**7. (a)** How does DHCP assign IP address to a newly arriving host? Describe with block diagram **(2)**

**(b)** What are some of the possible services that a link-layer protocol can offer to the network layer? Which of these link-layer services have corresponding services in IP? In TCP? **(2)**

**(c)** What is MAC? Write the characteristics of MAC. **(2.75)**

**(d)** Explain the Ethernet Frame header with necessary pictorial diagram **(2)**

**8. (a)** What do you mean by mobility? Give short note on: mobility via indirect routing and mobility via direct routing. **(3)**

**(b)** How a mobile agent register it's mobile IP with its home agent? **(2)**

**(c)** Differentiate between mobile IP and GSM mobility. **(2)**

**(d)** Why are different inter-AS and intra-AS protocols used in the Internet? **(0.75)**

**(e)** What are BSS and AP? **(1)**

---

# 6th Semester B.Sc (Engineering) Examination 2017
**Course Code:** CSE 613  **Course Title:** Computer Networks
**Full Marks:** 52.5  **Time:** 4 hours

*[Answer any 3 questions from each section. Answer all parts of questions chronologically. Figures in the right hand margin indicate full marks.]*

### Section A

**1 a)** Show a journey of a message from host A to host B considering following topics. **(2.75)**

*(Diagram showing host A with wireless devices connecting through network to host B with routers and network infrastructure)*

  i) Identify different network devices in the scenario.
  ii) Give some example of network application program runs on a host.
  iii) Mention the protocols use in different layers.
  iv) Different transmission media used in computer networking.
  v) Different LAN technologies used now a day.
  vi) How does a host access the network infrastructure?
  vii) Techniques to switch packets over network.

**b)** Illustrate the differences between OSI and TCP/ IP models.

**c)** Consider two hosts, A and B, connected by a single link of rate R bps. Suppose that the two hosts are separated by m meters, and suppose the propagation speed along the link is s meters/sec. Host A is to send a packet of size L bits to Host B.

  i. Express the propagation delay, d_prop, in terms of m and s.
  ii. Determine the transmission time of the packet, d_trans, in terms of L and R.
  iii. Ignoring processing and queuing delays, obtain an expression for the end-to-end delay.
  iv. Suppose Host A begins to transmit the packet at time t = 0. At time t = d_trans, where is the last bit of the packet?
  v. Suppose d_prop is greater than d_trans. At time t = d_trans, where is the first bit of the packet?

**d)** Some content providers have created their own networks. Describe Google's network. What motivates content providers to create these networks? **(2)**

**a)** Describe how Web caching can reduce the delay in receiving a requested object. Will Web caching reduce the delay for all objects requested by a user or for only some of the objects? **(2)**

**b)** Why it is said that FTP sends control information "out-of-band"? **(2)**

**c)** From a user's perspective, what is the difference between the download-and delete mode and the download-and-keep mode in POP3? **(2)**

**d)** Consider the following string of ASCII characters that were captured by Wireshark when the browser sent an HTTP request and receive response message from a server. Answer the following questions, **(2.75)**

```
GET /cs453/index.html HTTP/1.1<cr><lf>Host: gaia.cs.umass.edu<cr><lf>User-Agent: Mozilla/5.0 (Windows; U;
Windows NT 5.1; en-US; rv:1.7.2) Gecko/20040804 Netscape/7.2 (ax) <cr><lf>Accept:ext/xml, application/xml,
application/xhtml+xml, text/html;q=0.9, text/plain;q=0.8,image/png,*/*;q=0.5 <cr><lf>Accept-Language: en-
us,en;q=0.5<cr><lf>Accept-Encoding: zip,deflate<cr><lf>Accept-Charset: ISO-8859-1,utf
8;q=0.7,*;q=0.7<cr><lf>Keep-Alive: 300<cr><lf>Connection:keep-alive<cr><lf><cr><lf>

HTTP/1.1 200 OK<cr><lf>Date: Tue, 07 Mar 2008 12:39:45GMT<cr><lf>Server: Apache/2.0.52
(Fedora)<cr><lf>Last-Modified: Sat, 10 Dec2005 18:27:46GMT<cr><lf>ETag: "526c3-f22-
a88a4c80"<cr><lf>Accept-Ranges:bytes<cr><lf>Content-Length: 3874<cr><lf>

Keep-Alive: timeout=max=100<cr><lf>Connection:Keep-Alive<cr><lf>Content-Type: text/html; charset= ISO-8859-
1<cr><lf><cr><lf><!doctype html public "-//w3c//dtd html
4.0 transitional//en"><lf><html><lf><head><lf><metahttp-equiv="Content-Type"content="text/html;
charset=iso88591"><lf>< meta name ="GENERATOR"content="Mozila/4.79 [en] (Windows NT 5.0; U)
Netscape]"><lf> <title>CMPSCI 453 / 591 /NTU-ST550A Spring 2005 homepage</title><lf></head><lf> <much
more document text following here (not shown)>
```

  i. What is the URL of the document requested by the browser?
  ii. What version of HTTP is the browser running?
  iii. Does the browser request a non-persistent or a persistent connection?
  iv. What type of browser initiates this message? Why is the browser type needed in an HTTP request message?
  v. Was the server able to successfully find the document or not? What time was the document reply provided?
  vi. When the document was last modified?
  vii. How many bytes are there in the document being returned?
  viii. What are the first 5 bytes of the document being returned? Did the server agree to a persistent connection?

**a)** Describe the FSM of stop-and-wait rdt protocol. What is the main problem of it? How next rdt protocol overcomes that problem? **(2)**

**b)** Mention whether the following scenarios or statements are true or false. **(2.75)**
  i. Host A is sending Host B a large file over a TCP connection. Assume Host B has no data to send Host A. Host B will not send acknowledgments to Host A because Host B cannot piggyback the acknowledgments on data.
  ii. The size of the TCP rwnd never changes throughout the duration of the connection.
  iii. Suppose Host A is sending Host B a large file over a TCP connection. The number of unacknowledged bytes that A sends cannot exceed the size of the receive buffer.
  iv. Suppose Host A is sending a large file to Host B over a TCP connection. If the sequence number for a segment of this connection is m, then the sequence number for the subsequent segment will necessarily be m + 1.
  v. The TCP segment has a field in its header for rwnd.
  vi. Suppose that the last SampleRTT in a TCP connection is equal to 1 sec. The current value of TimeoutInterval for the connection will necessarily be ≥ 1 sec.
  viii. Suppose Host A sends one segment with sequence number 38 and 4 bytes of data over a TCP connection to Host B. In this same segment the acknowledgment number is necessarily 42.

**c)** Describe the advantage and disadvantage of GBN protocol. How SR protocol overcomes the problem of GBN protocol? **(2)**

**d)** Describe TCP flow control mechanism. Indicate which field is used for flow control in TCP segment structure? Describe with block diagram. **(2)**

**4 a)** Differentiate between end-to-end congestion control and network assisted congestion control **(2)**

**b)** Suppose that the five measured SampleRTT values are 106 ms, 120 ms, 140 ms, 90 ms, and 115 ms. Compute the EstimatedRTT after each of these SampleRTT values is obtained, using a value of α= 0.125 and assuming that the value of EstimatedRTT was 100 ms just before the first of these five samples were obtained. Compute also the DevRTT after each sample is obtained, assuming a value of β= 0.25 and assuming the value of DevRTT was 5 ms just before the first of these five samples was obtained. Last, compute the TCP TimeoutInterval after each of these samples is obtained. **(2.75)**

**c)** What are the roles of electromagnetic spectrum in wireless transmission? **(2)**

**d)** Consider transferring an enormous file of L bytes from Host A to Host B. Assume an MSS of 536 bytes. **(2)**
  i. What is the maximum value of L such that TCP sequence numbers are not exhausted? Recall that the TCP sequence number field has 4 bytes.
  ii. For the L you obtain in (a), find how long it takes to transmit the file. Assume that a total of 66 bytes of transport, network, and data-link header are added to each segment before the resulting packet is sent out over a 155 Mbps link. Ignore flow control and congestion control so A can pump out the segments back to back and continuously.

### Section B

**5 (a)** Do the routers in both datagram networks and virtual-circuit networks use forwarding tables? If so, describe the forwarding tables for both classes of networks.

**(b)** Consider a router that interconnects three subnets: Subnet 1, Subnet 2, and Subnet 3. Suppose all of the interfaces in each of these three subnets are required to have the prefix 223.1.17/24. Also suppose that Subnet 1 is required to support at least 60 interfaces, Subnet 2 is to support at least 90 interfaces, and Subnet 3 is to support at least 12 interfaces. Provide three network addresses (of the form a.b.c.d/x) that satisfy these constraints. **(2)**

**(c)** Consider a subnet with prefix 128.119.40.128/26. Give an example of one IP address (of form xxx.xxx.xxx.xxx) that can be assigned to this network. Suppose an ISP owns the block of addresses of the form 128.119.40.64/26. Suppose it wants to create four subnets from this block, with each block having the same number of IP addresses. What are the prefixes (of form a.b.c.d/x) for the four subnets? What are the ranges of assignable IP address for the four subnets? **(2.75)**

**(d)** Suppose you purchase a wireless router and connect it to your cable modem. Also suppose that your ISP dynamically assigns your connected device (that is, your wireless router) one IP address. Also suppose that you have five PCs at home that use 802.11 to wirelessly connect to your wireless router. How are IP addresses assigned to the five PCs? Does the wireless router use NAT? Why or why not? **(2)**

**5 a)** Compare and contrast the IPv4 and the IPv6 header fields. Do they have any fields in common? Which fields are no longer present in IPv6 datagram? **(2)**

**b)** Is it necessary that every autonomous system use the same intra-AS routing algorithm? Why or why not? **(1.75)**

**c)** Differentiate between RIP and OSPF routing protocol. **(3)**

**d)** How DHCP assign ip address to a newly arriving host? Describe with block diagram. **(2)**

**a)** How big is the MAC address space? The IPv4 address space? The IPv6 address space? **(0.75)**

**b)** Differentiate among CSMA, CSMA/CD and CSMA/CA. **(2)**

**c)** Describe polling and token-passing protocols. Why would the token-ring protocol be inefficient if a LAN had a very large perimeter? **(2)**

**d)** What are the services provided by data link layer (DLL) to network layer. **(2)**

**e)** Why is an ARP query sent within a broadcast frame? Why is an ARP response sent within a frame with a specific destination MAC address? **(2)**

**a)** What do you mean by mobility? Give short note on: mobility via indirect routing and mobility via direct routing. **(2.75)**

**b)** How a mobile agent register it's mobile IP with its home agent? **(2)**

**c)** What are the difference between message confidentiality and message integrity? **(2)**

**d)** Using RSA, choose p=3 and q= 11, and encode the word "hello". Apply the decryption algorithm to the encrypted version to recover the original plaintext message. **(2)**
