VLAN-Based Network Segmentation

This project demonstrates a basic VLAN-based network designed and configured using Cisco Packet Tracer. The network is divided into separate logical groups to improve organization, reduce broadcast traffic, and isolate devices.

Project Objectives

Create separate VLANs for two groups.

Assign switch ports to the correct VLANs.

Configure IPv4 addresses on end devices.

Test communication between devices in the same VLAN.

Verify isolation between devices in different VLANs.

Network Components

1 Cisco 2960 switch

10 PCs

Copper straight-through cables

Technologies Used

Cisco Packet Tracer

Cisco 2960 Switch

VLANs

IPv4 Addressing

LAN Switching

VLAN Structure

VLAN

Group

Devices

VLAN 10

Group 1

PC0-PC3

VLAN 20

Group 2

PC4-PC8

Update the device list or VLAN numbers if your Packet Tracer configuration is different.

Basic Switch Configuration

enable
configure terminal

vlan 10
name GROUP_1

vlan 20
name GROUP_2

interface range fastEthernet 0/1-4
switchport mode access
switchport access vlan 10

interface range fastEthernet 0/5-9
switchport mode access
switchport access vlan 20

end
write memory

Verification Commands

show vlan brief
show interfaces status

Ping can be used to confirm that devices within the same VLAN communicate successfully. Devices in different VLANs cannot communicate unless inter-VLAN routing is configured.

What I Learned

Creating and naming VLANs

Assigning access ports to VLANs

Understanding logical network segmentation

Configuring basic IPv4 addressing

Testing and troubleshooting connectivity

Author

Tarun Rajput
