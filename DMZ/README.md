# DMZ Purpose

A DMZ (Demilitarized Zone) is a separate network used for public-facing systems such as web servers. Its purpose is to prevent a compromised server from directly accessing the internal LAN.

add another network adapter to pfsense configure DMZ.

LAN : 192.168.10.0/24
DMZ : 192.168.20.0/24
Ubuntu web server : 192.168.20.10
pfsense DMZ gateway: 192.168.20.1

## Firewall Policy
|--|--|
|LAN -> DMZ web server| Allowed on TCP 80/443|
|DMZ -> Internet| Allowed|
|DMZ -> LAN| Blocked and logged|
|WAN -> DMZ| Blocked by default|



The testing confirmed that CLIENT01 could access the Nginx website, while Ubuntu could not access the internal LAN. This demonstrates network segmentation, routing, firewall rules, logging, and protection of internal systems.
