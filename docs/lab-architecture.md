# Home Lab Architecture

## Purpose

This home lab simulates the Sew4U Academy IT environment so I can practice cybersecurity, IAM/IGA, system administration, networking, hardening, monitoring, and troubleshooting in a controlled environment.

## Virtualization Platform

- Oracle VirtualBox - free virtualization platform

## Current Systems

### Sew4U-Ubuntu-01
- Operating System: Ubuntu Linux
- Purpose: Linux administration, command-line practice, networking, logging, security, and hardening
- Status: Installed and updated

### Sew4U-DC01
- Operating System: Windows Server 2025 Evaluation
- Purpose: Active Directory Domain Services, user/group management, permissions, Group Policy, IAM, IGA, auditing, and domain security
- Domain: sew4u.local
- Status: Installed; AD domain and identity structure implemented

### Windows Client
- Purpose: Domain-joined workstation for practicing authentication, permissions, endpoint controls, Group Policy, IAM tickets, and troubleshooting
- Status: Planned

## Planned Security Components - Free Tools

- Microsoft Defender Antivirus / Windows Security - endpoint protection
- Windows Defender Firewall - host-based firewalling
- Group Policy - centralized domain/security configuration
- PowerShell - administration, IAM reporting, auditing, and automation
- pfSense CE or OPNsense - virtual firewall/router and network segmentation
- WireGuard or OpenVPN Community Edition - VPN / secure remote access
- Nmap - authorized lab discovery/scanning
- Greenbone/OpenVAS Community Edition - vulnerability management
- Wazuh - centralized security monitoring / SIEM-XDR practice
- Sysmon - enhanced Windows telemetry
- Windows Event Forwarding / Event Viewer - Windows logging
- Wireshark - packet/network analysis
- Kali Linux - controlled security-testing VM when needed

## Skills Practiced / Planned

- Identity and Access Management (IAM)
- Identity Governance and Administration (IGA)
- Active Directory and RBAC
- Windows Server Administration
- Linux Administration and CLI
- Joiner-Mover-Leaver lifecycle management
- Access reviews and least privilege
- Server/domain hardening
- Endpoint security
- Network segmentation and firewalling
- VPN / secure remote access
- Vulnerability management
- Security monitoring / SIEM
- Incident response and digital forensics
- PowerShell automation
- Cloud IAM concepts
- Troubleshooting and technical documentation

## Lab Progress

- [x] Install Oracle VirtualBox
- [x] Install/update Ubuntu Linux VM
- [x] Build Windows Server VM
- [x] Install Active Directory Domain Services
- [x] Create sew4u.local domain
- [x] Create final departmental OU structure
- [x] Create user identities
- [x] Populate job title, department, company, and manager attributes
- [ ] Create security groups
- [ ] Assign users to groups and implement RBAC
- [ ] Build Windows client VM
- [ ] Join Windows client to domain
- [ ] Harden domain/server and endpoint settings
- [ ] Add firewall/network segmentation lab
- [ ] Add safe VPN/remote-access lab
- [ ] Add vulnerability-management lab
- [ ] Add centralized logging/security monitoring
- [ ] Run incident-response scenarios
- [ ] Practice PowerShell automation
- [ ] Expand into cloud IAM

## Architecture Principle

Security components will be added in stages. The lab will prioritize free tools, realistic scenarios, safe isolation, repeatable hands-on practice, and documentation of both successful configurations and troubleshooting lessons.
