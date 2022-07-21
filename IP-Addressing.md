# IETF-114 Router IP addresses

IPv6 = 2001:67c:370::/48 and 2001:67c:1230::/46 

IPv4 = 31.133.128.0/18 and 31.130.224.0/20 

# 3 static addresses (IPv4, IPv6)
We'll assign to each of these routers (1) Casa CMTS, (2) CommScope CMTS, (3) Nokia WiFi Router AP

1. Casa CMTS
* IPv4 31.133.XXX.1 /24, subnet mask 255.255.255.0, static route to 31.133.128.1
* IPv6 unicast is 2001:67c:1230:XXX:XXX:XXX:XXX:XXX, subnet is 2001:67c:1230:XXX::/50 

2. CommScope
* IPv4 31.133.XXX.1 /24, subnet mask 255.255.255.0, static route to 31.133.128.1
* IPv6 unicast is 2001:67c:1230:XXX:XXX:XXX:XXX:XXX, subnet is 2001:67c:1230:XXX::/50

3. Nokia WiFi AP Router
* IPv4 31.133.XXX.1 /24, subnet mask 255.255.255.0, static route to 31.133.128.1
* IPv6 unicast is 2001:67c:1230:XXX:XXX:XXX:XXX:XXX, subnet is 2001:67c:1230:XXX::/50

# DHCP Scopes for clients 
1. Casa
* IPv4 xxx.xxx.xxx.10 - .254, subnet mask 255.255.255.0
* IPv6 2001:67c:1230:XXX::/56
2. CommScope
* IPv4 xxx.xxx.xxx.10 - .254, subnet mask 255.255.255.0
* IPv6 2001:67c:1230:XXX::/56
3. Nokia
* IPv4 xxx.xxx.xxx.10 - .254, subnet mask 255.255.255.0
* IPv6 2001:67c:1230:XXX::/56

# Servers 
1. Casa
* Dell R630 XXX.XXX.XXX.2, subnet mask 255.255.255.0, static route to 31.133.128.1
* Dell R640 XXX.XXX.XXX.3, subnet mask 255.255.255.0, static route to 31.133.128.1
* Clock XXX.XXX.XXX.4, subnet mask 255.255.255.0, static route to 31.133.128.1
* Also available .5 to .9

2. CommScoope 
* DHCP-1 XXX.XXX.XXX.2, subnet mask 255.255.255.0, static route to 31.133.128.1
* DHCP-2 XXX.XXX.XXX.3, subnet mask 255.255.255.0, static route to 31.133.128.1
* Also available .4 to .9

3. Nokia 
* Emulator XXX.XXX.XXX.2, subnet mask 255.255.255.0, static route to 31.133.128.1
* Also available .3 to .9

4. Load/Test Servers
* Nokia App Server xxx.xxx.xxx.2, subnet mask 255.255.255.0 
* FreeBSD Server xxx.xxx.xxx.3, subnet mask 255.255.255.0
* Apple QUIC Server xxx.xxx.xxx.4, subnet mask 255.255.255.0
* PicoQUIC Server xxx.xxx.xxx.5, subnet mask 255.255.255.0
* Nokia App Server xxx.xxx.xxx.6, subnet mask 255.255.255.0
* Nokia Load Server xxx.xxx.xxx.7, subnet mask 255.255.255.0
* Google TCP Server xxx.xxx.xxx.8, subnet mask 255.255.255.0
