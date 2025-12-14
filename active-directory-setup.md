# Windows Server Active Directory Lab

## Environment Details

- **Hypervisor:** VMware ESXi 8.0
- **Server OS:** Windows Server 2019
- **Domain Name:** mutoba.local
- **Roles Installed:** Active Directory Domain Services (AD DS), DNS
- **Client OS:** Windows 10 (domain-joined)

---

## Architecture Overview

- Single ESXi host running multiple VMs
- Dedicated Domain Controller (DC01)
- DNS integrated with Active Directory
- Centralized user and group management

---

## ESXi Host and Virtual Machines

![ESXi Host and VM](Screenshots/vm.jpeg)

---

## Step 1: Server Preparation

- Installed Windows Server 2019
- Applied Windows Updates
- Renamed server to **DC01**
- Configured a static IP address
- Verified network connectivity

---

## Step 2: Install Active Directory Domain Services

- Opened Server Manager
- Added **Active Directory Domain Services (AD DS)** role
- Installed **DNS Server** role
- Promoted server to Domain Controller
- Created a new forest: **mutoba.local**

### Server Manager Roles

![Server Manager](Screenshots/server-manager.jpeg)

---

## Step 3: Verify Active Directory Configuration

- Opened **Active Directory Users and Computers**
- Verified domain structure
- Confirmed default Organizational Units (OUs)
- Validated users and security groups

### Active Directory Users and Computers

![Active Directory Users and Computers](Screenshots/active-directory.jpeg)

---

## Step 4: Verify DNS Configuration

- Opened **DNS Manager**
- Confirmed forward lookup zones
- Verified AD-integrated DNS records
- Tested domain name resolution

### DNS Manager

![DNS Manager](Screenshots/dns-manager.jpeg)

---

## Skills Demonstrated

- Windows Server 2019 administration
- Active Directory Domain Services (AD DS)
- DNS configuration and troubleshooting
- VMware ESXi virtualization
- Server hardening and network configuration
- Technical documentation

---

## Result

Successfully deployed a fully functional Active Directory domain environment with integrated DNS, centralized identity management, and enterprise-ready configuration.
