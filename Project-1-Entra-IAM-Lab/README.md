# Project 1 — Microsoft Entra ID IAM Lab

## Microsoft Entra ID — IAM Lifecycle & Access Control

**Project Type:** Simulated IAM Portfolio Project  
**Organization:** Acme Corporation (Simulated)  
**Technology:** Microsoft Entra ID  
**Focus:** Identity Lifecycle Management, RBAC, MFA, Conditional Access

## Project Overview

This project simulates an enterprise Microsoft Entra ID environment for Acme Corporation.

The objective was to demonstrate practical Identity and Access Management concepts including user administration, group-based access, role-based access control, least privilege, MFA, Conditional Access, and Joiner-Mover-Leaver (JML) lifecycle management.

## IAM Activities

### Identity Administration
- Created and managed simulated users
- Created department-based security groups
- Assigned users to appropriate groups
- Assigned Microsoft Entra licenses

### Role-Based Access Control
- Assigned the Microsoft Entra User Administrator role to an IT administrator
- Applied the principle of least privilege
- Avoided unnecessary Global Administrator privileges

### Conditional Access & MFA
- Created a Conditional Access policy requiring MFA for Sales users
- Tested the policy using a simulated Sales user
- Reviewed sign-in activity to validate policy enforcement

### Mover Scenario
Simulated an employee transfer from Human Resources to Finance.

- Changed department and job title
- Removed the user's previous HR group membership
- Added the user to the Finance group
- Verified the access change

### Leaver Scenario
Simulated employee offboarding.

- Disabled the user's account
- Revoked active sessions
- Removed application/group access
- Verified the account was disabled

## Security Controls Demonstrated

- Role-Based Access Control (RBAC)
- Least Privilege
- Multi-Factor Authentication (MFA)
- Conditional Access
- Group-Based Access
- Identity Lifecycle Management
- Joiner-Mover-Leaver (JML)
- User Deprovisioning
- Sign-In Log Review

## Key Learning Outcomes

This project demonstrated how identity attributes, groups, roles, authentication controls, and lifecycle processes work together to manage access to enterprise resources.

It also reinforced the importance of removing obsolete access when employees change roles and promptly disabling accounts when employees leave an organization.

## Evidence

Screenshots documenting the configuration and testing activities are included in the `screenshots` directory.

---

*This project uses a simulated organization and test identities for educational and portfolio purposes.*
