# Windows Server 2019 – Active Directory Lab

## Environment
- Hypervisor: VMware ESXi 8.0
- Server OS: Windows Server 2019
- Domain Name: mutoba.local
- Roles Installed: AD DS, DNS
- Client OS: Windows 10 (domain-joined)

---

## Architecture Overview
- One ESXi host running multiple VMs
- Dedicated Domain Controller (DC01)
- DNS integrated with Active Directory
- Centralized identity management

---

## ESXi Host and Virtual Machine
![ESXi Host and VM](Screenshots/VM.jpeg)

---

## Step 1: Server Preparation
- Installed Windows updates
- Renamed server to **DC01**
- Configured static IP address
- Verified network connectivity

---

## Step 2: Install Active Directory Domain Services
- Opened Server Manager
- Installed **Active Directory Domain Services (AD DS)**
- Installed **DNS Server**
- Promoted server to Domain Controller
- Created new forest: **mutoba.local**

### Server Manager
![Server Manager](Screenshots/Server%20Manager.jpeg)

---

## Step 3: Verify Active Directory Configuration
- Opened **Active Directory Users and Computers**
- Verified domain structure
- Confirmed default OUs
- Validated users and security groups

### Active Directory Users and Computers
![Active Directory](Screenshots/Active%20Directory.jpeg)

---

## Step 4: Verify DNS Configuration
- Opened DNS Manager
- Confirmed forward lookup zones
- Verified AD-integrated DNS records
- Tested name resolution

### DNS Manager
![DNS Manager](Screenshots/DNS%20Manager.jpeg)

---

## Skills Demonstrated
- Windows Server administration
- Active Directory Domain Services (AD DS)
- DNS configuration & troubleshooting
- VMware ESXi virtualization
- Technical documentation

---

## Result
Successfully deployed a fully functional Active Directory domain with DNS integration in a virtualized ESXi environment.
