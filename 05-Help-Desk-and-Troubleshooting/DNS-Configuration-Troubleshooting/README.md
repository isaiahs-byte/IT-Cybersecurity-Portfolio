# DNS Configuration & Troubleshooting Lab

## Lab Overview

This lab demonstrates DNS configuration, troubleshooting, and verification within a Windows Server Active Directory environment.

The purpose of this project was to practice:
- DNS zone management
- Name resolution testing
- DNS troubleshooting
- Command-line diagnostics
- Network configuration repair
- Help desk and system administration troubleshooting procedures

This lab was performed using Windows Server and Active Directory integrated DNS services.

---

# Technologies Used

- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS Manager
- Command Prompt
- TCP/IP Configuration
- Microsoft Hyper-V / Azure VM Environment

---

# Environment Information

| System | Hostname | IP Address |
|---|---|---|
| Domain Controller | DC1 | 10.0.0.4 |
| Client Machine | CLIENT01 | 10.0.0.5 |

Domain Name:

```text
lab.local
```

---

# Objectives

- Verify DNS zone configuration
- Test internal DNS resolution
- Test external DNS resolution
- Simulate DNS misconfiguration
- Troubleshoot DNS issues
- Restore DNS functionality
- Verify successful DNS repair

---

# DNS Configuration Verification

The DNS Manager console was opened to verify the Active Directory integrated forward lookup zone and DNS records.

## DNS Manager

![DNS Manager](screenshots/01_DNS_Manager_Opened.png)

---

## Forward Lookup Zone

![Forward Lookup Zone](screenshots/02_Forward_Lookup_Zone_Visible.png)

---

## DNS Records

![DNS Records](screenshots/03_DNS_Records_Inside_Forward_Zone.png)

---

## Domain Controller DNS Settings

![Domain Controller DNS Settings](screenshots/04_Domain_Controller_DNS_IP_Settings.png)

---

# DNS Resolution Testing

DNS resolution testing was performed using the `nslookup` command.

## DC1 DNS Resolution

![DC1 NSLookup](screenshots/05_NSLookup_DC1_Success.png)

---

## CLIENT01 DNS Resolution

![CLIENT01 NSLookup](screenshots/06_NSLookup_CLIENT01_Success.png)

---

## External DNS Resolution

![Google DNS Resolution](screenshots/07_NSLookup_Google_Success.png)

---

# DNS Troubleshooting Simulation

A DNS misconfiguration was intentionally created by changing the DNS server to an incorrect external DNS address.

This simulated a real-world troubleshooting scenario commonly encountered in help desk and system administration environments.

---

## Incorrect DNS Configuration

![Incorrect DNS Configuration](screenshots/08_Incorrect_DNS_Server_Configured.png)

---

## DNS Test with Incorrect DNS Configuration

![DNS Test Incorrect Configuration](screenshots/09_NSLookup_DC1_With_Incorrect_DNS_Config.png)

---

## DNS Misconfiguration Identified

![DNS Misconfiguration Identified](screenshots/10_DNS_Misconfiguration_Identified.png)

---

# DNS Repair Process

The DNS server settings were corrected and DNS cache was flushed to restore proper name resolution functionality.

---

## DNS Server Restored

![DNS Server Restored](screenshots/11_DNS_Server_Restored_Correctly.png)

---

## DNS Cache Flushed

![DNS Cache Flushed](screenshots/12_DNS_Cache_Flushed_After_Repair.png)

---

## DNS Functionality Restored

![DNS Functionality Restored](screenshots/13_DNS_Functionality_Restored.png)

---

# DNS Service Verification

The DNS service status was verified after troubleshooting was completed.

---

## DNS Service Running

![DNS Service Running](screenshots/14_DNS_Service_Running.png)

---

# Skills Demonstrated

- DNS administration
- Active Directory DNS integration
- Internal hostname resolution
- External DNS testing
- DNS troubleshooting
- TCP/IP configuration management
- Windows command-line diagnostics
- Network troubleshooting
- IT help desk troubleshooting workflow
- System administration fundamentals

---

# Outcome

This lab successfully demonstrated the ability to configure, test, troubleshoot, and repair DNS functionality within a Windows Active Directory environment.

The project also demonstrated practical help desk troubleshooting methodology and system administration diagnostic procedures.
