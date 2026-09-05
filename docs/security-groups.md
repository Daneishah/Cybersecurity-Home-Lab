# Sew4U Academy Security Groups

## Purpose

This document defines the planned Active Directory security groups for the simulated Sew4U Academy environment.

Security groups will be used to assign access based on job responsibilities instead of assigning permissions directly to individual users.

## Department Security Groups

| Security Group | Department | Purpose |
|---|---|---|
| SG-Executive | Executive | Executive and organizational resources |
| SG-HumanResources | Human Resources | Employee and HR resources |
| SG-Finance | Finance & Grants | Financial and grant-related resources |
| SG-Programs | Programs & Youth Services | Program and participant resources |
| SG-CreativeArts | Sewing / Creative Arts | Sewing and creative arts resources |
| SG-Wellness | It's Healthy Baby! / Wellness | Wellness program resources |
| SG-Operations | Operations / Facilities | Operational and facilities resources |
| SG-IT | IT & Cybersecurity | IT administration resources |
| SG-Marketing | Marketing / Community Outreach | Marketing and outreach resources |
| SG-Volunteers | Volunteers | Limited volunteer resources |
| SG-Contractors | Contractors | Limited contractor resources |

## Administrative Groups

Additional privileged groups will be created for administrative responsibilities.

- SG-IT-Admins
- SG-HelpDesk
- SG-Server-Admins

Membership in privileged groups will be restricted and reviewed regularly.

## Security Principles

- Users receive access through security group membership.
- Permissions follow the principle of least privilege.
- Department changes require security group membership review.
- Privileged access is separated from standard user access.
- Volunteer and contractor access is limited.
- Access is removed when it is no longer required.

## Planned Implementation

These groups will later be created in Active Directory and connected to folder permissions, organizational units, Group Policy, and other Sew4U Academy resources.

Group membership and permissions will be tested using the simulated user accounts documented in this project.
