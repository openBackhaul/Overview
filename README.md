# Overview
This github is for making technology specific extensions to the ONF Core Information Model (ONF TR-512) available.

The following types of extensions are distinguished:
- Interfaces are attached to the LayerProtocol class of the ONF Core IM and they are for managing network layers at the interfaces of devices
- Profiles are attached to the new Profile class of the ONF Core IM and they are for managing functionalities, which are shared by several interfaces of a device
- Connections are attached to the ForwardingDomain, Link or ForwardingConstruct class of the ONF Core IM and they are for documenting topology information of the respective network layer

## Network Layers

### Air
* [**airInterface**](../../../airInterface) : Physical layer of the microwave radio interface

### EthernetContainer
- [ethernetContainer](../../../ethernetContainer) : Transport resource for Ethernet

### HybridMwStructure
* [**hybridMwStructure**](../../../hybridMwStructure) : Structuring of a microwave radio interface into multiple TDM and a single Ethernet segment

### IP
- [ipInterface](../../../ipInterface) : IPv4 interface according to IETF RFC 791

### MAC
- [**macInterface**](../../../macInterface) : Ethernet MAC interface according to IEEE 802.1
- [macFd](../../../macFd) : Potential forwarding (MAC switch) according to IEEE 802.1

### PureEthernetStructure
- [**pureEthernetStructure**](../../../pureEthernetStructure) : Structuring of a microwave radio interface into a single Ethernet segment

### Synchronization
- [synchronization](../../../synchronization) : Synchronization model according to ITU-T G.7721-2018

### TdmContainer
- [**tdmContainer**](../../../tdmContainer) : Transport resource for TDM

### VLAN
- [**vlanInterface**](../../../vlanInterface) : VLAN interfaces (Port) according to IEEE 802.1Q
- [vlanFd](../../../vlanFd) : Potential forwarding (Component) according to IEEE 802.1Q
- [vlanFc](../../../vlanFc) : Actual forwarding (VLAN) according to IEEE 802.1Q

### Wire
- [**wireInterface**](../../../wireInterface) : Physical layer of an Ethernet PHY interface according to IEEE 802.3

## Profiles
- [coChannelProfile](../../../coChannelProfile) : Groups of microwave radio interfaces, which are using the same frequency channel
- [l3vpnProfile](../../../l3vpnProfile) : Layer 3 Virtual Private Networks
- [policingProfile](../../../policingProfile) : 
- [qosProfile](../../../qosProfile) : Quality of Service based on 802.1p, MPLS Exp and IP DSCP
- [wredProfile](../../../wredProfile) : WRED (Weighted Random Early Detection)

## Core
- [core](../../../core) : Core Information Model that consolidates all Interfaces, Profiles and Equipments
- [ltpAugment](../../../ltpAugment) : Technology agnostic amendment to the LogicalTerminationPoint class
- [firmware](../../../firmware) : Information model and RPCs for managing firmware on the device
- [equipment](../../../equipment) : Device Inventory, Device type specific Information and Interface Behavior
- [alarms](../../../alarms) : Centralized representation of alarms

## Controller
- [O1-Controller](../../../o1controller) : OpenDaylight based SDN Controller, which is used in the ONAP project
- [SDN-R](../../../o1controller) : OpenDaylight based SDN Controller, which is used in the ONAP project

## Applications
- [ApplicationPattern](../../../ApplicationPattern) : Basic functions of REST applications

**Tiny Application Controller**
(These repositories are private. If you would like to access, please contact Thorsten Heinze.)
- [RegistryOffice](../../../RegistryOffice) : List of registered applications
- [TypeApprovalRegister](../../../TypeApprovalRegister) : List of approved applications
- [ExecutionAndTraceLog](../../../ExecutionAndTraceLog) : List of records about service requests
- [OamLog](../../../OamLog) : List of records about OAM activities
- [AdministratorAdministration](../../../AdministratorAdministration) : Authenticates OAM of applications
- [ApplicationLayerTopology](../../../ApplicationLayerTopology) : Application network repository
- [OperationKeyManagement](../../../OperationKeyManagement) : Management of API keys

**Data Sanitation and Caching**
- [MediatorInstanceManager](../../../MediatorInstanceManager) : Mediator management
