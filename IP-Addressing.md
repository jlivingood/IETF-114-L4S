IPv4 /22
IPv6 /48

IETF-114 Router
IPv6 = 2001:67c:370::/48 and 2001:67c:1230::/46 
IPv4 = 31.133.128.0/18 and 31.130.224.0/20 

3 static addresses (IPv4, IPv4), which we'll assign to each of these routers (1) Casa CMTS, (2) CommScope CMTS, (3) Nokia WiFi Router AP
1. Casa CMTS: IPv4 xxx.xxx.xxx.1, subnet mask 255.255.252.0, static route to 31.133.128.1 and IPv6 unicast is 2001:67c:1230:XXX:XXX:XXX:XXX:XXX, subnet is 2001:67c:1230:XXX::/64 eui-64
2. CommScope: IPv4 xxx.xxx.xxx.2, subnet mask 255.255.252.0, static route to 31.133.128.1 and IPv6 unicast is 2001:67c:1230:XXX:XXX:XXX:XXX:XXX, subnet is 2001:67c:1230:XXX::/64 eui-64
8. Nokia WiFi AP Router: IPv4 xxx.xxx.xxx.3, subnet mask 255.255.252.0, static route to 31.133.128.1 and IPv6 unicast is 2001:67c:1230:XXX:XXX:XXX:XXX:XXX, subnet is 2001:67c:1230:XXX::/64 eui-64

DHCP Scopes for clients 
1. Casa DHCP scopes: xxx.xxx.xxx.10 - 254, subnet mask 255.255.255.0, 001:67c:1230::/48
2. CommScope DHCP scopes: xxx.xxx.xxx.10 - 254, subnet mask 255.255.255.0, 001:67c:1230::/48
3. Nokia DHCP scopes: xxx.xxx.xxx.10 - 254, subnet mask 255.255.255.0, 001:67c:1230::/48

For any servers - use IPv4 addresses between XXX.XXX.XXX.2 to .9   
