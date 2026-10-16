# Lab 10: Active Directory Installation

## Objective
Install AD DS Role and promote Server to Domain Controller.

## Steps

### 1. VM Configuration
- Adapter 1: NAT (Internet)
- Adapter 2: Internal Network (lab-net)
- Static IP on Adapter 2: 192.168.10.1

### 2. AD DS Role Installation
- Server Manager → Add Roles and Features
- Role: Active Directory Domain Services
- Install

### 3. Domain Controller Promotion
- Forest: Add a new forest
- Root Domain: lab.local
- Forest Level: Windows Server 2016
- Domain Level: Windows Server 2016
- DNS Server: Yes
- Global Catalog: Yes
- DSRM Password: Admin123!
- Install and Restart

### 4. Verification
- whoami: lab\administrator
- Host Name: DC01
- Primary DNS Suffix: lab.local
- Ethernet 2 IPv4: 192.168.10.1
- DNS Servers: 192.168.10.1

## Key Settings

| Setting | Value |
|---------|-------|
| Domain Name | lab.local |
| NetBIOS Name | LAB |
| DSRM Password | Admin123! |
| Forest Level | Windows Server 2016 |
| Domain Level | Windows Server 2016 |
| Hostname | DC01 |
| IP (Internal) | 192.168.10.1 |
| IP (NAT) | 10.0.2.15 (DHCP) |

## What I Learned
- Active Directory basics
- Domain Controller setup
- Forest and Domain
- VM Network Adapters (NAT + Internal)
- Static IP configuration
- AD DS Role installation
- Domain Controller promotion
- DSRM password