# Sew4U Academy User Accounts

## Purpose

This document defines the simulated employee, contractor, and volunteer identities implemented in the Sew4U Academy Active Directory home lab.

The accounts are organized by department and will be used for hands-on IAM and identity governance exercises involving provisioning, RBAC, least privilege, access reviews, transfers, and deprovisioning.

## User Accounts

| Name | Username | Department | Role | Account Type |
|---|---|---|---|---|
| Angela Brooks | abrooks | Executive | Executive Director | Employee |
| Marcus Reed | mreed | Human Resources | HR Manager | Employee |
| Jasmine Carter | jcarter | Finance & Grants | Finance Manager | Employee |
| Nicole Davis | ndavis | Programs & Youth Services | Program Director | Employee |
| Tasha Green | tgreen | Sewing & Creative Arts | Sewing Instructor | Employee |
| Maya Thompson | mthompson | Wellness | Wellness Coordinator | Employee |
| David Lewis | dlewis | Operations & Facilities | Operations Coordinator | Employee |
| Jordan Smith | jsmith | IT & Cybersecurity | IT Administrator | Employee |
| Kiara Johnson | kjohnson | Marketing & Community Outreach | Marketing Coordinator | Employee |
| Renee Williams | rwilliams | Programs & Youth Services | Volunteer | Volunteer |
| Christopher Brown | cbrown | IT & Cybersecurity | IT Support Technician | Contractor |

## Account Naming Standard

Sew4U Academy user accounts follow this naming convention:

`first initial + last name`

Example: `Angela Brooks = abrooks`

## Identity Attributes Implemented

Active Directory user objects have been populated with organizational identity information including:

- Job title
- Department
- Company: Sew4U Academy
- Manager/reporting relationship where applicable

These attributes provide identity context that can later support role-based access, governance decisions, access reviews, and lifecycle automation.

## IAM Requirements

- Every user has an individual account.
- Shared user accounts are not permitted.
- Users receive access based on job responsibilities.
- Users will be assigned to security groups based on department and role.
- Administrative access will be separated from standard access.
- Accounts will be disabled when employees, contractors, or volunteers leave the organization.
- Access will be reviewed when a user's role or department changes.
- Password and account lockout policies will be enforced through Group Policy.

## Lab Tasks

- [x] Create department Organizational Units (OUs)
- [x] Create employee accounts
- [x] Create contractor account
- [x] Create volunteer account
- [x] Enter user job titles
- [x] Enter department and company attributes
- [x] Configure applicable manager/reporting relationships
- [ ] Create department security groups
- [ ] Assign users to appropriate security groups
- [ ] Configure role-based permissions
- [ ] Test authorized access
- [ ] Test unauthorized access
- [ ] Disable a terminated employee account
- [ ] Transfer an employee between departments
- [ ] Perform an access review after a role change
- [ ] Reset a user's password
- [ ] Unlock a locked user account

## Governance Scenarios Planned

Future exercises will use these identities to practice Joiner-Mover-Leaver (JML) processes, access certification/reviews, least-privilege validation, role changes, account deprovisioning, contractor/volunteer restrictions, and audit documentation.
