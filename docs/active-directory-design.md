# Sew4U Academy Active Directory Design

## Purpose

This document defines the planned Active Directory structure for the Sew4U Academy cybersecurity home lab.

The goal is to create a realistic identity and access management environment where users, departments, security groups, and permissions can be managed and tested.

## Domain

Domain Name: sew4u.local

The domain will provide centralized authentication and access management for Sew4U Academy users and computers.

## Organizational Units

The following Organizational Units (OUs) will be created:

- Executive
- Human Resources
- Finance & Grants
- Programs & Youth Services
- Sewing / Creative Arts
- Wellness
- Facilities / Operations
- IT & Cybersecurity
- Marketing / Community Outreach
- Contractors
- Volunteers
- Computers
- Servers
- Service Accounts

## Security Groups

Security groups will be used to assign access based on job responsibilities instead of assigning permissions directly to individual users.

Examples include:

- SG-Executive
- SG-HR
- SG-Finance
- SG-Programs
- SG-Sewing
- SG-Wellness
- SG-Facilities
- SG-IT
- SG-Marketing
- SG-Contractors
- SG-Volunteers

## Administrative Accounts

Administrative privileges will be separated from normal user accounts.

IT administrators will use a standard account for everyday work and a separate privileged account when performing administrative tasks.

Example:

Standard account:
jsmith

Administrative account:
adm-jsmith

## Access Control Principles

Sew4U Academy will follow these IAM principles:

- Least privilege
- Role-based access control (RBAC)
- Individual user accounts
- No shared user accounts
- Separate administrative accounts
- Security-group-based permissions
- Regular access reviews
- Disabled accounts for terminated users
- Restricted access for contractors and volunteers

## Lab Implementation

This design will later be implemented in a Windows Server Active Directory lab.

The implementation will include:

1. Installing Windows Server
2. Installing Active Directory Domain Services
3. Creating the Sew4U Academy domain
4. Creating Organizational Units
5. Creating users
6. Creating security groups
7. Assigning users to groups
8. Configuring permissions
9. Joining Windows workstations to the domain
10. Testing authentication and access controls
