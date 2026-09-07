# Sew4U Academy Active Directory Design

## Purpose

This document defines the Active Directory structure implemented for the Sew4U Academy cybersecurity home lab.

The goal is to create a realistic identity and access management environment where users, departments, security groups, permissions, lifecycle events, and governance controls can be managed and tested.

## Domain

**Domain Name:** sew4u.local

The domain provides centralized authentication and identity administration for Sew4U Academy users and computers.

## Organizational Structure

Under the Sew4U Academy structure, user identities are organized into departmental OUs:

- Executive
- Human Resources
- Finance & Grants
- Programs & Youth Services
- Sewing & Creative Arts
- Wellness
- Operations & Facilities
- IT & Cybersecurity
- Marketing & Community Outreach

Additional organizational containers include:

- Computers
- Groups
- Service Accounts

## User Identity Implementation

Simulated employee, contractor, and volunteer accounts have been created and placed into their appropriate departmental OUs.

Identity attributes configured include job title, department, company, and applicable manager/reporting relationships. This creates a foundation for future IAM and IGA exercises.

## Security Groups

Security groups will be used to assign access based on job responsibilities instead of assigning permissions directly to individual users.

Planned examples include:

- SG-Executive
- SG-HR
- SG-Finance
- SG-Programs
- SG-Sewing
- SG-Wellness
- SG-Operations
- SG-IT
- SG-Marketing
- SG-Contractors
- SG-Volunteers

## Administrative Accounts

Administrative privileges will be separated from normal user accounts as the lab progresses.

IT administrators will use a standard identity for everyday work and a separate privileged identity for administrative tasks.

Example:

Standard account: `jsmith`

Administrative account: `adm-jsmith`

## IAM and Governance Principles

Sew4U Academy will follow these principles:

- Least privilege
- Role-Based Access Control (RBAC)
- Individual user identities
- No shared user accounts
- Separate privileged administrative accounts
- Security-group-based permissions
- Joiner-Mover-Leaver lifecycle management
- Regular access reviews and certification
- Timely deprovisioning of terminated users
- Restricted contractor and volunteer access
- Documentation for audit and governance purposes

## Implementation Status

1. [x] Install Windows Server
2. [x] Install Active Directory Domain Services
3. [x] Create the sew4u.local domain
4. [x] Create Sew4U Academy OU structure
5. [x] Create user accounts
6. [x] Populate job title, department, and company attributes
7. [x] Configure applicable manager/reporting relationships
8. [ ] Create security groups
9. [ ] Assign users to groups
10. [ ] Configure role-based permissions
11. [ ] Join Windows workstations to the domain
12. [ ] Test authentication and access controls
13. [ ] Perform Joiner-Mover-Leaver scenarios
14. [ ] Perform identity governance and access-review scenarios
