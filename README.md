# 🌐 Azure Networking Lab: Multi-Region Office Connectivity

A hands-on Azure networking lab focused on designing and implementing secure, multi-region connectivity that simulates an on-premises enterprise environment running in the cloud.

This lab models how organizations with multiple physical offices can extend and interconnect their networks in Azure while maintaining secure, reliable communication across regions.

## ✨ Technologies
  - Microsoft Azure
  - Azure Virtual Networks (VNets)
  - VNet Peering
  - Azure Networking & Routing concepts
  - Multi-region architecture (East US & West US)

## 🚀 Features
  - Simulated on-premises infrastructure hosted in Azure
  - Three interconnected data centers across two Azure regions:
    - New York (East US)
    - Boston (East US)
    - Seattle (West US)
  - Mesh-style network connectivity between offices
  - Secure inter-office communication design
  - Focus on networking architecture rather than resource sprawl

## 🧠 The Process
This lab started with a realistic enterprise scenario:
multiple offices, geographically separated, that must communicate as if they were on the same wide-area network.

Instead of focusing on individual Azure resources, the goal was to understand how networking decisions shape reliability, performance, and security in a multi-region environment.

By designing connectivity between East US and West US regions, I explored how Azure networking abstractions can replicate traditional on-premises WAN designs while offering cloud-native flexibility.

The emphasis was on connectivity, routing, and trust boundaries, not just clicking through the portal. 

## 🧪 What I Learned
How to design multi-region network topologies in Azure
  - The tradeoffs between regional latency and connectivity
  - How mesh-style networking improves redundancy
  - Why network architecture should be planned before deploying workloads
  - How on-premises concepts translate into cloud-native designs
This lab reinforced that cloud networking is still networking — just with different primitives.

## 🧭 Architecture Overview
  - Two offices deployed in East US to represent regional proximity
  - One office deployed in West US to represent cross-country connectivity
  - All offices connected in a mesh topology to allow direct communication
  - Secure routing paths established between all locations

<img width="1658" height="2540" alt="Network_Diagram" src="https://github.com/user-attachments/assets/220d2a9b-d733-4598-8eeb-6ac388288180" />
