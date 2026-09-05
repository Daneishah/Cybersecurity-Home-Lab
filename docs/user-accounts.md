# Sew4U Academy User Accounts

## Purpose

This document defines the simulated employee, contractor, and volunteer accounts that will be used in the Sew4U Academy cybersecurity home lab.

These accounts will later be created in Active Directory and assigned to departments, security groups, and resources according to the principle of least privilege.

## User Accounts

| Name | Username | Department | Role | Account Type |
|---|---|---|---|---|
| Angela Brooks | abrooks | Executive | Executive Director | Employee |
| Marcus Reed | mreed | Human Resources | HR Manager | Employee |
| Jasmine Carter | jcarter | Finance & Grants | Finance Manager | Employee |
| Nicole Davis | ndavis | Programs & Youth Services | Program Director | Employee |
| Tasha Green | tgreen | Sewing / Creative Arts | Sewing Instructor | Employee |
| Maya Thompson | mthompson | It's Healthy Baby! / Wellness | Wellness Coordinator | Employee |
| David Lewis | dlewis | Operations / Facilities | Operations Coordinator | Employee |
| Jordan Smith | jsmith | IT & Cybersecurity | IT Administrator | Employee |
| Kiara Johnson | kjohnson | Marketing / Community Outreach | Marketing Coordinator | Employee |
| Renee Williams | rwilliams | Programs & Youth Services | Volunteer | Volunteer |
| Christopher Brown | cbrown | IT & Cybersecurity | IT Support Technician | Contractor |

## Account Naming Standard

Sew4U Academy user accounts will follow this naming convention:

`first initial + last name`

Example:

`Angela Brooks = abrooks`

## IAM Requirements

- Every user will have an individual account.
- Shared user accounts will not be permitted.
- Users will receive access based on their job responsibilities.
- Users will be assigned to security groups based on department and role.
- Administrative accounts will be separate from standard user accounts.
- Accounts will be disabled when employees, contractors, or volunteers leave the organization.
- Access will be reviewed when a user's role or department changes.
- Password and account lockout policies will be enforced through Group Policy.

## Planned Lab Tasks

- [ ] Create organizational units (OUs)
- [ ] Create department security groups
- [ ] Create employee accounts
- [ ] Create contractor account
- [ ] Create volunteer account
- [ ] Assign users to appropriate security groups
- [ ] Configure role-based permissions
- [ ] Test authorized access
- [ ] Test unauthorized access
- [ ] Disable a terminated employee account
- [ ] Transfer an employee between departments
- [ ] Reset a user's password
- [ ] Unlock a locked user account
