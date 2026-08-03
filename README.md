# Microsoft Intune Device Management & Endpoint Security Lab

   ![Microsoft Intune](https://img.shields.io/badge/Microsoft%20Intune-Endpoint%20Management-blue)
   ![Microsoft Entra ID](https://img.shields.io/badge/Microsoft%20Entra%20ID-Identity%20Management-purple)
   ![Windows 11](https://img.shields.io/badge/Windows%2011-Endpoint%20Management-blue)
   ![Endpoint Security](https://img.shields.io/badge/Endpoint-Security-green)

---


<img width="1912" height="920" alt="intune-dashboard png" src="https://github.com/user-attachments/assets/369971d1-b4d5-40ff-8a0e-52f80df49f86" />



# Project Overview

This project demonstrates the deployment and management of Windows endpoints using **Microsoft Intune** integrated with **Microsoft Entra ID**.

The objective of this hands-on lab was to simulate a real-world enterprise endpoint management environment where administrators can securely manage devices, enforce security policies, deploy applications, configure endpoint protection, manage updates, and perform remote administrative actions.

The lab focuses on practical skills used by:

- IT Support Specialists
- Endpoint Administrators
- Microsoft 365 Administrators
- Junior Systems Administrators
- Junior Cybersecurity Analysts

---

# Project Objectives

The goals of this project were to:

- Configure Microsoft Intune for cloud-based endpoint management
- Integrate Intune with Microsoft Entra ID
- Enrol Windows devices into Intune
- Create device compliance policies
- Configure endpoint security settings
- Deploy applications to managed devices
- Manage Windows Update policies
- Perform remote device management actions
- Monitor device compliance and deployment status

---

# Technologies Used

| Technology | Purpose |
|------------|---------|
| Microsoft Intune | Cloud endpoint management |
| Microsoft Entra ID | Identity and device management |
| Microsoft 365 Admin Centre | Licence management |
| Windows 11 Pro | Managed endpoint |
| Oracle VirtualBox | Virtualisation platform |
| Microsoft Defender | Endpoint protection |
| Windows Defender Firewall | Device security |
| BitLocker | Device encryption |
| Microsoft Store Apps | Application deployment |
| Windows Update Rings | Update management |

---

# Lab Environment

## Cloud Environment

| Component | Details |
|-----------|---------|
| Identity Provider | Microsoft Entra ID |
| Device Management Platform | Microsoft Intune |
| Management Portal | Microsoft Intune Admin Centre |
| Licence | Microsoft Intune Plan 1 Trial |

---

## Endpoint Environment

| Component | Details |
|-----------|---------|
| Operating System | Windows 11 Pro |
| Device Type | Managed corporate endpoint |
| Virtualisation | Oracle VirtualBox |
| Device Join Type | Microsoft Entra ID Joined |
| Management Status | Intune Enrolled |

---

# Lab Architecture


                   Microsoft 365 Tenant
                            |
                            |
                 Microsoft Entra ID
              Identity & Device Management
                            |
                            |
                   Microsoft Intune
              Cloud Endpoint Management
                            |
        ----------------------------------------
        |                   |                   |
        |                   |                   |
     Compliance        Security Policies     Application
     Policies          Configuration         Deployment
        |                   |                   |
        ----------------------------------------
                            |
                            |
                   Windows 11 Endpoint
                            |
         ----------------------------------------
         |                  |                   |
    Windows Updates   Remote Actions      Device Monitoring




---


# Project Implementation Overview

The lab was completed through the following stages:

1. Microsoft Intune Environment Setup
2. Windows Device Enrolment
3. Device Compliance Configuration
4. Endpoint Security Configuration
5. Application Deployment
6. Windows Update Management
7. Remote Device Management
8. Monitoring and Reporting

Detailed implementation notes, screenshots, and configuration settings are available in:

documentation/Intune-Lab-Technical-Report.md

## Repository Structure
Microsoft-Intune-Device-Management-Lab/

    ├── README.md
    │
    ├── screenshots/
    │   ├── intune-dashboard.png
    │   ├── device-enrolment.png
    │   ├── compliance-policy.png
    │   ├── endpoint-security.png
    │   ├── application-deployment.png
    │   ├── update-management.png
    │   └── monitoring.png
    │
    └── documentation/
    └── Intune-Lab-Technical-Report.md

---

# Project Implementation

## Phase 1 — Microsoft Intune Environment Setup

The Microsoft cloud environment was prepared for endpoint management by configuring Microsoft Intune and integrating it with Microsoft Entra ID.

### Tasks Completed

- Activated Microsoft Intune Plan 1 Trial
- Verified Microsoft Intune Admin Centre access
- Confirmed Microsoft Entra ID integration
- Created test users
- Assigned required Intune licences

### Outcome

The environment was successfully prepared for managing Windows devices through cloud-based endpoint management.

📸 **Evidence**

      screenshots/
      ├── intune-dashboard.png
      ├── entra-user-management.png
      └── intune-license.png



---

# Phase 2 — Windows Device Enrolment

A Windows 11 Pro virtual machine was configured as a managed corporate endpoint.

The device was joined to Microsoft Entra ID and enrolled into Microsoft Intune, allowing administrators to apply policies, deploy applications, and manage security settings remotely.

### Tasks Completed

- Installed Windows 11 Pro
- Configured Microsoft Entra ID Join
- Enrolled device into Microsoft Intune
- Verified device registration
- Confirmed device visibility in Intune inventory

### Outcome

The Windows endpoint became available for centralised cloud management.

📸 **Evidence**

      screenshots/
      ├── windows-device.png
      ├── entra-device-registration.png
      └── intune-device-inventory.png


---

# Phase 3 — Device Compliance Policy

A Windows compliance policy was created to ensure managed devices meet organisational security requirements.

## Policy Created

**Windows Security Compliance Policy**

### Security Controls Implemented

- Password protection requirements
- BitLocker encryption requirement
- Microsoft Defender Antivirus requirement
- Firewall protection requirement
- Device security validation

### Assignment

Target:
All Users


### Purpose

The compliance policy ensures that devices meet minimum security standards before being considered compliant within the organisation.

📸 **Evidence**


      screenshots/
      ├── compliance-policy.png
      ├── compliance-settings.png
      └── compliance-assignment.png


---

# Phase 4 — Endpoint Security Configuration

An Endpoint Protection configuration profile was created to strengthen Windows security settings across managed devices.

## Configuration Profile

**Windows Endpoint Security Baseline**

### Security Features Configured

### Microsoft Defender

Configured:

- Microsoft Defender protection
- SmartScreen security settings
- Malware protection controls

### Windows Firewall

Enabled:

- Domain firewall
- Private firewall
- Public firewall

### Device Encryption

Configured:

- BitLocker encryption requirements
- Encryption settings for managed devices

### Assignment


Target:
All Devices


### Purpose

This configuration establishes a security baseline for Windows endpoints by enforcing protection against malware, unauthorised access, and data exposure.

📸 **Evidence**


      screenshots/
      ├── endpoint-security-profile.png
      ├── defender-settings.png
      └── firewall-configuration.png


---

# Phase 5 — Application Deployment

Microsoft Intune was used to deploy applications remotely to managed Windows devices.

## Application Deployed

**Company Portal**

### Deployment Method


Microsoft Store app (new)


### Assignment


Required Installation

Target:
All Devices


### Purpose

This demonstrates how administrators can centrally deploy software across an organisation without requiring manual installation on each endpoint.

📸 **Evidence**

<img width="1919" height="922" alt="application-deployment-status png" src="https://github.com/user-attachments/assets/bf23889b-fb53-4fdf-b561-ca0d2792990f" />
<img width="1019" height="770" alt="Company Portal App on CL PC" src="https://github.com/user-attachments/assets/30e4dbe5-061d-4719-a4db-a3a4374848d7" />


      screenshots/
      ├── company-portal-app.png
      ├── application-assignment.png
      └── application-deployment-status.png

---

# Phase 6 — Windows Update Management

Microsoft Intune Update Rings were configured to manage Windows update deployment across managed devices.

The goal was to simulate an enterprise update strategy where security updates are deployed in a controlled manner while reducing disruption to users.

## Update Ring Created

**Corporate Windows Update Policy**

### Configuration Highlights

- Microsoft product updates enabled
- Windows driver updates enabled
- Quality update deferral configured
- Feature update deferral configured
- Automatic update installation configured
- Active hours configured
- Update deadlines configured

### Assignment
Target:
All Devices


### Purpose

This demonstrates practical experience with enterprise patch management and controlling how Windows updates are deployed across an organisation.

📸 **Evidence**


    screenshots/
    ├── windows-update-policy.png
    ├── update-ring-assignment.png
    └── update-ring-summary.png


---

# Phase 7 — Remote Device Management

Microsoft Intune provides administrators with remote management capabilities for troubleshooting, maintenance, and device lifecycle management.

The following remote actions were tested:

## Device Sync

Forced the Windows endpoint to immediately check for:

- New policies
- Configuration changes
- Application deployments

**Use case:**

Helpful when administrators need devices to receive updates without waiting for the normal synchronisation cycle.

---

## Remote Restart

Performed a remote restart action on the managed Windows device.

**Use case:**

Useful after:

- Software installations
- Security policy changes
- Troubleshooting activities

---

## Retire Device

Tested the device retirement process to remove organisational management while preserving personal user data.

The Retire action removes:

- Intune management
- Corporate policies
- Organisation-related applications
- Work account access

The action does not remove:

- Personal files
- Personal applications
- Windows operating system

**Use case:**

Commonly used during:

- Employee offboarding
- BYOD device removal
- Device replacement scenarios

📸 **Evidence**

    screenshots/
    ├── remote-device-actions.png
    └── retire-device.png


---

# Phase 8 — Monitoring and Reporting

After deploying policies, applications, and security configurations, Intune monitoring tools were used to verify deployment status and device health.

## Monitoring Areas Reviewed

### Device Compliance

Reviewed:

- Compliance status
- Policy evaluation
- Device health information

---

### Configuration Profiles

Verified:

- Endpoint security profile deployment
- Policy assignment status
- Deployment results

---

### Application Deployment

Monitored:

- Company Portal deployment status
- Installation results
- Application assignment

---

### Device Inventory

Reviewed:

- Enrolled devices
- Operating system information
- Device management status
- Last check-in information

📸 **Evidence**

    screenshots/
    ├── compliance-monitoring.png
    └──  configuration-profile-status.png
     
    




---

# Challenges & Troubleshooting

During the implementation of this lab, several common enterprise endpoint management scenarios were encountered.

## Device Compliance Showing "Not Evaluated"

### Issue

After creating compliance policies, the device did not immediately display a compliance status.

### Resolution

- Verified Intune enrolment status
- Confirmed policy assignments
- Performed manual device synchronisation
- Allowed time for compliance evaluation

---

## Configuration Profile Deployment Delay

### Issue

Security configuration policies did not immediately apply to the managed endpoint.

### Resolution

- Verified device assignment
- Triggered an Intune sync
- Restarted the endpoint
- Confirmed deployment status in Intune monitoring

---

## Application Deployment Delay

### Issue

The Company Portal application did not immediately install after deployment.

### Resolution

- Confirmed application assignment
- Verified device check-in
- Performed manual synchronisation
- Monitored installation progress

---
# Skills Demonstrated

## Microsoft Intune Administration

- Windows device enrolment
- Compliance policy management
- Configuration profile deployment
- Application deployment
- Windows Update Ring configuration
- Remote device administration

---

## Microsoft Entra ID Administration

- Device registration
- Identity integration
- User and licence management

---

## Endpoint Security

- Microsoft Defender configuration
- Windows Firewall management
- BitLocker encryption enforcement
- Endpoint security hardening
- Device compliance enforcement

---

## IT Support & Administration

- Remote device troubleshooting
- Software deployment
- Policy troubleshooting
- Windows endpoint management
- Enterprise device lifecycle management



---

# Future Improvements

Future enhancements planned for this lab include:

- Implementing Conditional Access policies
- Integrating Microsoft Defender for Endpoint
- Deploying PowerShell scripts through Intune
- Configuring Windows Autopilot
- Implementing Endpoint Privilege Management
- Deploying security baselines
- Integrating Microsoft Sentinel for security monitoring



---

# Author

**Ayodeji Olumide Awe**

**CompTIA Security+ Certified**

Aspiring **IT Support Specialist | Endpoint Administrator | Cybersecurity Professional**

Hands-on experience with:

- Microsoft Intune
- Microsoft Entra ID
- Windows Administration
- Endpoint Security
- SIEM Monitoring
- Vulnerability Management

---

# Project Summary

This project demonstrates the end-to-end management of Windows endpoints using Microsoft Intune and Microsoft Entra ID.

The lab covers device enrolment, compliance enforcement, endpoint security configuration, application deployment, Windows update management, remote administration, and monitoring.

It reflects real-world tasks performed by IT Support Specialists, Endpoint Administrators, and Microsoft 365 Administrators in modern cloud-managed environments.
