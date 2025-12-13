# Active Directory Setup – Windows Server 2019

## Objective
Deploy Windows Server 2019 and configure Active Directory Domain Services (AD DS)
to create a functional domain environment for user authentication and management.

## Environment
- Hypervisor: VMware ESXi
- Server OS: Windows Server 2019
- Domain Name: mutoba.local
- Roles Installed: AD DS, DNS

## Step 1: Install Windows Server
- Created a virtual machine in ESXi
- Installed Windows Server 2019
- Applied updates
- Renamed server to DC01
- Configured a static IP address

## Step 2: Install Active Directory Domain Services
- Opened Server Manager
- Added AD DS role
- Verified successful installation

## Step 3: Promote to Domain Controller
- Created a new forest: mutoba.local
- Configured DSRM password
- Restarted the server

## Step 4: Verify Configuration
- Confirmed domain in Active Directory Users and Computers
- Verified DNS forward lookup zone
- Tested authentication

## Step 5: Create Users and Groups
- Created Organizational Units (OUs)
- Added test users
- Assigned users to security groups

## Skills Demonstrated
Windows Server • Active Directory • DNS • VMware ESXi • Documentation
