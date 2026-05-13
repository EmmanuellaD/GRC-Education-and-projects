# NIST CSF 2.0 Home Network Cybersecurity Assessment

## Overview

This project applies the **NIST Cybersecurity Framework 2.0** to a personal home network in order to assess cybersecurity maturity, identify security gaps, and create practical recommendations for improvement.

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

The objective of this project is to:

- Assess the cybersecurity posture of a home network using NIST CSF 2.0.
- Create an asset inventory of connected devices.
- Evaluate current security practices using a maturity scoring model.
- Identify gaps in governance, protection, detection, response, and recovery.
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
