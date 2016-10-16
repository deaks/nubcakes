UDP and TCP

UDP/IP: connection-less, unreliable transmission, simple

deaks on UDP in practice: low latency for real-time transmission (if you miss something, it is too late anyway so no sense in sending you a copy of the event), video games, audio/video streaming

TCP/IP: connection oriented, reliable transmission, more complex, SYN/ACK/SYN-ACK three-way handshake, bind-listen/accept and CONNECT, retransmission and ACKs

deaks on TCP in practice: application protocols {ssh, http/https, rdp, vnc},  managing latency and retransmission, managing ACK overhead

deaks on satellite communication: used everywhere/everyday by almost everyone, characterized by high latency limited by the speed of light for electrical propagation through a medium (fiber, air, wire) and relatively long distances between satellite and ground locations as well as two-way necessity; characterized by high bandwidth at typical operation frequencies; high latency and high bandwidth limits interaction so many satellite systems tend toward 1: many relationships and use subscriber side decoders to isolate specific channels of interest while all channels are sent all the time

deaks on winning with UDP: long-fat pipes (high latency, high bandwidth) may use UDP with custom negatice ACK protocol to manage interactivity efficiently
