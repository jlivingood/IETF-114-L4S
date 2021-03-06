Space, Power, and Networking Needs for IETF-114

Please add your requirements below. 

# Apple
Space: Don't need rack space. Will bring a few laptops, iPhones that can be placed on table.

Power: Standard power needs for small devices

Network: Same as above

# NVIDIA
Space: Don't need rack space. Will bring 2 workstations (client, server) that can be placed on a table.

Power: 2 standard 120V grounded AC connections.

Network: 2 GigE RJ45 connections (1x per workstation), more is better (e.g., for out-of-band management) but not mandatory.

Is the equipment noisy: No.

Other info as needed: Dedicated internet connection via L4S critical path would be useful to test against cloud application.

# Nokia

Space: Don't need rack space. Will bring a few laptops, smartphones, monitor(s) and desktop servers that can be placed on a table/trolley.

Power: US and EU plugs (we can bring adapters and extension cables)

Network: We will bring some simple L2 switches and a WiFi AP.

Is the equipment noisy: No.

# CommScope

Space: TBD it looks like we will bring in our travel mini-rack with the CMTS and servers for DHCP etc. 

Power: 5 120V/15A standard connections (4 for the CMTS mobile rack, 1 for connecting CPEs, laptops etc)

Network: 2 GigE RJ45 connections (1 connection network side of CMTS, other is for any other possible need as backup)

Is the equipment noisy: Yes, the CMTS mobile rack goes in the "NOC" area.

# Casa

Equipment in NOC:
- 1RU - Dell R630 vCCAP server
- 1RU - Dell R650 DHCP/TFTP/ToD/ETC server
- 1RU - FiberStore N5860 ToR Switch/Router
- 1RU - Aruba 2920 Switch - management vlan (hosts/idracs)
- 1RU - ADVA/OSA 5420 PTP Clock

All of the above should be under 10A total.

Equipment at demo station:
- DA1250 RPD - AC wall plug power, need 10G mm Fiber to ToR switch in NOC
- Laptop - need 1G Ethernet cable to Management switch in NOC
- 2 Cable modems - will set up as baseline.

Casa vCCAP L4S/LLD Demo IP Ranges as currently configured:

Aruba switch
used for management all connections in 10.201.15.0/24
this subnet will be private to vccap setup and not visible

ToR switch/router
used for vlan/routing nb/sb
2 connections to vCCAP (CP/DP) vlan trunk (Core/Access/FFE/Mgmt vlans)
2 connections to DHCP/ETC server, 1 Core, 1 Access untagged
1 connection to PTP clock (routed) untagged
K8S uses 10.244.0.0/24 but think it will not be visible
FFE/Mgmt vlans should also not be visible
Core/NSI - 10.79.2.0/24
Access/CIN - 10.78.5.0/24 (DP/RPD)

vCCAP has ip-bundle interface with
10.101.40.0/24 cm
10.101.41.0/24 cpe

PTP Clock - 10.98.5.0/24
routed via ToR

TBD
Northbound interface to "IETF Ethernet" switch

vCCAP and ToR both run ospf



