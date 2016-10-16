# Ethernet, Endian-ness, and the Internet Protocol (v4)

This module discusses modern network principles and relies on a previous
treatment of data organization including bits, octets/bytes, as well as
some familiarity with the binary, and hexadecimal number systems.


## OSI Network Model

discussion of layers, relationships, and layer-to-layer communications


## Ethernet

OSI "you are here" diagram inset for all viewgraphs

CSMA/CD protocol and why the addition of "/CD" was important

introduction to shared media interfaces and collisions (hub,
archaic: repeater)

collision avoidance via switching (switch, archaic: bridge)

Ethernet MAC addressing and broadcast, collision/broadcast domain and
the "LAN" concept

data integrity, checksums, CRCs, and message digests (hashes)

Ethernet packet internals diagram


## deaks corner -- pseudocode conventions and metasyntactic variables

`$var`, `{var}`, `<var>`, `A[idx]`,
`M[row][col]` (except FORTRAN and MATLAB, sigh)

`foo`, `bar`, `baz`, `qux`


## Endian-ness

big endian, little endian, bi-endian; archaic: PDP endian


## Internet Protocol version 4

OSI "you are here" diagram inset for all viewgraphs

classical network organization (classful) and modern  (classless, CIDR) subnetting concepts and practice; network/broadcast addresses of a subnet, local broadcast address; private network ranges, network byte order

IPv4 packet internals diagram


## LAN/WAN concepts

routing (router, gateway, default route)


## Dynamic Configuration with IPv4

dhcp, link-local addressing

dhcp packet diagram


## deaks corner -- IPv4 directed broadcast

directed broadcast to a remote subnet, opt-in at switches


## deaks corner -- IPv4 multicast

multicast IP addressing, IGMP, and router interactions

data distribution modes (1:many, many:many) and applications for audio
