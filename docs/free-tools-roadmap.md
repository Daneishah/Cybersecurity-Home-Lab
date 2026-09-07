# Sew4U Academy Free Tools & Security Roadmap

## Purpose

This document tracks the free tools planned for the Sew4U Academy cybersecurity home lab. The goal is to gain substantial hands-on experience without paying for enterprise lab software.

## Current Core Lab

| Tool / Technology | Cost | Purpose | Status |
|---|---|---|---|
| Oracle VirtualBox | Free | Run virtual machines | In use |
| Windows Server Evaluation | Free evaluation | Active Directory, Group Policy, Windows Server administration | In use |
| Ubuntu Linux | Free / open source | Linux administration, CLI, permissions, logging, hardening | In use |
| GitHub | Free tier | Portfolio and technical documentation | In use |
| PowerShell | Built in / free | Windows and IAM administration and automation | Planned practice |

## IAM / Identity Governance

| Tool / Technology | Purpose |
|---|---|
| Active Directory Domain Services | Users, groups, authentication, OUs, domain identity |
| Active Directory Users and Computers | Provisioning, attributes, managers, group membership, lifecycle tasks |
| Group Policy | Password/account policies, security configuration, centralized controls |
| PowerShell | Bulk provisioning, reporting, group administration, audits, automation |
| Microsoft Entra concepts/free options when available | Cloud identity, MFA, SSO, Conditional Access concepts |

## Server / Domain Protection

- Microsoft Defender Antivirus / Windows Security
- Windows Defender Firewall
- Group Policy security settings
- Windows Update / patch management practice
- Windows auditing and Event Viewer
- Microsoft security baseline concepts
- Sysmon for enhanced Windows telemetry

## Network Security / VPN

- pfSense Community Edition or OPNsense for virtual firewalling, routing, and network segmentation
- WireGuard or OpenVPN Community Edition for secure remote-access/VPN practice
- Wireshark for packet capture and network analysis
- Nmap for authorized discovery and scanning inside the lab

## Vulnerability Management

- Greenbone/OpenVAS Community Edition for vulnerability scanning
- Nmap for service discovery and validation
- Windows/Linux patching and configuration remediation

## Logging / SIEM / Monitoring

- Wazuh for security monitoring and SIEM/XDR practice
- Sysmon for Windows event telemetry
- Windows Event Viewer
- Windows Event Forwarding for centralized Windows logs
- Linux system/authentication logs

## Incident Response / Forensics

- Built-in Windows and Linux logs
- Wireshark
- Sysmon
- Wazuh alerts/events
- Additional free forensic tools can be added when those labs begin

## Controlled Security Testing

- Kali Linux when a dedicated testing VM is needed
- Nmap and other free tools used only inside the authorized home-lab environment

## Roadmap Rule

Tools will be installed only when they support the current learning phase. The lab will not add software simply to make the environment larger. Each tool should support a real scenario, produce a documented result, and reinforce IAM, governance, networking, system security, monitoring, vulnerability management, or incident-response skills.

## Planned Progression

1. Finish Active Directory security groups and RBAC.
2. Build identity lifecycle and IGA scenarios.
3. Harden the Windows Server/domain and Ubuntu system.
4. Add endpoint and firewall protections.
5. Build virtual firewall and segmentation scenarios.
6. Add VPN / secure remote access safely.
7. Add vulnerability scanning and remediation.
8. Centralize logging and monitoring.
9. Run controlled detection and incident-response scenarios.
10. Add PowerShell automation and cloud IAM concepts.
