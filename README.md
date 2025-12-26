# ☁️ Distributed Infrastructure in Azure: Secure App & Data Segmentation

A hands-on Azure project demonstrating distributed infrastructure design, focused on network segmentation, secure access, and separation of application and data layers within a virtual network.

This project models how real-world environments isolate workloads while maintaining controlled connectivity between tiers.

## ✨ Technologies
  - Microsoft Azure
  - Azure Virtual Network (VNet)
  - Subnets (Application & Data tiers)
  - Network Security Groups (NSGs)
  - Azure Virtual Machines
  - Azure MySQL Flexible Server
  - SSH (TCP Port 22)

## 🚀 Features
  - Distributed application and data tiers within a single Azure VNet
  - Logical network segmentation using dedicated subnets:
    - App Subnet – Application workloads
    - Data Subnet – Database services
  - Secure VM access via SSH from the internet
  - Network Security Groups applied at multiple layers
  - Private connectivity between application and database tiers
  - Persistent storage attached to compute resources

## 🧠 The Process

This project was designed to answer a common infrastructure question:
“How do you securely separate application and data layers in the cloud?”

Using Azure’s networking primitives, I built a distributed layout where compute, storage, and database services are isolated by subnet boundaries and protected with security rules.

Rather than exposing everything publicly, access is intentionally limited:
- External access is restricted to SSH
- Database resources remain isolated in a dedicated data subnet
- Traffic flow is controlled through NSGs instead of implicit trust
The emphasis was on defense-in-depth and least privilege networking, not just deploying services.

## 🧪 What I Learned
  - How to design segmented network architectures in Azure
  - Why separating app and data tiers reduces blast radius
  - Practical use of Network Security Groups for traffic control
  - How cloud networking mirrors traditional on-prem designs
  - The importance of planning network boundaries before deploying workloads
This reinforced that secure infrastructure starts with network design, not tooling.

## 🧭 Architecture Overview
  - Virtual Network hosting all resources
  - App Subnet
    - Linux VM (devapp_VM)
    - Attached disks for persistence
    - Network Interface (devNIC)
    - NSG controlling inbound/outbound traffic
  - Data Subnet
    - Azure MySQL Flexible Server
    - Restricted access from application tier only
    - Dedicated NSG
  - External Access
    - SSH (TCP 22) permitted from the internet to the application VM only
