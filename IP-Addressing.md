# IETF-114 Router IP addresses

IPv6 = 2001:67c:370::/48 and 2001:67c:1230::/46 

IPv4 = 31.133.128.0/18 and 31.130.224.0/20 

# 3 static addresses (IPv4, IPv4)
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
* IPv6 2001:67c:1230:XXX::/48
2. CommScope
* IPv4 xxx.xxx.xxx.10 - .254, subnet mask 255.255.255.0
* IPv6 2001:67c:1230:XXX::/48
3. Nokia
* IPv4 xxx.xxx.xxx.10 - .254, subnet mask 255.255.255.0
* IPv6 2001:67c:1230:XXX::/48

# Servers
Use IPv4 addresses between XXX.XXX.XXX.2 to .9   
