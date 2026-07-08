# ServiceNow ITSM Help Desk Lab

**Platform:** ServiceNow Personal Developer Instance (dev425764)  
**Instance Version:** Australia (Latest Release)  
**Status:** Complete ✅

---

## Project Overview

This lab documents the setup and use of a ServiceNow Personal Developer Instance (PDI) to simulate a real enterprise IT help desk environment. Three Tier 1 incident tickets were created and resolved from start to finish, demonstrating the full ITSM ticket lifecycle — from caller intake to resolution documentation and ticket closure.

ServiceNow is the most widely used IT Service Management (ITSM) platform in the world, deployed by Fortune 500 companies, government agencies, and managed service providers. This lab provides hands-on experience with the same platform used by enterprise help desk teams daily.

---

## Environment Setup

| Component | Details |
|-----------|---------|
| Platform | ServiceNow Personal Developer Instance |
| Instance ID | dev425764 |
| Version | Australia (Latest Release) |
| Access Level | Admin |
| Module Used | Incident Management |

### Provisioning Process
1. Created a free ServiceNow Developer account at developer.servicenow.com
2. Verified email address
3. Requested a Personal Developer Instance (PDI)
4. Received instance provisioning confirmation email
5. Logged into instance as Admin
6. Navigated to Incident module via Application Navigator

---

## Incident Tickets Created and Resolved

### Ticket 1 — Locked Out Account
**Incident Number:** INC0010007  
**Caller:** David Miller  
**Category:** Inquiry / Help | Login / Password  
**Priority:** Medium  
**State:** Resolved ✅

**Scenario:**  
User David Miller called the help desk reporting he was unable to log in to his workstation. The system displayed an "Account Locked" error after multiple failed login attempts.

**Actions Taken:**
- Verified user identity via employee ID
- Located account in Active Directory Users and Computers
- Unlocked the account
- Advised user to attempt login

**Resolution Code:** Solution provided  
**Resolution Notes:** Account unlocked in Active Directory Users and Computers. User identity verified via employee ID prior to action. User confirmed successful login after account was unlocked. No further action required.

---

### Ticket 2 — Password Reset
**Incident Number:** INC0010008  
**Caller:** Marcus Williams  
**Category:** Inquiry / Help | Login / Password  
**Priority:** Low  
**State:** Resolved ✅

**Scenario:**  
User Marcus Williams contacted the help desk requesting a password reset after forgetting his domain password following a two-week vacation.

**Actions Taken:**
- Verified user identity via employee ID and manager confirmation
- Reset password in Active Directory Users and Computers
- Enabled "User must change password at next logon" flag
- Provided temporary password to user

**Resolution Code:** Solution provided  
**Resolution Notes:** Password reset in Active Directory. User must change password at next logon flag enabled. User confirmed successful login with temporary password.

---

### Ticket 3 — Terminated Employee Account Disable
**Incident Number:** INC0010010  
**Caller:** Sarah Johnson (HR Manager)  
**Category:** Inquiry / Help | Software  
**Priority:** High  
**State:** Resolved ✅

**Scenario:**  
HR Manager Sarah Johnson submitted an urgent request to disable the Active Directory account of terminated employee Thomas Harris (username: tharris). Per company security policy, all access must be revoked within one hour of termination.

**Actions Taken:**
- Received urgent request from HR
- Located account for tharris in Active Directory Users and Computers
- Disabled account immediately
- Moved account to Disabled Users OU
- Flagged email and remote access tokens for revocation
- Notified IT Security team per offboarding policy

**Resolution Code:** Solution provided  
**Resolution Notes:** Account for tharris located and disabled in Active Directory Users and Computers. Account moved to Disabled Users OU. IT Security team notified per offboarding policy. All actions completed within SLA window.

---

## Key Concepts Demonstrated

| Concept | Application in This Lab |
|---------|------------------------|
| **Ticket Lifecycle** | Created, updated, and resolved all tickets from open to closed |
| **Caller Verification** | Documented identity verification before taking action on all tickets |
| **Resolution Documentation** | Filled in Resolution Code and Resolution Notes on every ticket |
| **SLA Awareness** | Ticket 3 (terminated employee) treated as Priority 1 with time-sensitive resolution |
| **Security-Aware Offboarding** | Followed proper access revocation procedures for terminated employee |
| **ITSM Workflow** | Navigated Application Navigator, Incident module, and Resolution Information tab |

---

## Skills Demonstrated

- ServiceNow ITSM Platform Navigation
- Incident Management (Create, Update, Resolve, Close)
- Ticket Documentation and Resolution Notes
- Caller Intake and Identity Verification
- Priority and Impact Assessment
- SLA-Aware Ticket Handling
- Security-Aware Account Offboarding

---

## Connection to Active Directory Lab

The three scenarios in this lab are directly linked to the [Active Directory Home Lab](https://github.com/Marquisb2170506/active-directory-home-lab). The same tasks performed in Active Directory (account unlock, password reset, account disable) are now formally documented as ServiceNow incident tickets — demonstrating the complete IT support workflow from the technical action in AD to the business record in the ticketing system.

---

## Screenshots

Screenshots documenting the full lab from account provisioning to ticket resolution are included in the `/screenshots` folder of this repository.

---

## Contact

**Marquis Borney**  
Email: marquisb.2315@gmail.com  
Location: St. Louis, MO (Open to Remote)  
LinkedIn: [linkedin.com/in/marquis-borney](https://linkedin.com/in/marquis-borney)
