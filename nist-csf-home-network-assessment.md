# NIST CSF 2.0 Home Network Cybersecurity Assessment

## Overview

This project applies the **NIST Cybersecurity Framework 2.0** to a personal home network to assess cybersecurity maturity, identify security gaps, and create practical recommendations for improvement.

The assessment reviews internet-connected devices, wireless security, account protection, device management, monitoring, incident response, and recovery readiness.

## About NIST CSF 2.0

The NIST Cybersecurity Framework helps organizations understand, manage, and reduce cybersecurity risk. It is organized around six core functions:

| Function | Description |
|---|---|
| Govern | Establish cybersecurity strategy, policies, roles, responsibilities, and risk management processes. |
| Identify | Understand assets, systems, data, users, business risks, and dependencies. |
| Protect | Implement safeguards such as access controls, MFA, encryption, patching, and secure configurations. |
| Detect | Monitor systems and activities to identify suspicious behavior, vulnerabilities, and security events. |
| Respond | Create and follow plans to contain, investigate, and manage cybersecurity incidents. |
| Recover | Restore systems, data, and operations after an incident while improving future resilience. |

## Project Objective

- Assess the cybersecurity posture of a home network using NIST CSF 2.0.
- Create an inventory of connected devices.
- Evaluate current security practices using a maturity scoring model.
- Identify gaps across governance, protection, detection, response, and recovery.
- Develop practical recommendations to improve home network security.

## Scope

This assessment focuses on:

- Home Wi-Fi and network devices
- Laptops, desktop, tablets, and mobile phones
- Smart home and IoT devices
- Account security and MFA
- Device updates and patching
- Security alerts and monitoring
- Backup and recovery readiness
- Incident response preparation

## Asset Inventory

| Asset | Type | Owner | Data Stored / Processed | Criticality | Notes |
|---|---|---|---|---|---|
| Laptop 1 | Endpoint | Household member | Personal files, work files | High | Used for daily work and personal activity |
| Laptop 2 | Endpoint | Household member | Personal files, work files | High | Used for daily work and personal activity |
| Desktop | Endpoint | Household member | Personal files, work files | High | Used for personal and work-related activity |
| Cellphone 1 | Mobile endpoint | Me | Email, banking apps, MFA, personal apps | High | Used for sensitive accounts |
| Cellphone 2 | Mobile endpoint | Household member | Email, banking apps, personal apps | High | Used for sensitive accounts |
| Smart TV | IoT device | Household | Streaming account access | Medium | Connected to home Wi-Fi |
| Tablet 1 | Mobile endpoint | Me | Email, apps, cloud files, browsing data, photos | High | Used for personal accounts and cloud access |
| Tablet 2 | Mobile endpoint | Household member | Email, apps, cloud files, browsing data, photos | High | Used for personal accounts and cloud access |
| Tablet 3 | Mobile endpoint | Household member | Apps, browsing data, photos | Medium | Lower sensitivity than primary devices |
| Router | Network device | Household | Network traffic | High | Provides internet connectivity |
| Google Nest | Network / smart home device | Household | Network connectivity and device traffic | High | Main connection point for household devices |

## Network Overview

The home network includes laptops, mobile phones, tablets, smart devices, a router, and a Google Nest environment. Trusted personal devices and smart home devices currently operate within the same general home network environment.

A future improvement is to separate trusted devices, guest devices, and IoT devices where technically possible.

```text
Internet
   |
Router / Google Nest
   |
Home Wi-Fi Network
   |
------------------------------------------------
| Laptops | Desktop | Phones | Tablets | Smart TV |
```

## Maturity Scoring Scale

| Score | Maturity Level | Description |
|---|---|---|
| 1 | Initial | Not documented or inconsistent |
| 2 | Developing | Some practices exist, but they are informal |
| 3 | Defined | Process exists and is mostly consistent |
| 4 | Managed | Process is documented, monitored, and reviewed |
| 5 | Optimized | Process is mature, measured, and continuously improved |

## NIST CSF Assessment

| NIST Function | Area Reviewed | Current State | Score | Gap / Improvement |
|---|---|---|---|---|
| Govern | Security rules | Security practices are informal and not documented. | 2 | Create a home cybersecurity checklist. |
| Identify | Asset inventory | Devices are known but not fully documented. | 3 | Complete an inventory of devices, accounts, and critical data. |
| Protect | Wi-Fi security | WPA2/WPA3 is enabled, and the network uses a password. | 4 | Review router firmware and admin settings. |
| Protect | MFA | MFA is enabled on some critical accounts. | 3 | Enable MFA on all important accounts. |
| Protect | Device updates | Most devices receive automatic updates. | 4 | Document update status for all devices. |
| Protect | IoT separation | Smart devices are connected to the same Wi-Fi environment through Google Nest. | 3 | Monitor the Nest network periodically and consider network separation where available. |
| Detect | Alerts and monitoring | Some login and antivirus alerts exist, but reviews are not scheduled. | 2 | Enable alerts and review account and device activity seasonally. |
| Respond | Incident response | No written incident response plan exists. | 1 | Create a response checklist for common incidents. |
| Recover | Backups | Some files are backed up, but recovery has not been tested. | 3 | Test file restoration and document recovery steps. |

## Maturity Score Calculation

The overall maturity score was calculated by averaging the individual assessment scores.

```text
Govern: 2
Identify: 3
Protect - Wi-Fi security: 4
Protect - MFA: 3
Protect - Device updates: 4
Protect - IoT separation: 3
Detect: 2
Respond: 1
Recover: 3

Total score = 25
Number of assessed areas = 9

25 / 9 = 2.8
```

## Maturity Summary

The home network received an overall NIST CSF maturity score of:

```text
2.8 out of 5
```

This places the home network at the **Developing** maturity level, moving toward **Defined**.

### Strengths

- WPA2/WPA3 Wi-Fi security is enabled.
- The network uses password protection.
- Most devices receive automatic updates.
- MFA is enabled on some critical accounts.
- Household devices are generally known and identified.

### Key Improvement Areas

- Formal cybersecurity checklist or policy
- Complete asset documentation
- MFA coverage across all critical accounts
- Scheduled monitoring and alert review
- Written incident response plan
- Backup restoration testing

## Gap Analysis

| Finding | NIST Function | Current State | Gap | Recommended Improvement | Priority |
|---|---|---|---|---|---|
| Security rules are informal | Govern | Security practices exist but are not documented. | No formal home cybersecurity checklist or policy exists. | Create a simple home cybersecurity checklist covering passwords, MFA, updates, backups, account recovery, and safe device use. | Medium |
| Asset inventory is incomplete | Identify | Devices are known but not fully documented. | There is no complete record of devices, accounts, critical data, owners, update status, and security status. | Complete an inventory of all devices, accounts, and sensitive data, including update status and criticality. | High |
| Router settings need review | Protect | WPA2/WPA3 is enabled and the Wi-Fi network uses a password. | Router firmware and admin settings have not been fully reviewed or documented. | Review router firmware, admin password, DNS settings, guest network settings, and connected devices. | Medium |
| MFA is not fully implemented | Protect | MFA is enabled on some critical accounts. | MFA is not consistently enabled across all important accounts. | Enable MFA on email, cloud storage, banking, social media, password manager, and other high-value accounts. | High |
| Device update tracking is incomplete | Protect | Most devices receive automatic updates. | Devices may be updated, but update status is not fully documented. | Record OS, app, and firmware update status in the asset inventory and review periodically. | Medium |
| IoT devices share the main Wi-Fi environment | Protect | Smart devices are connected through the same Wi-Fi environment via Google Nest. | IoT devices are not clearly separated from personal devices such as laptops, phones, and tablets. | Monitor the Nest network periodically and consider using guest network separation where available. | Medium |
| Monitoring is not scheduled | Detect | Some login and antivirus alerts exist, but reviews are not scheduled. | Security alerts and connected-device reviews are not performed on a routine schedule. | Enable important login alerts and review account activity, antivirus alerts, and connected devices seasonally. | Medium |
| No incident response plan exists | Respond | There is no written incident response plan. | No documented steps exist for responding to account compromise, malware, lost devices, or unknown network activity. | Create a home incident response checklist with steps for identifying, containing, recovering from, and documenting incidents. | High |
| Backup recovery has not been tested | Recover | Some files are backed up, but recovery has not been tested. | Backup reliability is unknown because restore testing has not been performed. | Test restoration of sample files and document backup locations, frequency, and recovery steps. | High |

## Recommended Remediation Plan

| Timeline | Action | NIST Function | Priority |
|---|---|---|---|
| 0-30 Days | Create a home cybersecurity checklist | Govern | Medium |
| 0-30 Days | Complete asset inventory | Identify | High |
| 0-30 Days | Enable MFA on all critical accounts | Protect | High |
| 0-30 Days | Review router firmware and admin settings | Protect | Medium |
| 31-60 Days | Document device update status | Protect | Medium |
| 31-60 Days | Review Google Nest and connected devices | Protect | Medium |
| 31-60 Days | Enable login and account activity alerts | Detect | Medium |
| 31-60 Days | Create an incident response checklist | Respond | High |
| 61-90 Days | Test backup restoration | Recover | High |
| 61-90 Days | Reassess maturity score | Govern | Medium |

## Incident Response Checklist

This checklist provides basic response steps for common home cybersecurity incidents.

### 1. Identify

Examples of incidents:

- Suspicious login alert
- Malware or antivirus warning
- Unknown device connected to Wi-Fi
- Lost or stolen device
- Account compromise

### 2. Contain

Immediate actions:

- Disconnect affected device from Wi-Fi.
- Change passwords from a trusted device.
- Revoke suspicious account sessions.
- Enable MFA if it is not already active.
- Remove unknown devices from the network.

### 3. Eradicate

Follow-up actions:

- Run antivirus or malware scans.
- Remove suspicious apps, extensions, or files.
- Update the operating system and applications.
- Reset compromised passwords.

### 4. Recover

Recovery actions:

- Restore files from backup if needed.
- Confirm accounts are secure.
- Reconnect devices only after they are verified as safe.
- Monitor accounts and devices for additional suspicious activity.

### 5. Lessons Learned

Document:

- What happened
- Which device or account was affected
- What actions were taken
- What control should be improved

## Conclusion

This project demonstrates how NIST CSF 2.0 can be applied to a real-world home network environment. The assessment found that the home network has a solid security foundation, especially in Wi-Fi protection and device updates, but needs improvement in governance, documentation, monitoring, incident response, and recovery testing.

The recommended actions will help improve the home network from a **Developing** maturity level toward a more **Defined** and repeatable cybersecurity posture.
