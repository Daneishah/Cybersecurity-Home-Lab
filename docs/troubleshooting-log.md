# Sew4U Academy Home Lab Troubleshooting Log

## Purpose

This is a running record of roadblocks, mistakes, confusing screens, and technical issues encountered while building the home lab. The goal is to document not only what worked, but how problems were recognized and resolved.

## Earlier Build / Setup Roadblocks

### VirtualBox / VM setup and navigation
- Worked through learning VirtualBox VM creation and the differences between the host PC and guest virtual machines.
- Clarified NAT versus bridged networking and kept the initial lab on a safer/simple virtual networking configuration while the environment was being built.
- Installed VirtualBox Guest Additions on the Windows Server VM to improve usability/display integration.
- Full-screen/display navigation caused some confusion; practiced entering/exiting the VM display modes.

### Windows Server identity / naming
- Windows Server initially used an automatically generated computer name.
- Renamed the server for the Sew4U Academy environment and restarted so the new identity would apply.
- Lesson: establish consistent server naming early because names later appear throughout AD, DNS, documentation, and troubleshooting.

### Active Directory / domain build
- Installed Active Directory Domain Services and built the Sew4U Academy domain.
- Worked through unfamiliar Server Manager and AD administration screens.
- Created the OU structure and later corrected/reorganized it so the live AD structure and GitHub documentation matched.
- Lesson: documentation must follow the final implemented structure, not an outdated draft.

### Linux practice
- Used Ubuntu commands such as `sudo apt update`, `sudo apt upgrade`, `pro status`, `hostname`, and `hostname -I`.
- Chose to perform commands one at a time for now to build Linux/CLI familiarity and repetition rather than relying immediately on combined commands/scripts.

## September 6, 2026 - User Provisioning / IAM Build

### Password-policy rejection while creating users
**Roadblock:** A starter password was rejected while creating an Active Directory user.

**What we learned:** Active Directory password requirements can reject a password that does not satisfy the configured domain policy. The issue was not that the user-creation process was broken.

**Resolution:** Reviewed the domain password-policy requirements and used a compliant starter password. The user account then created successfully.

**Documentation decision:** A consistent lab starter-password process can be used for simulated users as long as it complies with the domain policy. Real organizations should use secure onboarding procedures and require password changes/strong authentication according to policy. Password values themselves should not be stored in a public GitHub repository.

### Finding/searching inside Active Directory windows
**Roadblock:** `Ctrl+F` did not behave as expected in an AD administration window.

**Resolution:** Used the interface's available object-selection/search workflow instead of relying on a browser/editor-style Find shortcut.

**Lesson:** Windows administrative consoles do not always use the same keyboard shortcuts or search behavior as standard applications.

### User/department consistency problem
**Roadblock:** The live AD structure and the earlier GitHub/planning information were temporarily inconsistent. Additional departments/OU names were introduced during the build, including the correct placement of Maya Thompson in Wellness.

**Resolution:** Stopped adding users long enough to reconcile the intended organization structure, then used the final Sew4U Academy department design consistently. GitHub documentation was later corrected to match the implemented lab.

**Lesson:** In IAM work, identity attributes, OU placement, role definitions, and documentation must stay synchronized. Inconsistent source data can cause incorrect access later.

### Role / job-title storage
**Roadblock:** Needed to determine where a user's organizational role should be stored in Active Directory.

**Resolution:** Used the user's Properties / Organization information to record job title, department, company, and manager information.

**Lesson:** Identity attributes provide business context that later supports RBAC, provisioning rules, access reviews, reporting, and governance.

### Manager assignments
**Roadblock:** Needed to determine which users should have managers and how to enter them.

**Resolution:** Used the Manager field in Active Directory user properties and assigned reporting relationships according to the Sew4U Academy structure. Angela Brooks, as Executive Director, remains at the top of the reporting structure.

**Lesson:** Manager data is important in IAM/IGA because it can drive approvals, access reviews, escalation, and lifecycle workflows.

### GitHub repository naming confusion
**Roadblock:** The repository was initially referenced with the wrong name (`Sew4U-Home-Lab`).

**Resolution:** Opened GitHub and confirmed the actual repository is `Daneishah/Cybersecurity-Home-Lab`.

**Lesson:** Verify the exact repository/asset name before performing updates instead of relying on memory.

### GitHub connected but read-only
**Roadblock:** ChatGPT could read the repository, but README updates failed with HTTP 403 / `Resource not accessible by integration`.

**Troubleshooting performed:**
1. Verified the GitHub connector was connected.
2. Confirmed the repository could be read.
3. Tried changing ChatGPT plugin permissions to allow all actions; write still failed.
4. Checked GitHub Authorized Apps / Installed GitHub Apps and discovered the initial authorization did not provide the required repository write path.
5. Reconnected/installed the ChatGPT Codex Connector with repository read/write access.
6. Re-tested repository permissions.

**Resolution:** The GitHub connector gained push/write access. README and documentation updates then completed successfully.

**Lesson:** A connector can be authenticated and able to read data while still lacking permission to modify it. Authentication and authorization are separate troubleshooting checks.

## Completed at End of Session

- All planned Sew4U Academy users created.
- Users placed in the final department OUs.
- Job titles/roles entered.
- Department and company attributes entered.
- Applicable manager relationships configured.
- GitHub write access repaired.
- README, user-account documentation, and Active Directory design updated.
- IAM + Identity Governance/IGA added to the career/lab direction.
- Free cybersecurity/security-tool roadmap added.

## Next Starting Point

**Do not recreate the domain, OUs, users, roles, or managers.**

Resume with:

1. Create Active Directory security groups.
2. Assign users to the correct groups.
3. Implement and test RBAC / least-privilege access.
4. Continue documenting every configuration and roadblock.

After the identity foundation is complete, move into server/domain hardening, endpoint protection, network segmentation/firewalling, VPN/secure remote access, vulnerability management, centralized logging/SIEM, incident response, automation, and cloud IAM concepts using free tools whenever possible.
