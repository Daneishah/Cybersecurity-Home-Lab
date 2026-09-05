# Sew4U Academy Access Control Matrix

## Purpose

This document defines role-based access permissions for Sew4U Academy. Access will be granted according to job responsibilities using the principles of least privilege and role-based access control (RBAC).

## Access Levels

- No Access — User cannot access the resource
- Read — User can view information
- Modify — User can create and modify information
- Full Control — User can manage the resource and permissions

## Department Access

| Department | Shared Department Files | Financial Records | HR Records | Program Records | IT Systems |
|---|---|---|---|---|---|
| Executive | Full Control | Read | Read | Read | No Access |
| Human Resources | Read | No Access | Full Control | No Access | No Access |
| Finance & Grants | Read | Full Control | No Access | Read | No Access |
| Programs & Youth Services | Modify | No Access | No Access | Full Control | No Access |
| Sewing / Creative Arts | Modify | No Access | No Access | Modify | No Access |
| Wellness | Modify | No Access | No Access | Modify | No Access |
| Operations | Modify | Read | No Access | Read | No Access |
| IT & Cybersecurity | Read | No Access | No Access | No Access | Full Control |
| Marketing | Modify | No Access | No Access | Read | No Access |
| Volunteers | Read | No Access | No Access | Read | No Access |
| Contractors | Limited | No Access | No Access | Limited | No Access |

## Security Rules

- Access will be assigned through security groups rather than directly to individual users.
- Users will receive only the access necessary to perform their jobs.
- Administrative accounts will be separate from standard user accounts.
- Sensitive HR and financial information will be restricted.
- Employee access will be reviewed when roles change.
- Accounts will be disabled promptly when employees, contractors, or volunteers leave the organization.
- Privileged access will be reviewed regularly.

## Planned Lab Implementation

These permissions will later be implemented using Active Directory security groups, shared folders, NTFS permissions, and Group Policy.

As the lab develops, access will be tested using simulated Sew4U Academy employee accounts to verify that authorized users can access required resources while unauthorized users are denied.
