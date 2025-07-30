# Active Directory Home Lab Project (GUI-Based)

## Objective
To set up an Active Directory Domain Services (AD DS) environment using Windows Server 2019 in VirtualBox using only the graphical user interface.

## Tools Used
- VirtualBox
- Windows Server 2019
- Active Directory Users and Computers (ADUC)

## What I Did
1. Installed Windows Server in VirtualBox.
2. Configured static IP.
3. Installed and promoted AD Domain Services.
4. Created domain: Lab.local
5. Created Organizational Units (HR Manager, HR Users)
6. Created users manually using the GUI.
7. Created groups and assigned users.
8. Attempted client login - initially failed due to DNS/network issue, but successfully logged in after troubleshooting.
## Outcome
Successfully created a domain and user structure. Learned AD basics and GUI usage.

## Screenshots
See screenshots folder for setup steps.

## Issues Faced
At first, I was unable to log in with the created domain user from the Windows 10 client machine. The login attempt failed due to a DNS/network misconfiguration.

### Causes:
- The client's DNS was not pointing to the Domain Controller IP
- VirtualBox networking was set to NAT instead of Internal or Host-Only
- The client was not joined correctly to the domain

### Resolution:
After reconfiguring the DNS settings on the client and switching the network mode in VirtualBox, I was able to successfully log in with the domain user account.

---

This troubleshooting experience helped me better understand how domain authentication depends on correct DNS and network configuration.

## GitHub Purpose
Sharing my home lab work as part of my learning journey in IT and system administration.
