# Packet Tracer: Create a LAN

## Project Overview
This project demonstrates how to build and configure a small office Local Area Network (LAN) using Cisco Packet Tracer. It covers physical device connections, dynamic and static IPv4 addressing, connectivity verification, DNS resolution, and basic network troubleshooting.

## Objectives
- Connect PCs, a printer, a switch, and a router.
- Configure end devices using DHCP and static IPv4 addressing.
- Verify local network connectivity using ping.
- Test access to an internet server using an IP address and URL.
- Use `ipconfig`, `ipconfig /all`, and `tracert` to inspect network configuration and routing.

## Tools Used
- Cisco Packet Tracer
- Ethernet copper straight-through cables
- IPv4 addressing and subnet masks
- DHCP (Dynamic Host Configuration Protocol)
- DNS (Domain Name System)
- ICMP (Internet Control Message Protocol)

## Network Topology
The simulated office network includes:
- Admin PC
- Manager PC
- Network printer
- Office switch
- Office router
- ISP connection
- Remote web server

## Addressing Configuration
The office LAN uses the `192.168.1.0/24` IPv4 network.

| Device | Addressing Method | IPv4 Address |
|---|---|---|
| Admin PC | DHCP | Dynamically assigned |
| Manager PC | DHCP | Dynamically assigned |
| Printer | Static | `192.168.1.100` |
| Web server | Provided by the activity | `209.165.200.225` |

The PCs receive their IP addresses, subnet masks, default gateways, and DNS settings from DHCP. The printer uses a static IP address so that other devices can reliably reach it.

## Tasks Performed
1. Connected the office router to the ISP and office switch.
2. Connected the Admin PC, Manager PC, and printer to the switch.
3. Configured both PCs to obtain network settings through DHCP.
4. Configured the printer with a static IPv4 address.
5. Tested connectivity to the printer using `ping`.
6. Accessed the remote web server by IP address and URL.
7. Inspected network configuration using `ipconfig` and `ipconfig /all`.
8. Traced the route to a remote destination using `tracert`.

## Commands Used

### Display IP Configuration
```text
ipconfig
ipconfig /all
```

### Test Connectivity
```text
ping 192.168.1.100
```

### Trace the Route to a Remote Server
```text
tracert www.cisco.pt
```

## Key Findings
- Devices on the same subnet can communicate through the local network without routing between subnets.
- DHCP simplifies IP address assignment and reduces manual configuration.
- Static addressing makes printers and other shared resources easier to locate.
- DNS translates domain names into IP addresses.
- Ping tests connectivity, while traceroute helps identify the routers along a path.
- A default gateway enables communication with remote networks.

## Skills Demonstrated
- LAN setup and physical connectivity
- IPv4 addressing and subnetting fundamentals
- DHCP and static IP configuration
- DNS troubleshooting
- Connectivity testing with ping
- Route analysis using traceroute
- Basic network administration

## Conclusion
This lab demonstrates how to establish a functional small-office LAN and verify communication between local devices and remote resources. It builds practical knowledge of network addressing, DHCP, DNS, routing, and connectivity troubleshooting.

## Disclaimer
This is a simulated networking exercise completed in Cisco Packet Tracer for educational and portfolio purposes.
