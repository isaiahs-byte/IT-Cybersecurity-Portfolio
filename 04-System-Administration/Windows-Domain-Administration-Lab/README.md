# Windows Domain Administration Lab

## Lab Overview
This lab demonstrates Windows Active Directory domain administration tasks using Microsoft Azure virtual machines. The environment includes a Domain Controller and a Windows client machine joined to the domain.

---

## Skills Demonstrated
- Active Directory Domain Services (AD DS)
- Domain user account creation
- Security group management
- Group Policy configuration
- Account lockout policy configuration
- Domain join process
- Windows administration
- Remote Desktop Protocol (RDP)
- Help desk style account troubleshooting

---

## Environment
| System | Purpose |
|---|---|
| DC1 | Domain Controller |
| CLIENT01 | Windows 11 Client |
| Azure | Cloud hosting platform |

---

## Tasks Completed
- Created Active Directory users
- Created security groups
- Added users to groups
- Joined Windows client to domain
- Configured account lockout policy
- Forced Group Policy update with gpupdate /force
- Tested domain authentication
- Verified domain membership

---

## Screenshots
Screenshots for this lab are stored in the screenshots folder.

---

## Commands Used

```powershell
gpupdate /force

---

This lab provided hands-on experience with enterprise Windows domain administration and common help desk account management tasks using Active Directory and Group Policy.
