# Notes

* All devices must respond to pings
* Set whatever DNS/NTP servers you like: IETF network is 2001:67c:370:229::6 & 31.130.229.6 and 2001:67c:370:229::7 & 31.130.229.7 
* Important: Send MAC addresses of the routers to Clemens at csch@kiez.net in order for routing to be activated!

# IETF-114 Router IP addresses

* IPv6 = 2001:67c:1230:601::1
* IPv4 = 31.130.239.1

# Addressing Scheme

1. Casa 

1.1 CMTS
* Send MAC address of interface to Clemens at csch@kiez.net in order for routing to be activated
* IPv4 31.130.239.17/24, subnet mask 255.255.255.0, static default route to 31.130.239.1
* IPv6 unicast is 2001:67c:1230:601::17/64, static default route to 2001:67c:1230:601::1

1.2 DHCP Scopes for Clients
* IPv4 (from 31.133.188.0/24) 31.133.188.10 - .254, subnet mask 255.255.255.0, route to 31.130.239.17
* IPv6 2001:67c:1233:4000::/50 (hand out /56 prefix to each CM), route to 2001:67c:1230:601::17

1.3 Servers
* Option to use SLAAC/DHCP
* Dell R630 31.133.188.2, subnet mask 255.255.255.0, static default route to 31.130.239.1
* Dell R640 31.133.188.3, subnet mask 255.255.255.0, static default route to 31.130.239.1
* Clock 31.133.188.4, subnet mask 255.255.255.0, static default route to 31.130.239.1
* Also available .5 to .9

2. CommScope

2.1 CMTS
* Send MAC address of interface to Clemens at csch@kiez.net in order for routing to be activated
* IPv4 31.130.239.18/24, subnet mask 255.255.255.0, static route to 31.130.239.1
* IPv6 unicast is 2001:67c:1230:601::18/64, static default route to 2001:67c:1230:601::1

2.2 DHCP Scope for Clients
* IPv4 (from 31.133.189.0/24) 31.133.189.10 - .254, subnet mask 255.255.255.0, route to 31.130.239.18
* IPv6 2001:67c:1233:8000::/50 (hand out /56 prefix to each CM), route to 2001:67c:1230:601::18

2.3 Servers
* Option to use SLAAC/DHCP
* DHCP-1 31.133.189.2, subnet mask 255.255.255.0, static default route to 31.130.239.1
* DHCP-2 31.133.189.3, subnet mask 255.255.255.0, static default route to 31.130.239.1
* Also available .4 to .9

3. Nokia 

3.1 WiFi AP Router
* Send MAC address of interface to Clemens at csch@kiez.net in order for routing to be activated
* IPv4 31.130.239.19/24, subnet mask 255.255.255.0, static default route to 31.130.239.1
* IPv6 unicast is 2001:67c:1230:601::19/64, static default route to 2001:67c:1230:601::1

3.2 DHCP Scope for Clients
* IPv4 (from 31.133.190.0/24) 31.133.190.10 - .254, subnet mask 255.255.255.0, route to 31.130.239.19
* IPv6 2001:67c:1233:c000::/50 (hand out /56 prefix to each AP), route to 2001:67c:1230:601::19

3.3 Servers
* Option to use SLAAC/DHCP
* Emulator 31.133.190.2, subnet mask 255.255.255.0, static default route to 31.130.239.1
* Also available .3 to .9

4. Load/Test Servers: USE SLAAC / DHCP
* Nokia App Server 
* FreeBSD Server 
* Apple QUIC Server 
* PicoQUIC Server 
* Nokia App Server 
* Nokia Load Server 
* Google TCP Server 
* CableLabs Network Monitor Server 
