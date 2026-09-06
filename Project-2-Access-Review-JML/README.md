# Project 2 — Access Review & JML Governance

## Acme Corporation — Access Review & Identity Lifecycle Governance

**Project Type:** Simulated IAM Portfolio Project  
**Organization:** Acme Corporation (Simulated)  
**Focus:** Access Reviews, Least Privilege, Identity Governance, Joiner-Mover-Leaver (JML)

## Project Overview

This project simulates a quarterly enterprise access review and identity lifecycle governance process for Acme Corporation.

The objective was to evaluate user access, identify excessive or outdated permissions, validate business justification, and document remediation recommendations.

## Access Review

A simulated access review was performed for 10 users across HR, Finance, IT, and Sales.

The review evaluated:

- User identity and job role
- Department
- Manager
- Application
- Access level
- Group or role
- Business justification
- Review decision
- Recommended remediation
- Approver
- Reason for decision

## Key Findings

The review identified several access governance issues, including:

- Outdated access following a role change
- Excessive administrative privileges
- Contractor access requiring validation
- Application access requiring business justification
- Missing or inconsistent organizational reporting information

### Example Remediation

A Finance user retained access to HR records after transferring from HR to Finance.

**Recommendation:** Remove the outdated HR access and maintain only the access required for the user's current Finance role.

An IT support user was assigned Global Administrator privileges that exceeded the responsibilities documented for the role.

**Recommendation:** Remove excessive privileges and assign a lower-privilege administrative role based on confirmed responsibilities.

## JML Governance

A Joiner-Mover-Leaver workflow was designed to establish consistent identity lifecycle controls.

### Joiner

HR/Manager Request  
→ Manager Approval  
→ Identity Creation  
→ Approved Access Assignment  
→ MFA Registration  
→ Verification  
→ Evidence Retained

### Mover

Role Change Identified  
→ Review Existing Access  
→ Approve New Access  
→ Remove Old Access  
→ Add New Access  
→ Verification  
→ Evidence Retained

### Leaver

HR Notification  
→ Disable Account  
→ Revoke Sessions  
→ Remove Access  
→ Verify Deprovisioning  
→ Evidence Retained

## Security Controls Demonstrated

- Access Reviews
- Access Certification
- Least Privilege
- Role-Based Access Control
- Separation of Duties
- Identity Lifecycle Management
- Access Remediation
- User Deprovisioning
- Approval and Accountability
- Audit Evidence

## Key Learning Outcomes

This project demonstrated how periodic access reviews can identify inappropriate, excessive, outdated, or unnecessary access.

The JML workflow demonstrated how access should be managed throughout the employee lifecycle, from onboarding through role changes and eventual offboarding.

The project reinforced the importance of ensuring that users have the **right access, for the right reason, for the right amount of time**, with appropriate approval and evidence.

## Evidence

The project includes access review documentation and a JML lifecycle workflow.

---

*This project uses simulated users, systems, and organizational data for educational and portfolio purposes.*
