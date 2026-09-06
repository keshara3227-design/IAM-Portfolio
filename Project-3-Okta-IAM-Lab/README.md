# Project 3 — Okta IAM Lab

## Okta — Identity & Application Access Lab

**Project Type:** Simulated IAM Portfolio Project  
**Organization:** Acme Corporation (Simulated)  
**Technology:** Okta  
**Focus:** Identity Administration, Application Access, MFA, Audit Logging, JML

## Project Overview

This project simulates an enterprise Identity and Access Management environment using Okta.

The objective was to demonstrate practical IAM activities including identity provisioning, group-based access management, application assignment, authentication policy review, System Log investigation, and Joiner-Mover-Leaver lifecycle management.

## IAM Activities

### User Administration

- Created and activated a Finance test user
- Configured department and job title attributes
- Managed user lifecycle status
- Reviewed user activity through the Okta System Log

### Group-Based Access

Department-based groups were created and managed:

- ACME-HR
- ACME-Finance
- ACME-IT
- ACME-Sales

The Finance test user was added to ACME-Finance.

ACME-Finance was assigned access to the Zendesk application.

### Application Access

Zendesk application access was provisioned through group membership.

The application used Secure Web Authentication (SWA).

The Okta System Log confirmed successful application membership assignment.

During application testing, the Finance test user encountered a 404 error when launching Zendesk. The issue was documented as an application launch/authentication limitation rather than an Okta group-assignment failure.

### MFA & Authentication Policies

The Okta App Sign-In authentication policy was reviewed.

The applicable policy required any two authentication factors for supported applications.

Okta Verify and other available authenticators were reviewed as part of the security configuration exercise.

### System Log Analysis

Okta System Log events were reviewed to validate identity and access-management actions.

Examples included:

- Create Okta user — Success
- Activate user — Success
- Add user to group membership — Success
- Application membership — Success
- Update user profile — Success
- Remove user from group membership — Success
- Remove application membership — Success
- Deactivate Okta user — Success
- Clear user session — Success

## Mover Scenario

The Finance test user was simulated as an employee transferring from Finance to IT.

### Before

- Department: Finance
- Job Title: Finance Analyst
- Group: ACME-Finance
- Zendesk access

### Changes

- Department changed to Information Technology
- Job title changed to IT Support Specialist
- ACME-Finance membership removed
- Zendesk application membership removed
- ACME-IT membership added

System Log events were reviewed to validate the access changes.

### Result

The user's previous Finance-based access was removed before new IT group membership was provisioned.

## Leaver Scenario

The test user was then used to simulate employee offboarding.

### Actions

- Okta user account deactivated
- Active user session cleared
- System Log reviewed to validate the lifecycle actions

The ACME-IT group relationship remained associated with the deactivated identity, preserving the user's identity and audit history.

## Security Controls Demonstrated

- Identity Lifecycle Management
- Role-Based Access Control
- Least Privilege
- Group-Based Access
- Application Access Management
- Multi-Factor Authentication
- Authentication Policies
- User Provisioning
- User Deprovisioning
- Session Management
- System Log Analysis
- Audit Evidence

## Key Learning Outcomes

This project demonstrated how identity attributes, groups, application assignments, authentication policies, and lifecycle controls work together to manage enterprise access.

The Mover exercise demonstrated removal of obsolete access during a role change and provisioning of access appropriate to the user's new responsibilities.

The Leaver exercise demonstrated account deactivation and session clearing as part of employee offboarding.

The project also reinforced the importance of troubleshooting access issues by separating identity, authorization, authentication, and application availability.

## Evidence

Screenshots documenting the Okta configuration, access assignments, System Log events, Mover lifecycle, and Leaver lifecycle are included with this project.

---

*This project uses simulated users, systems, and organizational data for educational and portfolio purposes.*
