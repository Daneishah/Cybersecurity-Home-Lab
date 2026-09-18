# Cybersecurity Home Lab

## Overview

This project documents my hands-on cybersecurity learning journey as I build and manage a simulated business IT environment for Sew4U Academy.

The purpose of this lab is to strengthen my practical skills through real-world scenarios instead of only studying concepts. I use this environment to practice system administration, Identity and Access Management (IAM), Identity Governance and Administration (IGA), Active Directory, networking, security, troubleshooting, automation, and cybersecurity fundamentals.

## Areas of Focus

- Identity and Access Management (IAM)
- Ethical hacking and penetration testing in authorized lab environments
- Active Directory attack-and-defense scenarios
- Identity Governance and Administration (IGA)
- Active Directory and Role-Based Access Control (RBAC)
- User lifecycle management and access governance
- Windows Server and Linux administration
- Server and domain hardening
- Network security and segmentation
- VPN / secure remote-access concepts
- Endpoint protection
- Vulnerability management
- Centralized logging, SIEM, and security monitoring
- Incident response and digital forensics
- PowerShell and automation
- Cloud IAM and cloud security concepts
- Troubleshooting and documentation

## Lab Environment

This lab uses Oracle VirtualBox to run multiple systems in a simulated organizational environment.

Current systems include:

- Windows Server domain controller: Sew4U-DC01
- Windows 11 Pro client: Sew4U-CLIENT01 (installation/troubleshooting in progress)
- Active Directory domain: sew4u.local
- Ubuntu Linux virtual machine: Sew4U-Ubuntu-01

The Active Directory environment models Sew4U Academy with departmental Organizational Units, individual user identities, job-role attributes, reporting relationships, and planned security-group-based access controls.

## Free-Tool Commitment

The lab will use free, open-source, community-edition, evaluation, or built-in tools whenever possible. The goal is to build job-ready hands-on skills without requiring paid enterprise lab software.

Planned tools and technologies include:

- Oracle VirtualBox - virtualization platform
- Windows Server Evaluation - Active Directory/domain lab
- Ubuntu Linux - Linux administration and security
- Microsoft Defender Antivirus / Windows Security - endpoint protection
- Windows Defender Firewall - host firewall and policy practice
- Group Policy - domain security configuration and hardening
- PowerShell - IAM administration, auditing, and automation
- OpenVPN Community Edition or WireGuard - VPN / secure remote-access labs
- pfSense CE or OPNsense - virtual firewall, routing, and segmentation
- Nmap - network discovery and authorized lab scanning
- Greenbone/OpenVAS Community Edition - vulnerability scanning
- Wazuh - endpoint/security monitoring and SIEM/XDR practice
- Sysmon - detailed Windows security telemetry
- Wireshark - network traffic analysis
- Microsoft Event Viewer / Windows Event Forwarding - Windows logging and centralized event collection
- Kali Linux - dedicated ethical-hacking / penetration-testing VM for authorized lab targets
- OWASP Juice Shop - intentionally vulnerable web application practice
- Burp Suite Community Edition - web security testing
- GitHub - portfolio and technical documentation

Tool choices may change as the lab grows, but paid software is not required for the planned learning path.

## Current Progress

- [x] Created cybersecurity home lab GitHub repository
- [x] Installed Oracle VirtualBox
- [x] Installed Ubuntu Linux virtual machine
- [x] Built Windows Server environment
- [x] Installed and configured Active Directory Domain Services
- [x] Created the sew4u.local domain
- [x] Created Sew4U Academy organizational structure
- [x] Created department Organizational Units (OUs)
- [x] Created employee, contractor, and volunteer user accounts
- [x] Added job titles, departments, and company attributes to user identities
- [x] Configured manager/reporting relationships for applicable accounts
- [ ] Create and configure department security groups
- [ ] Assign users to appropriate security groups
- [ ] Implement RBAC and least-privilege permissions
- [ ] Complete Sew4U-CLIENT01 Windows 11 Pro build with proper UEFI/TPM/Secure Boot configuration
- [ ] Connect Windows client computers to the domain
- [ ] Practice Joiner-Mover-Leaver identity lifecycle scenarios
- [ ] Perform access reviews and governance scenarios
- [ ] Harden Windows Server and the Active Directory domain
- [ ] Configure endpoint protection and host firewalls
- [ ] Build virtual firewall/network segmentation lab
- [ ] Configure a safe VPN / secure remote-access lab
- [ ] Perform vulnerability scans and remediation
- [ ] Centralize logs and build security-monitoring scenarios
- [ ] Practice incident response and digital-forensics scenarios
- [ ] Practice PowerShell IAM/security automation
- [ ] Build an isolated ethical-hacking practice network
- [ ] Add Kali Linux attacker VM and intentionally vulnerable targets
- [ ] Practice reconnaissance, enumeration, vulnerability validation, and controlled exploitation in the lab
- [ ] Practice Active Directory attack-and-defense scenarios
- [ ] Document findings, remediation, and lessons learned from penetration-testing exercises
- [ ] Expand into cloud IAM and cloud security concepts
- [ ] Build Microsoft Entra ID identity/governance practice scenarios using free capabilities where possible
- [ ] Add carefully controlled cloud labs using free tiers/credits where appropriate

## IAM / IGA Skills Being Practiced

This environment is being developed to practice responsibilities found in IAM Analyst, IAM Engineer, and Identity Governance roles, including identity creation and administration, OU design, user attribute management, department and role assignment, manager/reporting hierarchy configuration, RBAC, security group administration, least privilege, Joiner-Mover-Leaver lifecycle management, access reviews, provisioning/deprovisioning, privileged access concepts, documentation, and audit readiness.

## Ethical Hacking / Attack-and-Defense Focus

The lab is also being developed as a safe, isolated environment for authorized ethical-hacking practice. Offensive exercises will target only systems I own/control or purpose-built vulnerable training targets. The goal is to understand how attacks work so I can better design identity controls, investigate security events, remediate weaknesses, and connect offensive findings back to IAM and governance.

Planned practice includes reconnaissance and enumeration, network/service discovery, web-application testing, vulnerability assessment, Windows/Linux privilege concepts, Active Directory attack paths, authentication and access-control weaknesses, log analysis, detection, remediation, and professional findings documentation.

## Cloud Security Direction

The long-term lab will connect on-premises identity concepts with cloud identity and security. Planned topics include Microsoft Entra ID, cloud users and groups, authentication and MFA concepts, RBAC, least privilege, identity lifecycle/governance, cloud logging, and carefully controlled AWS/cloud-security exercises using free capabilities whenever possible.

## Troubleshooting Standard

Lab documentation distinguishes between **FIXED** (the underlying cause was corrected) and **WORKAROUND** (the immediate problem was bypassed but the root cause remains). Current example: the Sew4U-CLIENT01 Windows 11 TPM/Secure Boot requirement was bypassed during setup after UEFI-related boot/display trouble; the underlying UEFI/TPM/Secure Boot configuration remains unresolved and should be corrected before the client build is considered complete.

## Security Learning Cycle

The lab roadmap follows a practical cycle:

**Build -> Configure Identities -> Control Access -> Harden -> Monitor -> Test Safely -> Detect -> Respond -> Document**

## Documentation

Detailed lab documentation is maintained in the `docs` directory, including the Active Directory design, organization structure, user accounts, IAM plan, security groups, access-control matrix, lab architecture, free-tools roadmap, and troubleshooting log.

## Goal

My goal is to develop practical, job-ready cybersecurity and identity security skills by building, managing, securing, troubleshooting, governing, and documenting a realistic IT environment. The project supports future IAM Analyst, IAM Engineer, Identity Governance/IGA, penetration testing/ethical hacking, cloud security, and broader cybersecurity opportunities while reinforcing skills learned throughout my cybersecurity degree program.
