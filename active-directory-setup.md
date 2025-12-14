# Active Directory Setup – Windows Server 2019

## Objective
Deploy a Windows Server 2019 domain controller and configure Active Directory Domain Services (AD DS) and DNS to create a functional Windows domain environment for centralized authentication and management.

---

## Environment
- **Hypervisor:** VMware ESXi 8.0
- **Server OS:** Windows Server 2019
- **Domain Name:** mutoba.local
- **Roles Installed:** Active Directory Domain Services (AD DS), DNS
- **Client OS:** Windows 10 (domain-joined for testing)

---

## Architecture Overview
- One ESXi host running multiple virtual machines
- Dedicated Windows Server 2019 VM as Domain Controller
- DNS integrated with Active Directory
- Centralized user and group management

---

## ESXi Host and Virtual Machines
![ESXi VM Overview](Screenshots/VM.jpeg)

---

## Step 1: Install and Prepare Windows Server 2019
- Created a new virtual machine in VMware ESXi
- Installed Windows Server 2019
- Applied Windows updates
- Renamed server to **DC01**
- Configured a static IP address

---

## Step 2: Install Active Directory Domain Services
- Opened Server Manager
- Added the **Active Directory Domain Services (AD DS)** role
- Installed **DNS Server** role
- Promoted the server to a Domain Controller
- Created a new forest: **mutoba.local**

![Server Manager Roles](Screenshots/ServerManager.jpeg)

---

## Step 3: Verify Active Directory Configuration
- Opened **Active Directory Users and Computers**
- Verified domain structure
- Confirmed default Organizational Units (OUs)
- Validated domain security groups and users

![Active Directory Users and Computers](Screenshots/ActiveDirectory.jpeg)

---

## Step 4: Verify DNS Configuration
- Opened **DNS Manager**
- Confirmed forward lookup zones
- Verified AD-integrated DNS records
- Ensured domain name resolution was functional

![DNS Manager](Screenshots/DNSManager.jpeg)

---

## Skills Demonstrated
- Windows Server 2019 administration
- Active Directory Domain Services (AD DS)
- DNS configuration and troubleshooting
- VMware ESXi virtualization
- Server hardening and network configuration
- Technical documentation and lab validation

---

## Result
Successfully deployed a fully functional Active Directory domain environment with DNS integration, providing centralized authentication, name resolution, and administrative control suitable for enterprise environments.
