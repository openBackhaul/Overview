# Overview
This github is for making technology specific extensions to the ONF Core Information Model (ONF TR-512) available.

The following types of extensions are distinguished:
- Interfaces are attached to the LayerProtocol class of the ONF Core IM and they are for managing network layers at the interfaces of devices
- Profiles are attached to the new Profile class of the ONF Core IM and they are for managing functionalities, which are shared by several interfaces of a device
- Connections are attached to the ForwardingDomain, Link or ForwardingConstruct class of the ONF Core IM and they are for documenting topology information of the respective network layer

## Network Layers

### Air
- [airInterface](../../../airInterface) : Physical layer of the microwave radio interface
- [airLink](../../../airLink) : Potential forwarding on the physical layer of microwave transport
- [airFc](../../../airFc) : Actual forwarding on the physical layer of the radio connection

### EthernetContainer
- [ethernetContainer](../../../ethernetContainer) : Transport resource for Ethernet

### HybridMwStructure
- [hybridMwStructure](../../../hybridMwStructure) : Structuring of a microwave radio interface into multiple TDM and a single Ethernet segment

### IP
- [ipInterface](../../../ipInterface) : IPv4 interface according to IETF RFC 791

### MAC
- [macInterface](../../../macInterface) : Ethernet MAC interface according to IEEE 802.1
- [macFd](../../../macFd) : Potential forwarding according to IEEE 802.1

### PureEthernetStructure
- [pureEthernetStructure](../../../pureEthernetStructure) : Structuring of a microwave radio interface into a single Ethernet segment

### TdmContainer
- [tdmContainer](../../../tdmContainer) : Transport resource for TDM

### VLAN
- [vlanInterface](../../../vlanInterface) : VLAN interfaces according to IEEE 802.1Q
- [vlanFc](../../../vlanFc) : Actual forwarding according to IEEE 802.1Q
- [vlanFd](../../../vlanFd) : Potential forwarding according to IEEE 802.1Q

### Wire
- [wireInterface](../../../wireInterface) : Physical layer of an Ethernet PHY interface according to IEEE 802.3
- [wireFc](../../../wireFc) : Actual forwarding on the physical layer of Ethernet according to IEEE 802.3
- [wireLink](../../../wireLink) : Potential forwarding on the physical layer of Ethernet according to IEEE 802.3
- [wireEquipment](../../../wireEquipment) : Equipment for an Ethernet PHY interface according to IEEE 802.3

## Profiles
- [aclProfile](../../../aclProfile) : Access Control Lists
- [coChannelProfile](../../../coChannelProfile) : Groups of microwave radio interfaces, which are using the same frequency channel
- [l3vpnProfile](../../../l3vpnProfile) : Layer 3 Virtual Private Networks
- [policingProfile](../../../policingProfile) : Traffic Policing
- [qosProfile](../../../qosProfile) : Quality of Service based on 802.1p, MPLS Exp and IP DSCP
- [wredProfile](../../../wredProfile) : WRED (Weighted Random Early Detection)

## Core
- [core](../../../core) : Core Information Model that consolidates all Interfaces, Profiles and Equipments
