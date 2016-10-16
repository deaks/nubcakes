# ICMP, UDP, TCP, and Packet Capture

This module continues to explore the basic protocols used in computer
networks by delving into ICMP, UDP, and TCP with a brief introduction to
packet captures.


## Internet Control Message Protocol (ICMP)

ICMP ECHO_REQUEST, ECHO_REPLY, and "ping"

brief discussion of latency


## User Datagram Protocol (UDP)

connection-less, unreliable transmission, simple


## deaks corner -- UDP in practice

often used where low-latency is required including some types of
near-real-time data transmission where missing a packet means that the
data from that missing packet can be safely ignored

applications to video games and audio/video streaming protocols


## Transmission Control Protocol (TCP)

connection oriented, reliable transmission, more complex,
SYN/ACK/SYN-ACK three-way handshake, bind-listen/accept and CONNECT,
retransmission and ACKs


## deaks corner -- TCP in practice

application protocols {ssh, http/https, rdp, vnc}, managing latency and
retransmission, managing ACK overhead


## deaks corner -- frequency spectrum and the FCC

brief description of frequency spectrum with overview showing viewable

description of the role of the FCC and associated spectrum licensing
diagram


## deaks corner -- applications to satellite communication

used everywhere/everyday by almost everyone

characterized by high latency limited by the speed of light for
electrical propagation through a medium (fiber, air, wire) and
relatively long distances between satellite and ground locations as
well as two-way travel

characterized by high bandwidth at typical operation frequencies (C, L,
Ku, Ka bands)

long-fat pipes (high latency and high bandwidth) typical with satellite
communication limits interaction so many satellite systems tend toward
1:many relationships and use subscriber side decoders to isolate
specific channels of interest while all channels are sent all the time

optimize for long-fat pipes with UDP using custom application protocols
to manage data in flight vs. bandwidth and implement a negative ACK
scheme/protocol


## deaks corner -- firewalls, TCP, and UDP

brief discussion of firewalls, their purpose and configuration

difference of firewall traversal with TCP and connection tracking


## Packet Capture

introduction to the concept of capturing and even replaying sequences
of packets

brief discussion of wireshark, tshark, tcpdump, tcpreplay

brief discussion of netfilter, ethernet promiscuity, and the fact that
captures occur at layer 1 and can ignore higher layer filtering that
normally restricts the packets our applications can interact with,
usage to "see" packets arriving at a host even if they are not allowed
through the local firewall
