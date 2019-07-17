# Overview
This github is for making technology specific extensions to the ONF Core Information Model (ONF TR-512) available.

The following types of extensions are distinguished:
- Interfaces are attached to the LayerProtocol class of the ONF Core IM and they are for managing network layers at the interfaces of devices
- Profiles are attached to the new Profile class of the ONF Core IM and they are for managing functionalities, which are shared by several interfaces of a device
- Connections are attached to the ForwardingDomain, Link or ForwardingConstruct class of the ONF Core IM and they are for documenting topology information of the respective network layer

### Interfaces
- [airInterface](../../../airInterface) : Physical layer of the microwave radio interface
- [ethernetContainer](../../../ethernetContainer) : Transport resource for Ethernet
- [hybridMwStructure](../../../hybridMwStructure) : Structuring of a microwave radio interface into multiple TDM and a single Ethernet segment
- [ipInterface](../../../ipInterface) : IPv4 interface according to IETF RFC 791
- [macInterface](../../../macInterface) : Ethernet MAC interface according to IEEE 802.1
- [pureEthernetStructure](../../../pureEthernetStructure) : Structuring of a microwave radio interface into a single Ethernet segment
- [tdmContainer](../../../tdmContainer) : Transport resource for TDM
- [vlanInterface](../../../vlanInterface) : VLAN interfaces according to IEEE 802.1Q
- [wireInterface](../../../wireInterface) : Physical layer of an Ethernet PHY interface according to IEEE 802.3

### Profiles
- [coChannelProfile](../../../coChannelProfile) : Groups of microwave radio interfaces, which are using the same frequency channel
- [l3vpnProfile](../../../l3vpnProfile) : Layer 3 Virtual Private Networks
- [qosProfile](../../../qosProfile) : Quality of Service based on 802.1p, MPLS Exp and IP DSCP
- [wredProfile](../../../wredProfile) : WRED (Weighted Random Early Detection)

### Connections
- [airConnection](../../../airConnection) : Physical layer of the microwave radio connection
- [vlanConnection](../../../vlanConnection) : VLAN connections according to IEEE 802.1Q
- [wireConnection](../../../wireConnection) : Physical layer of the Ethernet PHY connection according to IEEE 802.3

### Equipment
- [wireEquipment](../../../wireEquipment) : Equipment for an Ethernet PHY interface according to IEEE 802.3

### Core
- [core](../../../core) : Core Information Model that consolidates all Interfaces, Profiles and Equipments
