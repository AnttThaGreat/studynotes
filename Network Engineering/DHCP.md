#### How DHCP Process works

1. At boot up, a pc sends a DHCP _Discovery packet_ 
normally to the broadcast address: 255.255.255.255:67(UDP)
2. The DHCP server respondes with an _offer packet_ sent to
the MAC requesting server on UDP port 68
3. After receiving the _offer packet_ from the DHCP,
the PC then returns a _request packet_ that asks for the proper IP settings
to the DHCP server.
4. The DHCP responds with an _acknowledgement packet_ which contains
required info.
5. PC changes settings to reflecting information received.

-----
### Components and processes of DHCP

-Ports Used.
- PC sends discovery packet to 255.255.255.255:67(UDP)
- DHCP sends offer packet to PC's MAC address on port 68(UDP)

-Address Scope
- Admin configures IP range that can be used 

-Address Reservations
- admin reserves specific ips for specific mac addresses (L2)
typically for devices that need the same IP address always. I.E
servers and routers
- Can change ip's from a single location. instead of logging in at the PC

-Leases
- Configuration settings are only valid for a set amount of time
- configured by admin

-Options
- default gateway location
- DNS server address(can be more than one)
- time server addresses
- other additional options

-Preferred ip configuration
- A PC can have a preferred IP address
- admin can config DHCP to ignore preferences

