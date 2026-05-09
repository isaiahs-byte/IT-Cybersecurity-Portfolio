# Windows Domain Administration Lab

## Project Overview

This project demonstrates hands-on Windows Server and Active Directory administration skills using Microsoft Azure virtual machines. The lab environment included a Domain Controller (DC1) and a Windows 11 client machine joined to the lab.local domain.

The project focused on enterprise identity management, Group Policy administration, account security policies, user administration, and domain management tasks commonly performed in help desk and junior system administrator roles.

---

# Environment

| System | Purpose |
|---|---|
| DC1 | Windows Server Domain Controller |
| CLIENT01 | Windows 11 Domain Client |
| Microsoft Azure | Cloud virtualization platform |
| Active Directory | Identity and access management |
| Group Policy | Security policy management |

---

# Skills Demonstrated

- Active Directory Domain Services (AD DS)
- Domain user account administration
- Security group creation and management
- Group Policy configuration
- Account lockout policy deployment
- Windows domain join operations
- Remote Desktop Protocol (RDP)
- Help desk troubleshooting workflows
- Windows administration
- Azure virtual machine administration

---

# Lab Tasks Completed

## 1. Initial Server Configuration
- Configured Windows Server virtual machine
- Verified server connectivity
- Prepared Active Directory environment

![Server Overview](screenshots/01_Server_LocalServer_Overview.png)

---

## 2. Active Directory Overview
- Opened Active Directory Users and Computers
- Verified domain structure
- Reviewed organizational hierarchy

![ADUC Overview](screenshots/02_ADUC_Domain_Overview.png)

---

## 3. Created New Domain User
- Created domain user account
- Configured account settings
- Verified successful user creation

![New User Created](screenshots/03_New_User_Account_Creation.png)

---

## 4. Created Additional User Accounts
- Added additional domain users
- Simulated enterprise user onboarding

![User Account Created](screenshots/04_User_Account_Created.png)

---

## 5. Created Security Groups
- Created Active Directory security groups
- Configured permissions structure

![Security Group Created](screenshots/05_Security_Group_Creation.png)

---

## 6. Additional Group Management
- Continued security group configuration
- Organized domain access structure

![Additional Group Creation](screenshots/06_Security_Group_Created.png)

---

## 7. Added Users to Security Groups
- Assigned domain users to security groups
- Verified membership configuration

![User Added To Group](screenshots/07_User_Added_To_Security_Group.png)

---

## 8. Opened Group Policy Management
- Accessed Group Policy Management Editor
- Navigated account security settings

![Group Policy Management](screenshots/08_GroupPolicy_Management.png)

---

## 9. Configured Account Lockout Policies
- Configured account lockout threshold
- Configured lockout duration
- Configured reset timer policies

![Group Policy Editor](screenshots/09_GroupPolicy_Editor_Open.png)

---

## 10. Applied Account Lockout Security Policy
- Enabled account lockout protections
- Verified policy configuration

![Account Lockout Policy](screenshots/10_Account_Lockout_Policies.png)

---

## 11. Tested Account Lockout Functionality
- Simulated failed authentication attempts
- Verified security policy enforcement

![Account Lockout Test](screenshots/11_Account_Lockout_Threshold.png)

---

## 12. Forced Group Policy Update
- Executed gpupdate /force
- Verified successful policy application

![Group Policy Update](screenshots/12_GroupPolicy_Update_Forced.png)

---

# Commands Used

## Force Group Policy Update

```powershell
gpupdate /force
```

## Run Command As Domain User

```cmd
runas /user:lab.local\JohnSmith cmd
```

---

# Troubleshooting Encountered

## RDP Authentication Issues
During the project, Remote Desktop credential caching and Azure RDP configuration created authentication issues when attempting to switch between local and domain accounts.

## Azure VM Session Handling
Azure virtual machines automatically reconnect to previously authenticated sessions, which prevented traditional multi-user Windows login screen behavior from appearing.

## Group Policy Propagation
After configuring account lockout policies, Group Policy updates needed to be manually forced using:

```powershell
gpupdate /force
```

to ensure policy deployment across the environment.

---

# Key Takeaways

This project provided practical experience with:
- Enterprise Windows administration
- Active Directory management
- Security policy deployment
- Identity and access management
- Help desk troubleshooting workflows
- Azure cloud infrastructure administration

The lab simulated real-world junior system administrator and help desk tasks commonly performed in enterprise IT environments.

---

# Future Improvements

- Implement Organizational Units (OUs)
- Configure Group Policy Objects (GPOs)
- Deploy roaming profiles
- Implement password complexity policies
- Add PowerShell automation
- Configure shared folders and NTFS permissions
- Expand environment with additional client systems
